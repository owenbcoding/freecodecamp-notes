# JavaScript Practice

Run the examples with Node.js or in a browser console. Each solution is a small pure function so its behavior is easy to test.

## 1. Normalize a display name

**Question:** Trim whitespace from a name and capitalize its first character. Return an empty string for non-string input or a name that contains only whitespace.

**Solution:**

```js
function normalizeName(value) {
  if (typeof value !== "string") return "";

  const name = value.trim();
  if (name.length === 0) return "";

  return name[0].toUpperCase() + name.slice(1).toLowerCase();
}

console.log(normalizeName("  aDa  ")); // "Ada"
```

## 2. Count values

**Question:** Return an object whose keys are the values in an array and whose values are their occurrence counts.

**Solution:**

```js
function countValues(values) {
  return values.reduce((counts, value) => {
    counts[value] = (counts[value] ?? 0) + 1;
    return counts;
  }, {});
}

console.log(countValues(["red", "blue", "red"]));
// { red: 2, blue: 1 }
```

## 3. Select passing scores

**Question:** From an array of scores, return the scores at least 70, sorted from highest to lowest. Do not mutate the input.

**Solution:**

```js
function passingScores(scores) {
  return scores
    .filter((score) => score >= 70)
    .toSorted((a, b) => b - a);
}

console.log(passingScores([60, 90, 72, 50])); // [90, 72]
```

`toSorted` is available in modern JavaScript runtimes. For older runtimes, sort a copy with `[...scores].sort(...)`.

## 4. Validate a simple password rule

**Question:** Return `true` only when a value is a string with at least eight characters and includes at least one number.

**Solution:**

```js
function isValidPassword(value) {
  return typeof value === "string"
    && value.length >= 8
    && /\d/.test(value);
}

console.log(isValidPassword("study2026")); // true
console.log(isValidPassword("short")); // false
```
