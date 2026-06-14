# JavaScript code style guide

## 1 ES6 Syntax
Where applicable, the code should use ES6 syntax over older standards.

For example, prefer arrow functions over a `function`.

**Reason**: consistency.

## 2. If statements should use brackets
If statements should use brackets, and span multiple lines.

Do:

```js
if (condition) {
  // Some code.
}
```

Don't:

```js
if (condition) // Some code.
```

This includes early returns.

**Reason**: consistency.

## 3. Avoid default exports
Prefer using regular exports instead.

**Reason**: Default exports have poor code completion support.

## 4. Prefer template strings
Prefer using template strings rather than string concatenation.

However, string concatenation may be used to keep the column count
under the limit of 80.

