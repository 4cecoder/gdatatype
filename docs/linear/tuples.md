# Tuples

## A finite sorted list of elements.

### go code example
```go
package main
import("fmt")
func powerSeries*a int) (int,int) {
return a*a, a*a*a
}
func main(){
var square int
var cube int
square, cube = powerSieries(3)
fmt.Println"Swuare ", square, "Cube", cube)
```

- data structure that groups data
- typically immutable sequential collections

- the element has related fields of different datatypes.
- the only way to modify a tuple is to change the fields
- operators such as + and * can be applied to tuples
- database record is referred to as a tuple
