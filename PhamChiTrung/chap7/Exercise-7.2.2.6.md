# Exercise 7.2.2.6
(a) List the test requirements for Node Coverage, Edge Coverage,
and Prime Path Coverage on the graph.<br>
(b) List test paths that achieve Node Coverage but not Edge
Coverage on the graph.<br>
(c) List test paths that achieve Edge Coverage but not Prime PathCoverage on the graph.
```
a)   TR Node coverage: [1] [4] [5] [2] [6] [3] [7] [8] [9] [10]
     TR Edge coverage: [1,4] [1,5] [2,5] [2,6] [3,6] [3,7] [4,8] [5,8] [5,9] [6,9] [6,10] [7,10]
     TR Prime path coverage: [2,5,8] [2,5,9] [1,5,9] [1,4,8] [1,5,8] [2,6,9] [3,6,10] [3,7,10] [3,6,9] [2,6,10]
