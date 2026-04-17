# Glam Elegance - Beauty & Cosmetics Website

A modern, responsive static website for a beauty and cosmetics brand with WhatsApp ordering integration.

## Features

- **Modern Design**: Beautiful, elegant design with smooth animations
- **Product Categories**: Lipsticks, Lotions, Makeups, Perfumes
- **WhatsApp Ordering**: Direct ordering via WhatsApp for each product
- **Responsive**: Fully responsive for all devices
- **Fast Loading**: Static HTML with no backend required

## Project Structure

```
glam/
├── index.html      # Main HTML file
├── css/
│   └── style.css # All styles
├── js/
│   └── main.js  # JavaScript functionality
├── images/       # Product images place here
└── README.md    # This file
```

## Setup

1. Open `index.html` in a web browser

## Adding Product Images

Place your product images in the `images/` folder with these names:

### Lipstick Products
- `lipstick-1.png` - Red Velvet Lipstick
- `lipstick-2.png` - Rose Petal Lipstick
- `lipstick-3.png` - Nude Classic Lipstick

### Lotion Products
- `lotion-1.png` - Rose Glow Body Lotion
- `lotion-2.png` - Shea Butter Cream
- `lotion-3.png` - Aloe Vera Gel

### Makeup Products
- `makeup-1.png` - Pro Coverage Foundation
- `makeup-2.png` - Golden Hour Eyeshadow Palette
- `makeup-3.png` - Volume Boost Mascara

### Perfume Products
- `perfume-1.png` - Elegance Signature Perfume
- `perfume-2.png` - Fresh Blossom
- `perfume-3.png` - Oriental Dream

### Other Images
- `hero-product.png` - Hero section product image
- `about.png` - About section image

## Configuring WhatsApp

1. Open `js/main.js`
2. Find this line:
   ```javascript
   const WHATSAPP_NUMBER = '1234567890';
   ```
3. Replace `'1234567890'` with your actual WhatsApp number (include country code, no + or dashes)

Example:
```javascript
const WHATSAPP_NUMBER = '256772123456'; // Uganda number
```

## Customization

### Changing Colors
Edit `css/style.css` and modify the CSS variables:
```css
:root {
    --primary: #1a1a2e;
    --accent: #e94560;
    --gold: #d4af37;
}
```

### Adding More Products
Add new product cards in the `products-grid` section of `index.html`:

```html
<div class="product-card fade-in-up" data-category="category-name">
    <div class="product-image">
        <img src="images/your-product.png" alt="Product Name">
    </div>
    <div class="product-info">
        <span class="product-category">Category</span>
        <h3>Product Name</h3>
        <p class="product-description">Description here</p>
        <div class="product-footer">
            <div class="product-price">$00.00</div>
            <button class="product-btn" onclick="orderViaWhatsApp('Product Name', '$00.00')">
                <i class="fab fa-whatsapp"></i>
                Order
            </button>
        </div>
    </div>
</div>
```

### Adding Contact Info
Update the footer section in `index.html` with your actual contact details.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## License

All rights reserved. © 2025 Glam Elegance.