# Lists

# Example Go Code
```go
package main
import(
"fmt"
"container/list"
)
func main() { 
        var intList list.List
            intList.PushBack(11)
            intList.PushBack(23)
            intList.PushBack(34)
    for element := intList.Front(): element !=nil:
    element = element.Next() {
        fmt.Println(element.Value.(int))
    }
}
```

## A list is a sequence of elements.

### Each element can be connected to another 

- with a link in a forward or backward direction
- The element can have other payload properties
- Lists are a basic type of container
- They have variable length
- Easier to remove or add elemets than an array

### Data items 
   - within a list 
        - not required to be contiguous (in sequence)
         - in memory or disk

Linked lists were proposed by Allen Newll, Cliff Shaw, and Herbert A. Simon at RAND Corp.    

