# 🛒 Shopify Custom Product Gallery & Accordion (Dawn Extension)

This project extends the standard **Shopify Dawn theme** by adding:

- A **custom Swiper-powered product gallery** with support for responsive settings and media filtering by variant.
- A **dynamic accordion** built using **product metafields**, allowing easy content control from the Shopify Admin.

It demonstrates how to enhance the default product page with flexible, reusable UI components that can be configured per product without code changes.

## 📌 Key Features

### ✅ 1. Custom Product Gallery (Swiper.js)
- Replaces the default Shopify media gallery.
- Built with [Swiper.js](https://swiperjs.com/).
- Fully responsive with dynamic settings configured via schema.
- Supports:
  - Adjustable number of slides by screen size.
  - Custom spacing, arrows, and pagination.
  - Filtering product media by selected variant (e.g., color).
  - Optimized for performance and accessibility.

### ✅ 2. Dynamic Accordion via Product Metafields
- Accordion items are fully managed via product metafields:
  - `custom.accordion_titles` — List of titles (Single-line text).
  - `custom.accordion_contents` — List of content blocks (Single-line text).
  - `custom.accordion_multiple_open` — Boolean to allow multiple items open at once.
- Accordion renders only if valid data is provided.
- A placeholder is displayed in Theme Editor if metafields are empty.

### 🧩 Technologies Used
- Shopify Liquid
- Vanilla JavaScript
- Swiper.js
- Product Metafields
- Theme Editor schema settings
- Base: **Shopify Dawn theme**

## 📂 File Structure

- `/sections/main-product.liquid` – Main product section with gallery and accordion logic.
- `/snippets/product-media-gallery.liquid` – Custom Swiper gallery.
- `/snippets/accordion.liquid` – Accordion component powered by metafields.
