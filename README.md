# Tailwind CSS Setup using CLI

This guide will help you quickly set up **Tailwind CSS** in your project using the **Tailwind CLI** tool. This is a great option for small projects or for learning purposes.

---

## ✅ Requirements

- Node.js and npm installed
- A basic HTML project structure

---

## 📦 Step 1: Install Tailwind CSS via CLI

In your project root, open your terminal and run:

```bash
npm install -D tailwindcss
````

Then generate the Tailwind configuration file:

```bash
npx tailwindcss init
```

This will create a minimal `tailwind.config.js` file in your project.

---

## 🗂️ Step 2: Project Structure Example

Create the following file structure:

```
my-project/
├── index.html
├── input.css
├── tailwind.config.js
├── package.json
└── output.css (generated later)
```

---

## ⚙️ Step 3: Build Your CSS

Use the Tailwind CLI to compile your CSS:

```bash
npx tailwindcss -i ./input.css -o ./output.css --watch
```

* `-i`: Input file (input.css)
* `-o`: Output file (output.css)
* `--watch`: Automatically rebuild when changes are made

---

## 🧪 Step 5: Link Output CSS in HTML

In your `index.html` file, link the generated `output.css` file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Tailwind CLI Project</title>
  <link href="output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold text-blue-600">Hello Tailwind!</h1>
</body>
</html>
```

---

## 🎉 Done!

Your Tailwind CSS is now set up using the CLI tool. You can now write utility-first CSS directly in your HTML files!

---

## 📚 More Info

For advanced usage and production setup, visit the official docs:
👉 [https://tailwindcss.com/docs/installation](https://tailwindcss.com/docs/installation)

```