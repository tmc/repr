## Overview

Prints Go data structures as syntactically valid Go code. Useful for code generation. The name "repr" stands for "representation" and alludes to the Python function with the same name.

Solves a problem unaddressed by https://github.com/davecgh/go-spew/spew and directly competes with https://github.com/shurcooL/go-goon.

See godoc at https://godoc.org/github.com/tmc/repr.

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

See the API documentation at https://godoc.org/github.com/tmc/repr.

## License

https://en.wikipedia.org/wiki/WTFPL

## Misc

I'm receptive to suggestions. If this package _almost_ satisfies you but needs changes, open an issue or chat me up. Contacts: https://tmc.com/#contacts
