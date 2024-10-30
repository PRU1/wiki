- example of [[divide and conquer]] recursive strategy
![[Pasted image 20240526152055.png]]
## divide
- split array into halves
## conquer 
- try to sort both subarrays. divide again if not at base case yet
## combine
- you have two sorted subarrays. use two pointers and merge them.

# pseudo code
```
mergeSort(A, p, r):
	if p > r
		return 
	q = (p+r)/2
	mergeSort(A, p, q)
	mergeSort(A, q+1, r)
	merge(A,p,q,r)
```
![[Pasted image 20240526153158.png]]
