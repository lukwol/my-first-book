# Chapter 1

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vitae porttitor ipsum. Proin semper condimentum leo nec laoreet. Aenean ut sollicitudin arcu, ac posuere elit. Nam a porta felis, sed fermentum sem. Duis nec velit diam. Praesent in sodales tellus. Donec nec rutrum felis.

```rust,noplayground
import envoy
import gleam/io

type Foo {
    Foo(name: String)
}

pub fn hello(name: String) -> String {
  "Hello " <> name <> "!"
}

pub fn main() -> Nil {
  let assert Ok(name) = envoy.get("GREET_NAME")

  name
  |> hello
  |> io.println
}
```
