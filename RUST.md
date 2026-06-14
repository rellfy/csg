# Rust code style guide

## 1 Avoid tuple structs
Instead of using a tuple struct, prefer using a struct with named properties.

**Reason**: readability, maintainability.

## 2 Prefer match
Use `match` over `if` for ternary operations.

## 3 Direct inline imports
Prefer to use imported types directly, rather than their modules.

e.g. prefer to use `Type` directly rather than `dependency::Type`.

## 4 Escape long strings
Escape long strings with `\` and a line break to keep them readable.

