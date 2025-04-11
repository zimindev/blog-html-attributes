### **HTML Attributes: The Complete Guide**

HTML attributes provide additional information about elements and modify their behavior. Here's everything you need to know:

---

## 📌 **Global Attributes (Work with Most Tags)**
| Attribute | Description | Example |
|-----------|-------------|---------|
| `id` | Unique identifier | `<div id="header">` |
| `class` | For CSS/JavaScript targeting | `<p class="text-red">` |
| `style` | Inline CSS styles | `<h1 style="color: blue;">` |
| `title` | Tooltip text | `<a title="Click me">` |
| `data-*` | Custom data attributes | `<div data-user-id="123">` |

---

## 🌟 **Element-Specific Attributes**

### **1. Links & Media**
```html
<a href="https://example.com" target="_blank" rel="noopener">Link</a>
<img src="image.jpg" alt="Description" width="200">
```
- `href` - Link URL
- `target` - Where to open (`_blank` for new tab)
- `src` - Resource path
- `alt` - Alternative text (required for accessibility)

### **2. Forms**
```html
<input type="text" name="username" placeholder="Enter name" required>
<button type="submit">Send</button>
```
- `type` - text/password/checkbox etc.
- `placeholder` - Hint text
- `required` - Mandatory field
- `disabled` - Disables the element

### **3. Media Elements**
```html
<video controls width="400" autoplay loop>
  <source src="movie.mp4" type="video/mp4">
</video>
```
- `controls` - Shows player controls
- `autoplay` - Auto-plays media
- `loop` - Loops playback

---

## 💡 **Special HTML5 Attributes**
| Attribute | Purpose | Example |
|-----------|---------|---------|
| `contenteditable` | Makes text editable | `<div contenteditable>...</div>` |
| `draggable` | Enables drag-and-drop | `<img draggable="true">` |
| `hidden` | Hides element | `<p hidden>Text</p>` |
| `spellcheck` | Enables spellcheck | `<textarea spellcheck="true">` |

---

## 🚀 **Best Practices**
1. **Quotes**: Always use `""` (not '' or none)
   ```html
   <img src="photo.jpg" alt="Description"> ✅
   <img src=photo.jpg alt=Description> ❌
   ```

2. **Boolean Attributes** (work without values)
   ```html
   <input disabled> <!-- Correct -->
   <input disabled="disabled"> <!-- Also correct -->
   ```

3. **Accessibility**:
   - Always include `alt` for images
   - Use `aria-*` attributes for screen readers
   ```html
   <button aria-label="Close menu">×</button>
   ```

---

## 🔥 **Practical Example**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Attributes</title>
    <style>
        .highlight { background: yellow; }
    </style>
</head>
<body>
    <article id="main-article" class="post" data-post-id="42">
        <h1 contenteditable>Edit me!</h1>
        <img src="cat.jpg" alt="Cat" width="300" title="Fluffy cat">
        <form>
            <input type="email" placeholder="Email" required>
            <button type="submit" disabled>Submit</button>
        </form>
    </article>
</body>
</html>
```

**Key Takeaways:**
- `data-post-id` - Custom attribute for JavaScript
- `contenteditable` - Makes heading editable
- `required`/`disabled` - Form control states
- `title` - Hover tooltip for image

---

## 📚 **Learning Resources**
- [MDN: HTML Attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)
- [Complete Attributes List](https://www.w3schools.com/tags/ref_attributes.asp)
- [Accessibility Attributes](https://webaim.org/techniques/aria/)

Mastering attributes will give you precise control over your HTML elements and their behavior! 🚀
