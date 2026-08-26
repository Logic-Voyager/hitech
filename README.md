# HiTech Interials

A responsive fashion ecommerce storefront built with HTML, CSS, and vanilla JavaScript. HiTech Interials focuses on clean everyday fashion, simple navigation, and a teal-led visual identity across desktop and mobile screens.

> Project status: front-end portfolio demo. The site is deployed and suitable for showcasing the interface, but it is not connected to a production backend or payment service.

## Live Website

The website is deployed with Netlify from this GitHub repository.

- Live site: https://hitechinterials.netlify.app/
- Repository: https://github.com/Logic-Voyager/hitech

## Features

- Responsive home, shop, blog, about, contact, cart, checkout, and product pages
- Mobile navigation with a slide-out menu
- Product cards that open individual product detail pages
- Shop pagination with page controls
- Responsive product grid for phone, tablet, and desktop screens
- Shopping cart layout with quantity controls and item removal
- Coupon-code feedback using the demo code `WELCOME10`
- Checkout form with order summary and secure-payment messaging
- Order confirmation screen with a generated order number
- Contact form with a client-side success message
- Shared brand navigation, newsletter section, footer, and visual styling
- Fashion editorial imagery with descriptive alternative text on primary images

## Pages

| Page | File | Purpose |
| --- | --- | --- |
| Home | `index.html` | Store introduction, featured products, promotions, and new arrivals |
| Shop | `shop.html` | Product catalog with pagination and product navigation |
| Product details | `sproduct.html`, `s1product.html` - `s6product.html` | Individual product views |
| Blog | `blog.html` | Style advice, wardrobe ideas, and clothing-care articles |
| About | `about.html` | Brand story, values, and store approach |
| Contact | `contact.html` | Store information and contact form |
| Cart | `cart.html` | Cart items, quantities, totals, and coupon field |
| Checkout | `payment.html` | Payment form, order summary, and confirmation state |

## Project Structure

```text
.
├── index.html
├── shop.html
├── about.html
├── blog.html
├── contact.html
├── cart.html
├── payment.html
├── sproduct.html
├── s1product.html
├── s2product.html
├── s3product.html
├── s4product.html
├── s5product.html
├── s6product.html
├── style.css
├── payment.css
├── script.js
└── img/
    ├── logo.png
    ├── play.png
    ├── shop.jpeg
    └── backGround.png
```

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Font Awesome 4.7
- Google Fonts: Spartan
- Unsplash and other remote image sources
- GitHub for source control
- Netlify for hosting and continuous deployment

## Run Locally

No build step or package installation is required.

### Option 1: Open directly

Open `index.html` in a browser.

### Option 2: Use a local server

A local server gives more reliable results for links and browser features. For example, with Python installed:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deploy With Netlify

1. Push the project to GitHub.
2. Sign in to Netlify.
3. Select **Add new site** and choose **Import an existing project**.
4. Connect the GitHub repository.
5. Use the following settings:
   - Build command: leave empty
   - Publish directory: `.`
6. Deploy the site.
7. Every future push to the selected branch will trigger a new deployment.

If Netlify does not publish the root correctly, set the publish directory to the repository root and confirm that `index.html` is at the top level. No framework preset or environment variables are required.

## Important Notes

This is a front-end demonstration project. The payment form does not process real payments, and the contact form does not send data to a server. Do not enter real card details.

Product images currently use remote URLs, so an internet connection may be required for every image to display. For production use, download approved product images into `img/` and update the page paths.

The cart and checkout are currently client-side demo features. Cart and checkout data are not a substitute for a production order system. A production store would need a backend, database, authentication, inventory management, payment provider, order persistence, and server-side validation.

## Customization

- Update colors and shared layouts in `style.css`.
- Update checkout-specific styling in `payment.css`.
- Update mobile-menu behavior in `script.js`.
- Replace product text, prices, images, and links in the product pages.
- Replace placeholder contact details in the footer and contact page.
- Replace the Netlify and GitHub URLs near the top of this README.

## Future Improvements

- Connect products to one shared data source
- Persist cart items consistently across product, shop, cart, and checkout pages
- Add search, filters, sorting, and wishlist support
- Add a real payment gateway such as Stripe or Razorpay
- Add server-backed contact submissions and order management
- Add product reviews, size guides, delivery estimates, and return information
- Add optimized local images and Open Graph metadata for sharing

## License

No license file is currently included. This project is intended for educational and portfolio use. Add a project-specific license before distributing or reusing the code publicly.
