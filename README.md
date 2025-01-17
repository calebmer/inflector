# Rust Inflector


[![Build Status](https://travis-ci.org/whatisinternet/inflector.svg?branch=master)](https://travis-ci.org/whatisinternet/inflector) [![Crates.io](https://img.shields.io/crates/v/inflector.svg)](https://crates.io/crates/inflector)

Adds String based inflections for Rust. Snake, kebab, camel,
sentence, class, title, upper, and lower cases as well as ordinalize,
deordinalize, demodulize, deconstantize, foreign key, table case, and pluralize/singularize are supported as both traits and pure functions
acting on String types.

-----
## Documentation:

Documentation can be found here at the README or via rust docs below.

[Rust docs with examples](http://whatisinternet.github.io/inflector/doc/inflector/)

-----

## Installation:

### As a [crate](http://crates.io)
```toml
[dependencies]
Inflector = "0.2.0"
```

### Compile yourself:

1. Install [Rust and cargo](http://doc.crates.io/)
2. git clone https://github.com/whatisinternet/inflector
3. Library: cd inflector && cargo build --release --lib
4. You can find the library in target/release

## Usage:

```rust
...
// to use methods like String.to_lower_case();
extern crate inflector;
use inflector::Inflector;
...
fn main() {
...
  let camel_case_string: String = "some_string".to_string().to_camel_case();
...
}

```

Or

```rust
...
// to use methods like to_lower_case(String);
extern crate inflector;

// use inflector::cases::classcase::to_class_case;
// use inflector::cases::classcase::is_class_case;

// use inflector::cases::camelcase::to_camel_case;
// use inflector::cases::camelcase::is_camel_case;

// use inflector::cases::screamingsnakecase::to_screamingsnake_case;
// use inflector::cases::screamingsnakecase::is_screamingsnake_case;

// use inflector::cases::snakecase::to_snake_case;
// use inflector::cases::snakecase::is_snake_case;

// use inflector::cases::kebabcase::to_kebab_case;
// use inflector::cases::kebabcase::is_kebab_case;

// use inflector::cases::sentencecase::to_sentence_case;
// use inflector::cases::sentencecase::is_sentence_case;

// use inflector::cases::titlecase::to_title_case;
// use inflector::cases::titlecase::is_title_case;

// use inflector::cases::tablecase::to_table_case;
// use inflector::cases::tablecase::is_table_case;

// use inflector::cases::uppercase::to_upper_case;
// use inflector::cases::uppercase::is_upper_case;

// use inflector::cases::lowercase::to_lower_case;
// use inflector::cases::lowercase::is_lower_case;

// use inflector::cases::::to_lower_case;
// use inflector::cases::lowercase::is_lower_case;

// use inflector::numbers::ordinalize::ordinalize;
// use inflector::numbers::deordinalize::deordinalize;

// use inflector::suffix::foreignkey::to_foreign_key;
// use inflector::suffix::foreignkey::is_foreign_key;

// use inflector::string::demodulize::demodulize;
// use inflector::string::deconstantize::deconstantize;

// use inflector::string::pluralize::to_plural;
// use inflector::string::singularize::to_singular;
...
fn main() {
...
  let camel_case_string: String = to_camel_case("some_string".to_string());
...
}

```

-----
# Methods:

```rust
to_class_case(String) -> String
```

```rust
to_camel_case(String) -> String
```

```rust
to_screaming_snake_case(String) -> String
```

```rust
to_snake_case(String) -> String
```

```rust
to_kebab_case(String) -> String
```

```rust
to_sentence_case(String) -> String
```

```rust
to_title_case(String) -> String
```

```rust
to_table_case(String) -> String
```

```rust
to_upper_case(String) -> String
```

```rust
to_lower_case(String) -> String
```

```rust
ordinalize(String) -> String
```

```rust
deordinalize(String) -> String
```

```rust
demodulize(String) -> String
```

```rust
deconstantize(String) -> String
```

```rust
to_foreign_key(String) -> String
```

```rust
to_plural(String) -> String
```

```rust
to_singular(String) -> String
```

```rust
is_class_case(String) -> bool
```

```rust
is_camel_case(String) -> bool
```

```rust
is_screaming_snake_case(String) -> bool
```

```rust
is_snake_case(String) -> bool
```

```rust
is_kebab_case(String) -> bool
```

```rust
is_sentence_case(String) -> bool
```

```rust
is_title_case(String) -> bool
```

```rust
is_table_case(String) -> bool
```

```rust
is_upper_case(String) -> bool
```

```rust
is_lower_case(String) -> bool
```

```rust
is_foreign_key(String) -> bool
```

## Contributing

This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

1. Fork it ( https://github.com/whatisinternet/inflector/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
