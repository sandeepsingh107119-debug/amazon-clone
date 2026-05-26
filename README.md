# 🛒 Amazon Clone

A modern, full-featured e-commerce platform built with Next.js that replicates the core functionality of Amazon's shopping experience.

## 🌟 Features

### 🛍️ Shopping Experience
- **Product Catalog**: Browse and search through a comprehensive product catalog
- **Product Details**: Detailed product pages with images, descriptions, and pricing
- **Shopping Cart**: Add, remove, and manage items in your cart
- **Favorites/Wishlist**: Save products to your favorites list for later
- **Responsive Design**: Seamless experience across desktop and mobile devices

### 🔐 User Authentication
- **NextAuth Integration**: Secure authentication system
- **User Sessions**: Persistent login sessions
- **Protected Routes**: Secure access to user-specific features

### 💳 Payment Processing
- **Stripe Integration**: Secure payment processing
- **Checkout Flow**: Complete checkout experience
- **Payment Success**: Order confirmation and success pages

### 🎨 User Interface
- **Modern Design**: Clean and intuitive Amazon-inspired interface
- **Interactive Components**: Responsive carousel, search functionality
- **Loading States**: Smooth loading indicators with React Spinners
- **Icon Library**: Rich icon set with React Icons

## 🚀 Tech Stack

### Frontend
- **Framework**: [Next.js 13](https://nextjs.org/) - React framework with SSR/SSG
- **Language**: [TypeScript](https://www.typescriptlang.org/) - Type-safe JavaScript
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- **State Management**: [Redux Toolkit](https://redux-toolkit.js.org/) - Modern Redux
- **Persistence**: [Redux Persist](https://github.com/rt2zz/redux-persist) - State persistence

### Authentication & Payments
- **Auth**: [NextAuth.js](https://next-auth.js.org/) - Authentication library
- **Payments**: [Stripe](https://stripe.com/) - Payment processing platform

### UI Components & Libraries
- **Icons**: [React Icons](https://react-icons.github.io/react-icons/)
- **Carousel**: [React Responsive Carousel](https://github.com/leandrowd/react-responsive-carousel)
- **Loading**: [React Spinners](https://www.davidhu.io/react-spinners/)

## 📦 Installation

### Prerequisites
- Node.js 18+ 
- npm or yarn
- Stripe account (for payment processing)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/amazon-clone.git
   cd amazon-clone
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Environment Configuration**
   Create a `.env.local` file in the root directory:
   ```env
   # NextAuth Configuration
   NEXTAUTH_URL=http://localhost:3000
   NEXTAUTH_SECRET=your-nextauth-secret

   # Stripe Configuration
   STRIPE_PUBLIC_KEY=your-stripe-public-key
   STRIPE_SECRET_KEY=your-stripe-secret-key
   STRIPE_WEBHOOK_SECRET=your-stripe-webhook-secret

   # Database (if applicable)
   DATABASE_URL=your-database-url
   ```

4. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🛠️ Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## 📁 Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── header/         # Header-related components
│   ├── Banner.tsx      # Homepage banner
│   ├── Products.tsx    # Product listing
│   ├── CartProduct.tsx # Cart item component
│   └── ...
├── pages/              # Next.js pages
│   ├── api/           # API routes
│   ├── index.tsx      # Homepage
│   ├── cart.tsx       # Shopping cart
│   ├── favorite.tsx   # Favorites/Wishlist
│   └── ...
├── store/             # Redux store configuration
├── styles/            # Global styles
└── images/            # Static images
```

## 🎯 Usage

### Shopping Flow
1. **Browse Products**: View the product catalog on the homepage
2. **Search**: Use the search functionality to find specific products
3. **Product Details**: Click on products to view detailed information
4. **Add to Cart**: Add desired items to your shopping cart
5. **Favorites**: Save items to your favorites for later
6. **Checkout**: Complete your purchase using Stripe

### State Management
The app uses Redux Toolkit for state management with persistence:
- **Cart State**: Shopping cart items and quantities
- **Favorites**: Saved products
- **User Session**: Authentication state

## 🌐 Deployment

### Vercel (Recommended)
1. Connect your repository to [Vercel](https://vercel.com)
2. Configure environment variables in Vercel dashboard
3. Deploy automatically on every push

### Manual Deployment
```bash
npm run build
npm run start
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by Amazon's user interface and functionality
- Built with modern web development best practices
- Leverages the power of the Next.js ecosystem

## 📞 Support

If you have any questions or run into issues, please:
- Check the [Issues](https://github.com/yourusername/amazon-clone/issues) page
- Create a new issue if needed
- Reach out to the maintainers

---

**Note**: This is a educational project created for learning purposes. It is not affiliated with Amazon in any way. 