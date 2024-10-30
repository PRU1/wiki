---
Link: https://dmoj.ca/problem/utso15p6
---
Ms. Evans is creating a new, eye-catching design for her company headquarters. She thinks the Royal Ontario Museum is really cool, so she has modeled her design after its jumbled-together look:

![[b6f23d7c-5813-4d91-b3ee-71b9579aa920.png]]

Specifically, the shape of the headquarters will be the union of two tetrahedra. Ms. Evans will cover the outside entirely with glass, and she wants to know how much glass she will need. What is the surface area of the headquarters?

### Input Specification

The input will consist of 8 lines, each line specifying a point with 3 integer coordinates in the range [0,1000]. The first 4 lines describe the vertices of the first tetrahedron; the last 4 lines describe the second tetrahedron.

### Output Specification

A single line containing the answer to the problem. Your answer will be considered correct if its absolute or relative error does not exceed 10−6.

### Note

The input will satisfy the following conditions:

- No three of the specified points will lie on a line.
- Both tetrahedra will have positive volume.
- Let a1 be a vertex of a tetrahedron and let b1,b2,b3 be vertices of the other tetrahedron. It is guaranteed that a1 does not lie on the plane formed by b1,b2,b3.
- Let a1,a2 be vertices of a tetrahedron and let b1,b2 be vertices of the other tetrahedron. It is guaranteed that the line passing through a1 and a2 does not intersect the line passing through b1 and b2.

### Partial Marks

In test cases worth 10% of the points, the tetrahedra will not intersect.

### Sample Input 1

Copy

```Plain
1 17 12
13 9 4
102 7 7
76 32 42
500 500 500
502 500 500
500 501 500
503 501 504
```

### Sample Output 1

Copy

```Plain
5122.604324
```

### Explanation for Sample Output 1

The tetrahedra do not intersect, so the answer is the sum of their surface areas.

### Sample Input 2

Copy

```Plain
0 0 0
10 0 0
0 10 0
0 0 10
1 1 1
2 1 1
1 2 1
1 1 2
```

### Sample Output 2

Copy

```Plain
236.6025404
```

### Explanation for Sample Output 2

The second tetrahedron is completely enclosed by the first tetrahedron, so the answer is the surface area of the first tetrahedron.

### Sample Input 3

Copy

```Plain
0 0 0
10 0 0
5 5 0
5 5 6
15 2 1
-4 10 4
-10 4 12
-3 -11 3
```

### Sample Output 3

Copy

```Plain
700.85581333
```

### Picture for Sample Input 3

![[8cc38248-8d4d-48db-829c-e43537657799.png]]

### Sample Input 4

Copy

```Plain
2 0 0
0 2 0
4 1 0
2 2 3
2 0 2
0 2 2
4 1 2
2 2 5
```

### Sample Output 4

Copy

```Plain
35.50054500
```

### Picture for Sample Input 4

![[1c511665-d1ed-4a48-805a-2e0b1301dc93.png]]