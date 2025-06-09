# 🚗 Porsche 911 Showcase

A visually engaging and responsive webpage showcasing the **Black Porsche 911**, featuring a modern **CSS Grid-based Masonry Layout** to emphasize performance, design, and luxury.

---
## 📸 Preview
![image](https://github.com/user-attachments/assets/9c154299-ae36-4b94-8b1b-a1fd7212613b)

---
## 🔑 Key Features

- 🧱 **CSS Grid Masonry-style Layout** for dynamic content arrangement
- 🎯 Responsive Design using media queries
- 🖼️ Beautiful imagery with minimalistic styling
- 🧭 Navigation bar with brand-centered design
- 🧩 Modular layout with clear section divisions
- 💻 Accessible and clean HTML5 + CSS3 markup

---

## 🛠️ Project Stack

| Layer        | Technology |
|--------------|------------|
| Markup       | HTML5      |
| Styling      | CSS3       |
| Fonts        | Google Fonts (Poppins) |

---

## 📐 Layout Overview

The site layout is powered by **CSS Grid**, and mimics a **Masonry-style layout**. Each `<div>` in the `main` section is assigned either a `short` or `tall` class, allowing it to span 1 or 2 rows respectively.

### CSS Grid Structure

```css
main {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-auto-rows: 250px;
  gap: 30px;
}
```
---
## 📱 Responsive Design Breakpoints
This project uses CSS media queries to ensure a smooth experience across all devices. The layout dynamically changes based on screen size:

| Screen Width | Columns           |
| ------------ | ----------------- |
| `> 960px`    | 3 Columns         |
| `≤ 960px`    | 2 Columns         |
| `≤ 650px`    | 1 Column (Mobile) |

## 🖥️ Desktop (≥ 961px)
- Grid Columns: 3
- Layout: Full-width experience with a 3-column masonry grid.
- CSS:
```css
    main {
      grid-template-columns: 1fr 1fr 1fr;
    }
```
## 📱 Tablet (651px – 960px)

- Grid Columns: 2
- Layout: Condensed view with two columns for improved readability on tablets.
- CSS:
```css
@media screen and (max-width: 960px) {
  main {
    grid-template-columns: 1fr 1fr;
  }
}
```

## 📱 Mobile (≤ 650px)

- Grid Columns: 1
- Layout: Stacked view for single-column scrolling.
- Visual: Cards now span the full width with vertical scrolling.
- CSS:

@media screen and (max-width: 650px) {
 ```css main {
    grid-template-columns: 1fr;
    max-width: 400px;
    margin: 20px auto;
  }
}
```
## Mobile Design Goals
- ✅ No horizontal scrolling
- ✅ Adequate padding and spacing
- ✅ Full-width readable text blocks
- ✅ Proper image scaling with min-width: 100% and height: 100%






