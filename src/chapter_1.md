# Chapter 1

Some description

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
