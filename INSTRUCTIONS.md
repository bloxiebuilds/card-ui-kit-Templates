# 📖 card-ui-kit-Templates — Instructions

A quick guide to using, customizing, and dropping these cards into your own projects.

---

## 📋 Table of Contents

1. [How to Use a Card](#1-how-to-use-a-card)
2. [Changing Colors](#2-changing-colors)
3. [Changing Text & Content](#3-changing-text--content)
4. [Dark Mode](#4-dark-mode)
5. [Card-Specific Tips](#5-card-specific-tips)
6. [FAQ](#6-faq)

---

## 1. How to Use a Card

1. Open any `.html` file in the `/cards` folder in your browser to preview it
2. Open the same file in a text editor (Notepad, VS Code, etc.)
3. Copy the HTML structure you want (inside `<body>`)
4. Copy the CSS styles you want (inside `<style>`)
5. Paste both into your own project

---

## 2. Changing Colors

Each card uses a simple accent color. Find this near the top of each file:

```css
--accent: #38BDF8;
```

Replace `#38BDF8` with any hex color. Some ideas:

| Color | Hex |
|-------|-----|
| Sky blue (default) | `#38BDF8` |
| Soft purple | `#A78BFA` |
| Warm orange | `#FB923C` |
| Hot pink | `#F472B6` |
| Mint green | `#6EE7B7` |

---

## 3. Changing Text & Content

All text content is written directly in the HTML. Just find and replace:

- Names, roles, bios → edit the text inside `<p>` tags
- Prices → edit the number inside `.price`
- Feature lists → add or remove `<li>` items
- Links → update the `href="..."` values

---

## 4. Dark Mode

To add dark mode to any card, add this CSS and a toggle button:

```css
[data-theme="dark"] {
  background: #0f0f0f;
  --card-bg: #1a1a1a;
  --border: #2a2a2a;
  --text: #f0f0f0;
  --muted: #888;
}
```

Then add `data-theme="dark"` to your `<body>` tag, or toggle it with JavaScript:

```js
document.body.setAttribute('data-theme', 'dark');
```

---

## 5. Card-Specific Tips

### Profile Card
- Set `avatar` to an image URL to replace the initials
- Add or remove `.pill` links as needed

### Stat Card
- Change `.up` color for positive trends, `.down` for negative
- Works great in a 2 or 3 column grid

### Pricing Card
- The `.featured` class adds the highlighted border
- Move it to whichever plan you want to highlight

### Notification Card
- `.unread` adds the left blue border
- Remove it from read notifications

### Product Card
- Replace the `.img-wrap` placeholder with a real `<img>` tag
- Change the `.tag` text and color class for sale/new/featured

### Link Card
- Change `.tag` class to `tutorial`, `guide`, or `news` for different colors
- Works great as a blog post preview grid

---

## 6. FAQ

**Q: Do I need to know how to code?**
Basic HTML and CSS knowledge helps, but most changes are just swapping out text and colors.

**Q: Can I use these in a commercial project?**
Yes — MIT licensed. Free to use and modify. Reselling the kit itself is not permitted.

**Q: Can I combine multiple cards on one page?**
Absolutely! Just copy multiple card blocks and their styles into a single HTML file.

**Q: Can I add animations?**
Yes! All cards have hover transitions built in. Add more with CSS `transition` or `animation`.

---

<p align="center">card-ui-kit-Templates was made by <a href="https://github.com/bloxiebuilds">bloxiebuilds</a></p>
