# CSS Practice

## 1. Box sizing

**Question:** Make all elements use predictable border-box sizing, including pseudo-elements.

**Solution:**

```css
*,
*::before,
*::after {
  box-sizing: border-box;
}
```

## 2. Style a reusable card

**Question:** Give `.card` a white background, a subtle border, rounded corners, and internal spacing. Avoid fixed height so content can grow.

**Solution:**

```css
.card {
  padding: 1.25rem;
  border: 1px solid #d5dce3;
  border-radius: 0.75rem;
  background: #fff;
}
```

## 3. Center items with Flexbox

**Question:** Arrange the children of `.toolbar` in a row, vertically center them, and leave space between the first and last items.

**Solution:**

```css
.toolbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
}
```

## 4. Make a two-column layout adapt

**Question:** Show `.content` and `.sidebar` side by side when there is room, but stack them on narrow screens.

**Solution:**

```css
.layout {
  display: grid;
  grid-template-columns: minmax(0, 2fr) minmax(14rem, 1fr);
  gap: 1.5rem;
}

@media (max-width: 40rem) {
  .layout {
    grid-template-columns: 1fr;
  }
}
```
