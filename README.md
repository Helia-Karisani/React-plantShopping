

# Paradise Nursery Shopping Cart

This is a **React + Redux** application for an online plant shop called *Paradise Nursery*. It allows users to browse a variety of houseplants, add them to a shopping cart, and manage their order before checkout.

## Live Demo

**[Click to view the deployed site](https://helia-karisani.github.io/React-plantShopping/)**



---

## Features

* **Landing Page** with a navigation bar and “Get Started” button
* **Product Listing Page** that displays:

  * Plant name, image, cost, description
  * “Add to Cart” button (disabled after adding)
  * Categorized sections (e.g., Aromatic and Medicinal Plants)
* **Cart Page** that supports:

  * Display of selected items
  * Per-item subtotal (quantity × unit cost)
  * Overall total cart amount
  * Increment / decrement quantity buttons
  * Delete item button
  * “Continue Shopping” button
  * “Checkout” button (currently shows alert)

---

## Technologies Used

* React (functional components)
* React Redux Toolkit
* JavaScript
* CSS

---

## Project Structure

```
src/
│
├── components/
│   ├── ProductList.jsx        // Displays all plants
│   └── CartItem.jsx           // Manages the cart display & functionality
│
├── redux/
│   └── CartSlice.jsx          // Redux slice with add/remove/updateQuantity reducers
│
├── store.js                   // Configures Redux store
├── App.jsx                    // App router and page logic
├── main.jsx                   // Redux Provider setup
└── index.css, *.css           // Styling
```

---

## Getting Started Locally

1. Clone your forked repo:

   ```bash
   git clone https://github.com/Helia-Karisani/your-repo-name.git
   cd your-repo-name
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Run the app:

   ```bash
   npm run dev
   ```

4. Open your browser to `http://localhost:5173/`

---

## Deployment Instructions

To deploy to GitHub Pages:

1. Install:

   ```bash
   npm install gh-pages --save-dev
   ```

2. In `package.json`, add:

   ```json
   "homepage": "https://helia-karisani.github.io/your-repo-name",
   "scripts": {
     "predeploy": "npm run build",
     "deploy": "gh-pages -d dist"
   }
   ```

3. In `vite.config.js`, add:

   ```js
   base: "/your-repo-name/",
   ```

4. Then deploy:

   ```bash
   npm run deploy
   ```

---

## What I Learned

* How to use Redux Toolkit for state management
* Handling dynamic rendering with `map()`
* Component interaction through props and event handlers
* Parsing and computing values like subtotal and total cost
* Proper deployment using GitHub Pages

---

## Author

**Helia Karisani**
[GitHub Profile](https://github.com/Helia-Karisani)



