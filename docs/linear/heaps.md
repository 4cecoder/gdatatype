# Heaps

## A heap is a data structure that is based on the heap property
### A heap is a tree with the property that each node is the minimum-valued node in its subtree.

The minimum element in the tree is the root, at index 0.

A heap is a common way to implement a priority queue. To build a priority queue, implement the Heap interface with the (negative) priority as the ordering for the Less method, so Push adds items while Pop removes the highest-priority item from the queue. The Examples include such an implementation; the file example_pq_test.go has the complete source.

### Go code example
```go
package main
import("container/heap" "fmt")
type IntegerHeap []int
func(iheap IntegerHeap) Len() int {return len(iheap)}
func (iheap IntegerHeap) Less(i,j int) bool {return iheap[i]<iheap[j]}
func (iheap IntegerHeap) Swap(i,j int) { iheap[i], iheap[j]=iheap[j],iheap[i]}
func (iheap *IntegerHeap) Push(heapintf interface{}){
    *iheap=append(*iheap, heapintf.(int))}
func(iheap *IntegerHeap) Pop() interface{}{
    var n int
    var x1 int
    var prev IntegerHeap = *iheap
    n=len(prev)
    x1=prev[n-1]
    *iheap = prev[0:n-1]
    return x1
}    

func main(){
    var intHeap *IntegerHeap = &IntegerHeap{1,4,5}

    heap.Init(intHeap)
    heap.Push(intHeap,2)
    fmt.Printf("minimum: %d\n", (*intHeap)[0])
    for intHeap.Len() > 0 {
        fmt.Printf("%d \n", heap.Pop(intHeap))}
}

```


### Algorithms using heap data structures:
- selection
- graph 
- k-way merge 

### Operations preformed on heaps:
 - finding
 - merging 
 - insertion
 - key changes
 - deleting 

### in Go Heaps are imported from the package container/heap

heap order (maximum heap) property
- the value stored at each node
    - is greater than or equal to its children

    Order is descending:
     - it is refered to as a Maximum heap; 

    Order is acending:
    - refered to as a Minimum heap


### NOT a sorted data structure:
-  but partially ordered

heap data structure proposed by J.W.J. Williams in 1964 for a heap sorting algorithm.
