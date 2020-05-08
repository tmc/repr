## Overview

Prints Go data structures as syntactically valid Go code. 

https://godoc.org/github.com/tmc/repr.

## Example

```go
import "github.com/tmc/repr"

type Data struct {
  Number int
  String string
  List   []int
}

fmt.Println(repr.String(Data{
  Number: 123,
  String: "hello world!",
  List:   []int{10, 20, 30},
}))

/*
Data{
  Number: 123,
  String: "hello world!",
  List: []int{10, 20, 30},
}
*/
```
