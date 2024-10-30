---
Link: https://medium.com/@rsinghal757/kadanes-algorithm-dynamic-programming-how-and-why-does-it-work-3fd8849ed73d
---
Top highlight

# Kadane’s Algorithm — (Dynamic Programming) — How and Why does it Work?

![[1_9X1XHsc69slW4Fk3t0t-w.jpeg]]

[Rohit Singhal](https://medium.com/@rsinghal757?source=post_page-----3fd8849ed73d--------------------------------)

·

[Follow](https://medium.com/m/signin?actionUrl=https%3A%2F%2Fmedium.com%2F_%2Fsubscribe%2Fuser%2F7175cbe2018a&operation=register&redirect=https%3A%2F%2Fmedium.com%2F%40rsinghal757%2Fkadanes-algorithm-dynamic-programming-how-and-why-does-it-work-3fd8849ed73d&user=Rohit+Singhal&userId=7175cbe2018a&source=post_page-7175cbe2018a----3fd8849ed73d---------------------post_header-----------)

6 min read

·

Dec 31, 2018

If you are here, then chances are that you were trying to solve the “Maximum Subarray Problem” and came across Kadane’s Algorithm but couldn’t figure out how something like that is working. Or maybe you were tired of using Kadane’s Algorithm as a “black-box”. Or maybe you wanted to understand the dynamic programming aspect of it. Or maybe you just want to learn about a new concept which can make you better at programming. Whatever the reason, you’ve come to the right place.

To better understand Kadane’s Algorithm, first, we would go through a short introduction of Dynamic Programming. Then, we would look at a quite popular programming problem, the Maximum Subarray Problem. We would see how this problem can be solved using a brute force approach and then we would try to improve our approach and come up with a better algorithm, aka, Kadane’s Algorithm.

So, let’s get into it.

## Dynamic Programming

Dynamic Programming is a method for solving a complex problem by breaking it down into a collection of simpler subproblems, solving each of those subproblems just once, and storing their solutions using a memory-based data structure (array, map, etc.). So the next time the same sub-problem occurs, instead of recomputing its solution, one simply looks up the previously computed solution, thereby saving computation time.

> Those who cannot remember the past are condemned to repeat it. — Dynamic Programming

Here’s a brilliant explanation on the concept of Dynamic Programming on Quora — [Jonathan Paulson’s answer to How should I explain dynamic programming to a 4-year-old?](https://www.quora.com/How-should-I-explain-dynamic-programming-to-a-4-year-old/answer/Jonathan-Paulson)

Though there’s more to dynamic programming, we would move forward to understand the Maximum Subarray Problem.

## Maximum Subarray Problem

The **maximum subarray problem** is the task of finding the largest possible sum of a contiguous subarray, within a given one-dimensional array A[1…n] of numbers.

Maximum Sum Subarray (In Yellow)

![[1li8Wlm3ZpInWLvpJ3yE9Iw.png]]

For example, for the array given above, the contiguous subarray with the largest sum is [4, -1, 2, 1], with sum 6. We would use this array as our example for the rest of this article. Also, we would assume this array to be zero-indexed, _i.e._ -2 would be called as the ‘0th’ element of the array and so on. Also, _**A[i]**_ would represent the value at index _**i**_.

Now, we would have a look at a very obvious solution to the given problem.

## Brute Force Approach

One very obvious but not so good solution is to calculate the sum of every possible subarray and the maximum of those would be the solution. We can start from index _**0**_ and calculate the sum of every possible subarray starting with the element _**A[0],**_ as shown in the figure below. Then, we would calculate the sum of every possible subarray starting with _**A[1]**_, _**A[2]**_ and so on up to _**A[n-1]**_,where _**n**_ denotes the size of the array (n = 9 in our case). Note that every single element is a subarray itself.

Brute Force Approach: Iteration 0 (left) and Iteration 1 (right)

![[1xm44zdqIv-pA2nGxCvbyBQ.png]]

We will call the maximum sum of subarrays starting with element _**A[i]**_ the _**local_maximum**_ at index _**i**_. Thus after going through all the indices, we would be left with _local_maximum_ for all the indices. Finally, we can find the maximum of these _local_maximum_s and we would get the final solution, _i.e_. the maximum sum possible. We would call this the _global_maximum_.

But you might notice that this is not a very good method because as the size of array increases, the number of possible subarrays increases rapidly, thus increasing computational complexity. Or to be more precise, if the size of the array is _**n**_, then the time complexity of this solution is _**O(n²)**_ which is not very good.

How can we improve this? Is there any way to use the concept of dynamic programming? Let’s find out.

## Kadane’s Algorithm

In this section, we would use the brute force approach discussed above again, but this time we would start backward. How would that help? Let’s see.

We would start from the last element and calculate the sum of every possible subarray ending with the element _**A[n-1]**_, as shown in the figure below. Then, we would calculate the sum of every possible subarray ending with _**A[n-2]**_, _**A[n-3]**_ and so on up to _**A[0]**_.

Backward Brute Force Approach: Iteration 0 (left) and Iteration 1 (right)

![[1QX8X7aC5fJlOMTmvrgUSkg.png]]

Now let’s focus on the subarrays ending with the element _**A[4]**_ (=-1) and _**A[5]**_ (=2) shown in the figure below.

![[1UrQhblF8B-6QoEC6E7kWow.png]]

From the figure above, we see that the _**local_maximum[4]**_ is equal to 3 which is the sum of the subarray [4, -1]. Now have a look at the subarrays ending with _**A[5]**_. You’ll notice that these subarrays can be divided into two parts, the subarrays ending with _**A[4]**_ (highlighted with yellow) and the single element subarray _**A[5]**_ (in green).

Let’s say somehow I know the _**local_maximum[4]**_. Then we see that to calculate the _**local_maximum[5]**_, we don’t need to compute the sum of all subarrays ending with _**A[5]**_ since we already know the result from arrays ending with _**A[4]**_. Note that if array [4, -1] had the maximum sum, then we only need to check the arrays highlighted with the red arrows to calculate _**local_maximum[5]**_. And this leads us to the principle on which Kadane’s Algorithm works.

> local_maximum at index i is the maximum of A[i] and the sum of A[i] and local_maximum at index i-1.

![[1mNAvwJ23ljNMthrgZfRYXg.png]]

This way, at every index _**i**_, the problem boils down to finding the maximum of just two numbers, _**A[i]**_ and _**(A[i] + local_maximum[i-1])**_. Thus the maximum subarray problem can be solved by solving these sub-problems of finding _**local_maximums**_ recursively. Also, note that _**local_maximum[0]**_ would be _**A[0]**_ itself.

Using the above method, we need to iterate through the array just once, which is a lot better than our previous brute force approach. Or to be more precise, the time complexity of Kadane’s Algorithm is _**O(n)**_.

Finally, let’s see how this all would work in code.

## Code Walkthrough

Below is a very much self-explanatory implementation (in C++) of a function which takes an array as an argument and returns the sum of the maximum subarray.

![[1rgcPr2WFkToaDBknC9IXBA.png]]

Note that instead of using an array to store _**local_maximums**_, we are simply storing the latest _**local_maximum**_ in an _int_ type variable ‘_local_max_’ because that’s what we need to calculate next _**local_maximum**_. Also, as we are using a variable ‘_global_max_’ to keep track of the maximum value of _**local_maximum**_, which in the end comes out to be the required output.

## Conclusion

Because of the way this algorithm uses optimal substructures (the maximum subarray ending at each position is calculated in a simple way from a related but smaller and overlapping subproblem: the maximum subarray ending at the previous position) this algorithm can be viewed as a simple example of dynamic programming. Kadane’s algorithm is able to find the maximum sum of a contiguous subarray in an array with a runtime of _**O(n)**_.