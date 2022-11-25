# RB-tree
<br>DAA Assignment
<br>Name:Harsh Sherekar
<br>Roll no :A_42(5th sem)
# Introduction
The red-Black tree is a binary search tree.Each node in the Red-black tree contains an extra bit that represents a color to ensure that the tree is balanced during any operations performed on the tree like insertion, deletion, etc. In a binary search tree, the searching, insertion and deletion take O(log2n) time in the average case, O(1) in the best case and O(n) in the worst case.
# Rules for red black tree:
<br>Every node has a color either red or black.
<br>The root of the tree is always black.
<br>There are no two adjacent red nodes (A red node cannot have a red parent or red child).
<br>Every path from a node (including root) to any of its descendants NULL nodes has the same number of black nodes.
<br>All leaf nodes are black nodes.

#Insertions in red black tree
<br>While inserting a new node, the new node is always inserted as a RED node. After insertion of a new node, if the tree is violating the properties of the red-black tree then, we do the following operations.

<br>Recolor
<br>Rotation
#Rotations in red black tree
<br>There are two types of rotations:

<br>Left Rotation
<br>Right Rotation
<br>In left rotation, we assume that the right child is not null. Similarly, in the right rotation, we assume that the left child is not null.
 # Algorithms
 # Left rotate
 ```
 LEFT ROTATE (T, x)
1.y ← right [x]
2.y ← right [x]
3.right [x] ← left [y]
4.p [left[y]] ← x
5.p[y] ← p[x]
6.If p[x] = nil [T] then root [T] ← y else if x = left [p[x]] then left [p[x]] ← y else right [p[x]] ← y
7.left [y] ← x.
8.p [x] ← y.
 ```
 # Right rotate
 ```
 LEFT ROTATE (T, x)

1.y ← left [x]
2.y ← left [x]
3.left [x] ← right [y]
4.p [right[y]] ← x
5.p[y] ← p[x]
6.If p[x] = nil [T] then root [T] ← y else if x = left [p[x]] then left [p[x]] ← y else right [p[x]] ← y
7.right [y] ← x.
8.p [x] ← y.
 ```
<br>Right left rotation can be done by first shifting to left and then right.
<br>Left right rotation can be done by first shifting to the right and then left.
# Operations performed in the code:
<br>1.Left rotate 
<br>2.Right rotate
<br>3.Insert
<br>4.Delete

# Applications of rb tree:
<br>1.In the java collections library,TreeSet,TreeMap and hashmap are implemented using the red black tree.
<br>2.The Completely Fair Scheduler in the Linux kernel uses this data structure.
<br>3.MySQL also uses Red-Black Tree indexing to reduce the searching and insertion time.
<br>4.To implement Standard Template Libraries (STL) in C++: multiset, map, multimap.
<br>5.To implement finite maps.








