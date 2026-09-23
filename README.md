# Paradise Nursery Shopping Cart

A **React + Redux** application for an online plant shop called *Paradise Nursery*. Users can browse houseplants, add them to a shopping cart, and manage their order before checkout.

## Live Demo

[helia-karisani.github.io/React-plantShopping](https://helia-karisani.github.io/React-plantShopping/)

---

## Features

* **Landing page** with a navigation bar and “Get Started” button
* **Product listing page** that shows:
  * Plant name, image, cost, description
  * “Add to Cart” button (disabled after adding)
  * Categorized sections (e.g., Aromatic and Medicinal Plants)
* **Cart page** that supports:
  * Display of selected items
  * Per-item subtotal (quantity × unit cost)
  * Overall total cart amount
  * Increment / decrement quantity buttons
  * Delete item button
  * “Continue Shopping” button
  * “Checkout” button (currently shows an alert)

---

## Technologies Used

* React (functional components)
* Redux Toolkit
* JavaScript
* CSS

---

## Project Structure

```
src/
│
├── components/
│   ├── ProductList.jsx        // Displays all plants
│   └── CartItem.jsx           // Cart display and functionality
│
├── redux/
│   └── CartSlice.jsx          // Redux slice with add/remove/updateQuantity reducers
│
├── store.js                   // Redux store
├── App.jsx                    // App router and page logic
├── main.jsx                   // Redux Provider setup
└── index.css, *.css           // Styling
```

---

## Running Locally

1. Clone the repo:

   ```bash
   git clone https://github.com/Helia-Karisani/React-plantShopping.git
   cd React-plantShopping
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Run the app:

   ```bash
   npm run dev
   ```

4. Open `http://localhost:5173/`

---

## Deployment

The site is deployed to GitHub Pages with `gh-pages`:

`package.json`:

```json
"homepage": "https://helia-karisani.github.io/React-plantShopping",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d dist"
}
```

`vite.config.js`:

```js
base: "/React-plantShopping/",
```

Deploy with:

```bash
npm run deploy
```

---

## What I Learned

* Using Redux Toolkit for state management
* Dynamic rendering with `map()`
* Component interaction through props and event handlers
* Computing subtotal and total cost
* Deploying with GitHub Pages
