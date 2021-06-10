# Answer questions a–g for the graph defined by the following sets:

The graph defined by the following sets:
N = {1, 2, 3, 4, 5, 6, 7}
N0 = {1}
Nf = {7}
E = {(1, 2), (1, 7), (2, 3), (2, 4), (3, 2), (4, 5), (4, 6), (5, 6), (6, 1)}

Also consider the following (candidate) test paths:
p1 = [1, 2, 4, 5, 6, 1, 7]
p2 = [1, 2, 3, 2, 4, 6, 1, 7]
p3 = [1, 2, 3, 2, 4, 5, 6, 1, 7]

## a) Draw the graph.<br>
![image](https://raw.githubusercontent.com/ibiann/Software-Testing-2021-USTH/main/PhamChiTrung/Img%207.2.2.5.PNG)

## b) List the test requirements for Edge-Pair Coverage:<br>
The Edge-Pair Coverage are: [1, 2, 3], [1, 2, 4], [2, 3, 2], [2, 4, 5], [2, 4, 6], [3, 2, 3], [3, 2, 4], [4, 5, 6], [4, 6, 1], [5, 6, 1], [6, 1, 2], [6, 1, 7]

## c) Does the given set of test paths satisfy Edge-Pair Coverage?<br>
No, it doesn't. 
t0 and t1 do not tour edges: [3, 2, 3], [6, 1, 2].

## d) Consider the simple path [3, 2, 4, 5, 6] and test path [1, 2, 3, 2, 4, 6, 1, 2, 4, 5, 6,
1, 7]. Does the test path tour the simple path directly? With a sidetrip? If so, write
down the sidetrip.<br>
The test path tours with a sidetrip is [4, 6, 1, 2, 4].

## f) List test paths from the given set that achieve Node Coverage but not Edge Coverage on the graph.<br>
The path that achieve Node Coverage but not Edge Coverage on the graph is [1, 2, 3, 2, 4, 5, 6, 1, 7]

## g) List test paths from the given set that achieve Edge Coverage but not Prime Path Coverage on the graph.<br>
The path that achieve Edge Coverage but not Prime Path Coverage on the path are: [1, 2, 3, 2, 4, 5, 6, 1, 7] and [1, 2, 4, 6, 1, 7]

## e) List the test requirements for Node Coverage, Edge Coverage, and Prime Path Coverage on the graph.<br>
Node coverage: TR = {1,2,3,4,5,6,7}
```
