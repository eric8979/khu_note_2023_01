## C++
- Template
```cpp
template <typename T>
T myMax(T x, T y){
	return (x > y) ? x : y;
}

int x = 7;
int y = 10;
add(x, y)

double a = 3.2;
double b = 2.8;
add(a, b)
```

---

## Array
- You know what it is...

## Stack & Queue
### Stack
- LIFO
```c
something.push("data")
something.pop()
top()
size()
empty()
```
### Queue
- FIFO

## Linked List
- weight
- direction

## Heap

## Tree & Graph
- Binary Tree
	- Binary Search Tree
		- Binary tree
		- left child < parent < right child

## Sorting (Big-O)
- Bubble sort (O(n^2))
![[bubble_sort.png]]
- Insertion sort (O(n^2))
	- Enlarge the sorted part of the array(left)
	- Say... left is sorted, right is unsorted
		- Choose left most element from the right and insert the value in sorted array in appropriate location.

- Selection sort
	- For each iteration, find the minimum and move it to the very last of the sorted mins

---

- Quick sort `(O(n*log(n)))`
	- Pick a Pivot element
	- Move every elements that are smaller than the Pivot to the left and vice versa.
 
- Merge sort
	- Break down the array until there's only one element
	- Merge them step-by-step
 
- Heap sort
	- Max (parent > child)
	- min (parent < child)
	- Heapify

---

- Binary expression
	- In-order: right-top-left
	- Pre-order: top-right-left
	- Post-order: right-left-top

- Recursion