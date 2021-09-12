# Tuples

## A finite sorted list of elements.

### go code example
```go
package main
import("fmt")
//return tuple of square and cube of integer "a"
func powerSeries(a int) (int,int) {
return a*a, a*a*a }

func main(){
// execute test return of a tuple
square, cube := powerSieries(3)
fmt.Println("Square ", square, "Cube", cube)
      }
```

### data structure that groups data
- typically immutable sequential collections
- the element has related fields of different datatypes.
- the only way to modify a tuple is to change the fields
- operators such as + and * can be applied to tuples
- database record is referred to as a tuple
