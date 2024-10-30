The recursive method of computing the nth term in a fibonacci sequence is slow because there are many repeated computations.

For example, consider the 5th term in the fibonacci sequence
![[Pasted image 20221229225931.png]]
Notice that fib(3) needs to be computed twice, fib(2) needs to be computed three times, etc.

This is a waste of time! What we can do instead is compute fib(3), fib(2), fib(1) once and store that value in memory for when the recursive function calls it again. 
This process is called **memiozation**. 

We can store the values we have already computed in an array. When we call function fib(int n), it will first check the array for a value.

Here's an alternate explananation: ![[Pasted image 20221231155355.png]]
Here's the completed program that stores computations:
```
int fib_mem(int n, vector<int>& past_results) {
	int result{};
	if (past_results[n] == -1) { // value has not been calculated yet
		if (n >= 3) {
			result = fib_mem(n - 1, past_results) + fib_mem(n - 2, past_results);
			past_results[n] = result;
		}
		else {
			result = 1;
		}
	}
	else {
		result = past_results[n];
		cout << "memiozation works yayyayayay \n";
	}
	return result;
}

int main() {
	int n = 40;
	vector<int> past_results(n+1, -1); // value not calculated yet is -1
	past_results[0] = 1; past_results[1] = 1; // initialize first two terms for speeeeed

	auto start = chrono::steady_clock::now(); // start timing
	cout << "without memiozation: " << fib(n) << "\n";

	auto non_memo_end = chrono::steady_clock::now(); // end timing
	auto memo_start = chrono::steady_clock::now(); // start timing

	cout << "with memiozation: " << fib_mem(n, past_results) << "\n";
	auto memo_end = chrono::steady_clock::now();

	// Find elapsed time
	double non_memo_time = double(chrono::duration_cast <chrono::milliseconds> (non_memo_end - start).count());
	double memo_time = double(chrono::duration_cast <chrono::milliseconds> (memo_end - memo_start).count());
	cout << "non memoized time (ms): " << non_memo_time << "\n";
	cout << "memoized time (ms): " << memo_time << "\n";


	return 0;
}
```