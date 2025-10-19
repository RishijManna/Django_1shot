# Day 1 — Foundations + HTML Essentials (Teacher mode)

## Aim for Day 1

By the end of Day 1 you will:

1. Have a proper development environment set up (editor, terminal, Git basics).
2. Understand the HTML5 document skeleton and semantic tags.
3. Be able to create a simple, valid web page (HTML file), include images and links.
4. Know how to use browser DevTools to inspect and debug HTML.
5. Complete small exercises to cement learning.

> Save this file as Day1-notes.md or copy-paste into your notebook. Do all exercises in a folder called day1-html.
> 

---

## 1. Setup & tools (quick, do this first)

**What you need**

- VS Code (or any code editor): install VS Code and these extensions: *Prettier*, *Live Server*, *HTML CSS Support* (optional).
- Browser: Chrome or Firefox (we’ll use DevTools).
- Git (basic): `git init`, `git add`, `git commit`.
- File structure for Day1:

```
learn-django-notes/
  day1-html/
    index.html
    images/
```

**Quick commands**

- Create folder and open VS Code:
    - Windows: `mkdir learn-django-notes && cd learn-django-notes && mkdir day1-html && code.`
    - Linux/Mac similar.
- Init git (optional):

```bash
cd day1-html
git init
echo "Day 1 notes" > README.md
git add README.md
git commit -m "Start Day 1"
```

---

## 2. The HTML5 skeleton (core concept)

### Explanation

Every HTML page must start with the HTML5 doctype and basic structure. This tells the browser how to interpret the file.

### Example — create `index.html`

Create file `day1-html/index.html` and paste:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Day 1 — HTML Basics</title>
</head>
<body>
  <header>
    <h1>Welcome — Day 1</h1>
    <p>Learning HTML fundamentals.</p>
  </header>

  <main>
    <section>
      <h2>Introduction</h2>
      <p>This page demonstrates a basic HTML5 structure.</p>
    </section>
  </main>

  <footer>
    <small>© Day 1</small>
  </footer>
</body>
</html>

```

**Action:** Open this file in the browser (double click or use Live Server in VS Code). You should see the headings and paragraph.

**Why these tags matter**

- `<!DOCTYPE html>`: switch browser to standards mode.
- `<html lang="en">`: language helps accessibility & SEO.
- `<meta charset="utf-8">`: character encoding (always include).
- `<meta name="viewport"...>`: makes layouts responsive on mobile.

---

## 3. Headings, paragraphs, line breaks, and semantic grouping

### Headings

- `<h1>` — main title, use only **one** per page ideally.
- `<h2>` .. `<h6>` — subsections.

### Paragraphs & breaks

- `<p>` for paragraphs.
- `<br>` for forced line breaks (use sparingly).

### Semantic grouping

- `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>` — use to describe page parts. Browsers & screen readers benefit.

### Example

Add to `index.html` inside `<main>`:

```html
<nav>
  <a href="#intro">Intro</a> |
  <a href="#examples">Examples</a>
</nav>

<section id="examples">
  <h3>Text Examples</h3>
  <p>This is a paragraph.<br>Here is the same paragraph with a line break.</p>
</section>

```

**Practice 1:** Add one `<article>` under main with an `<h3>` and two paragraphs about a hobby.

---

## 4. Links, images, and attributes

### Links (anchors)

- `href` — destination.
- `target="_blank"` opens in new tab (add `rel="noopener"` for security).

```html
<a href="https://developer.mozilla.org" target="_blank" rel="noopener">MDN Web Docs</a>

```

### Images

- `src` — image path
- `alt` — required for accessibility (describe image)

```html
<img src="images/sample.jpg" alt="Sample image of a sunrise" width="400">

```

**Practice 2:**

1. Put an image in `day1-html/images/` called `sample.jpg`.
2. Add an `<img>` tag to `index.html` with a meaningful `alt`. Resize using `width` or better with CSS later.

**Important note:** Always include `alt`. If an image is purely decorative, use `alt=""` (empty string) to tell screen readers to skip it.

---

## 5. Lists and definition lists

### Unordered list

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

```

### Ordered list

```html
<ol>
  <li>Install tools</li>
  <li>Write HTML</li>
</ol>

```

### Definition list

```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
</dl>

```

**Practice 3:** Create an ordered list titled “Steps to create a web page” with 4 items in an appropriate section.

---

## 6. Tables (basics)

Use tables for tabular data (not for layout).

```html
<table border="1">
  <thead>
    <tr><th>Medicine</th><th>Qty</th><th>Price</th></tr>
  </thead>
  <tbody>
    <tr><td>Paracetamol</td><td>20</td><td>50</td></tr>
    <tr><td>Ibuprofen</td><td>10</td><td>75</td></tr>
  </tbody>
</table>

```

**Practice 4:** Add a small table to your page representing 3 items with columns: name, category, price.

---

## 7. Forms (intro) — HTML side only (we’ll handle server side later)

**Basic form**

```html
<form action="/submit" method="post">
  <label for="name">Name</label>
  <input id="name" name="name" type="text" placeholder="Your name" required>

  <label for="email">Email</label>
  <input id="email" name="email" type="email" placeholder="you@example.com">

  <button type="submit">Send</button>
</form>

```

**Key points**

- `name` attribute: critical — this is the key used when the form is submitted.
- `id` connects `<label>` to `<input>` for accessibility.
- `required` enforces a browser-level validation.
- `type="email"` gives basic validation that input looks like an email.

**Practice 5:** Add a contact form with `name`, `email`, `message` (textarea) to your page. Don’t worry about server handling yet.

---

## 8. Using Developer Tools (inspect & live edit)

**How to inspect**

1. Right-click the element → Inspect (Chrome) or `F12`.
2. Explore Elements panel to see HTML structure and CSS rules.
3. Use Console to test JS: `document.querySelector('h1').textContent`.

**Practice 6:**

- Open DevTools → Select the `<h1>` on your page → change its text in Elements panel and see live change.
- In Console, run:

```jsx
document.querySelector('h1').style.color = 'green';

```

---

## 9. Mini-quiz (self-check — write answers in your notebook)

1. What tag do you always put at the top of an HTML5 document?
2. Why is `alt` important on `<img>`?
3. How do you group radio buttons so only one can be selected? (Hint: `name`)
4. What attribute must an input have so the server receives it?
5. Which tags are semantic alternatives to `<div>`?

(Answers are: `<!DOCTYPE html>`, accessibility & fallback, same `name` attribute for radio, `name` attribute, examples: `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<footer>`.)

---

## 10. Recommended tiny projects for Day 1 (practice)

- **Project A — Simple profile page**
    - Single HTML page with header, short bio (`<p>`), profile image, list of skills, and a contact form.
- **Project B — Small product table**
    - Add a table with 5 products and style widths via inline attribute for now (we’ll do CSS tomorrow).

**Do at least Project A.** Commit your changes to git after each milestone.

---

## 11. Common pitfalls & quick tips

- Don’t forget closing tags for non-void elements (`<p></p>`, `<div></div>`).
- Use semantic tags instead of lots of `<div>`s — easier to remember and better for screen readers.
- `id` must be unique per page; `class` can repeat.
- Use meaningful alt text for images (not “image1.jpg”).
- Name form inputs (e.g., `name="email"`) — otherwise server gets nothing.

---

## 12. What I expect you to hand me (when you come back)

When you’re done with Day 1, tell me “Day 1 done” and include:

- A short note: 3 things you learned, 2 things you struggled with.
- Optional: paste the `index.html` you created or describe one issue you encountered.

Then I’ll provide **Day 2** that builds on Day 1: CSS basics (box model, selectors, inline vs external), Flexbox intro, and then move into accessible forms and best practices + hands-on tasks.

---

## Quick reference cheatsheet (keep visible)

- HTML skeleton:

```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1"><title>...</title></head>
<body>...</body>
</html>

```

- Link:

```html
<a href="URL" target="_blank" rel="noopener">Link text</a>

```

- Image:

```html
<img src="path" alt="description">

```

- Form element:

```html
<label for="id">Label</label>
<input id="id" name="fieldname" type="text" required>

```

- List example:

```html
<ul><li>Item</li></ul>

```
