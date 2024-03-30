
Started with
``` rust
async fn root() -> &'static str {
    "Hello, World!"
}

```


Then added serilization via serde to a String.

Then Added type checking via `Json<Todo>`

then added state

took the code to ->
``` rust
async fn root(State(todos): State<Arc<Vec<Todo>>>) -> (StatusCode, Json<Vec<Todo>>) {
    (StatusCode::OK, Json(todos.as_ref().to_vec()))
}

```

