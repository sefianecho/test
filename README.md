# HTML DragSort

html-dragsort is a lightweight, zero-dependency library for reordering HTML elements using Pointer Events. It supports vertical, horizontal, and grid layouts, with options for drag handles and lifecycle events (`dragStart`, `sort`, `dragEnd`).

## Getting Started

Install using package manager:
```sh
npm install html-dragsort
```
or
```sh
yard add html-dragsort
```
### CDN

- UMD
```html
  <script src="https://cdn.jsdelivr.net/npm/html-dragsort@1/dist/html-dragsort.umd.min.js"></script>
```
- IIFE
```html
  <script src="https://cdn.jsdelivr.net/npm/html-dragsort@1/dist/html-dragsort.iife.min.js"></script>
```
- ES Module
```html
<script type="module">
    import DragSort from "https://cdn.jsdelivr.net/npm/html-dragsort@1/dist/html-dragsort.esm.min.js";
</script>
```
## Usage

html-dragsort makes any container sortable by dragging its children. Just pass a parent element (or a selector) to the constructor. By default, all direct children become draggable, but you can customize which ones are draggable using options like `handle` or a `draggable` class filter.

```javascript
const sorter = new HTMLDragSort('#container', { /* ...options */ });
```
