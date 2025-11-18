# actix-friendly-json-extractor

A friendly JSON extractor for actix-web with detailed error messages using `serde_path_to_error`.

## Usage

```rust
use actix_friendly_json_extractor::FriendlyJson;

#[post("/endpoint")]
async fn handler(payload: FriendlyJson<MyStruct>) -> impl Responder {
    // Use payload.into_inner() to access your data
}
```
