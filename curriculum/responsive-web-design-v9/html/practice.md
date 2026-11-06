# HTML Practice

Try each prompt first, then compare with the solution. Solutions are intentionally small; extend them with your own content and test with a browser and accessibility checker.

## 1. Semantic article

**Question:** Create a page with a site header, navigation, one main article, and a footer. Use meaningful landmarks and a logical heading order.

**Solution:**

```html
<header>
  <a href="/">Field Notes</a>
  <nav aria-label="Main navigation">
    <a href="/journal">Journal</a>
    <a href="/about">About</a>
  </nav>
</header>
<main>
  <article>
    <h1>Growing herbs at home</h1>
    <p>A sunny window is a good place to begin.</p>
  </article>
</main>
<footer><p>Field Notes</p></footer>
```

## 2. Image with a useful text alternative

**Question:** Add an image of a red bicycle leaning against a brick wall. The alternative text should convey the useful information without starting with “image of.”

**Solution:**

```html
<figure>
  <img src="red-bicycle.jpg" alt="A red bicycle leans against a brick wall.">
  <figcaption>A bicycle parked outside the workshop.</figcaption>
</figure>
```

## 3. Labeled form

**Question:** Build a form that collects a visitor's name and email address. Both fields are required, and each needs a programmatically associated label.

**Solution:**

```html
<form action="/subscribe" method="post">
  <label for="name">Name</label>
  <input id="name" name="name" autocomplete="name" required>

  <label for="email">Email</label>
  <input id="email" name="email" type="email"
         autocomplete="email" required>

  <button type="submit">Subscribe</button>
</form>
```

## 4. Group related choices

**Question:** Let a user choose one preferred contact method. Group and name the radio controls accessibly.

**Solution:**

```html
<fieldset>
  <legend>Preferred contact method</legend>
  <label><input type="radio" name="contact" value="email" required> Email</label>
  <label><input type="radio" name="contact" value="phone"> Phone</label>
</fieldset>
```
