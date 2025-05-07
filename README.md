# E-Commerce Website with Stripe Payment Integration

## Developed by Phạm Lê Ngọc Sơn

This is a modern e-commerce application built with Next.js, featuring seamless payment processing through Stripe and content management using Sanity CMS.

## Project Overview

This full-stack e-commerce platform provides a complete shopping experience from product browsing to checkout with real-time payment processing. The application features a responsive design, shopping cart functionality, and integrated content management system.

## Features

- **Modern UI/UX**: Responsive design that works across all devices
- **Product Catalog**: Browse and search through available products
- **Shopping Cart**: Add, remove, and adjust quantities of products
- **Secure Checkout**: Integrated with Stripe for secure payment processing
- **Content Management**: Sanity CMS for easy content updates
- **Order Confirmation**: Success page with order details and confetti animation

## Tech Stack

- **Frontend**: Next.js, React.js, CSS
- **Payment Processing**: Stripe
- **Content Management**: Sanity CMS
- **State Management**: React Context API
- **UI Enhancements**: 
  - react-hot-toast for notifications
  - canvas-confetti for celebration effects
  - react-icons for UI icons

## Project Structure

```
/
├── components/            # Reusable UI components
│   ├── Cart.jsx           # Shopping cart implementation
│   ├── Footer.jsx         # Site footer
│   ├── FooterBanner.jsx   # Promotional banner in footer
│   ├── HeroBanner.jsx     # Hero section banner
│   ├── Layout.jsx         # App layout wrapper
│   ├── Navbar.jsx         # Navigation bar
│   └── Product.jsx        # Product card component
│
├── context/               # State management with Context API
│
├── lib/                   # Utility functions and client setup
│   └── client.js          # Sanity client configuration
│
├── pages/                 # Application routes
│   ├── api/               # API endpoints
│   │   └── stripe.js      # Stripe payment integration
│   ├── product/           # Product detail pages
│   ├── _app.js            # Next.js app component
│   ├── index.js           # Homepage
│   └── success.js         # Order confirmation page
│
├── public/                # Static assets
│
├── sanity_ecommerce/      # Sanity CMS configuration
│   └── schemas/           # Content models for the CMS
│
└── styles/                # CSS styles
```

## Getting Started

### Prerequisites

- Node.js (v12 or higher)
- npm or yarn
- Sanity account
- Stripe account

### Installation

1. Clone the repository
   ```
   git clone https://github.com/ngocson-pham/ecommerce-stripe.git
   cd ecommerce-stripe
   ```

2. Install frontend dependencies
   ```
   npm install
   # or
   yarn install
   ```

3. Install Sanity dependencies
   ```
   cd sanity_ecommerce
   npm install
   # or
   yarn install
   cd ..
   ```

4. Set up environment variables
   Create a `.env.local` file in the root directory with:
   ```
   NEXT_PUBLIC_SANITY_TOKEN=your_sanity_token
   NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
   STRIPE_SECRET_KEY=your_stripe_secret_key
   ```

5. Start the development server
   ```
   npm run dev
   # or
   yarn dev
   ```
   
6. Run the Sanity studio (in a separate terminal)
   ```
   cd sanity_ecommerce
   npm run start
   # or
   yarn start
   ```

## Deployment

The application can be deployed to Vercel with the following steps:

1. Push your code to a GitHub repository
2. Connect your repository to Vercel
3. Configure the environment variables in Vercel dashboard
4. Deploy

## License

This project is licensed under the MIT License. 
