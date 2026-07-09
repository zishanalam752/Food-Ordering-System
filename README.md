# 🍔 Food Ordering System

A modern, cross-platform food ordering mobile application built with React Native and Expo. Users can browse menus, search for food items, filter by categories, add items to cart, and manage their orders seamlessly.

## ✨ Features

- 🔐 **User Authentication** - Sign up and sign in with secure authentication
- 🍽️ **Menu Browsing** - Browse food categories and items with images
- 🔍 **Advanced Search** - Search for food items with real-time filtering
- 🏷️ **Category Filtering** - Filter food items by categories
- 🛒 **Shopping Cart** - Add/remove items, manage quantities, view total price
- 👤 **User Profile** - View and manage user profile information
- 💾 **Data Persistence** - State management with Zustand for seamless experiences
- 📱 **Cross-Platform** - Works on iOS, Android, and Web

## 🛠️ Tech Stack

### Frontend
- **React Native** - Cross-platform mobile development
- **Expo** - Managed React Native framework with easy deployment
- **Expo Router** - File-based routing for navigation
- **NativeWind** - Tailwind CSS for React Native styling
- **React Navigation** - Tab-based and stack navigation

### State Management & Storage
- **Zustand** - Lightweight state management for auth and cart
- **Appwrite** - Backend-as-a-service for authentication and data storage

### UI Components & Utilities
- **Expo Vector Icons** - Comprehensive icon library
- **React Native Safe Area Context** - Handle device safe areas
- **Expo Image** - Advanced image handling
- **Use Debounce** - Debounce utility for search

## 📁 Project Structure

```
food_ordering/
├── app/                          # App screens and routing
│   ├── (auth)/                  # Auth stack (sign-in, sign-up)
│   │   ├── sign-in.tsx
│   │   ├── sign-up.tsx
│   │   └── _layout.tsx
│   ├── (tabs)/                  # Tab navigation
│   │   ├── index.tsx           # Home/Browse
│   │   ├── search.tsx          # Search screen
│   │   ├── cart.tsx            # Shopping cart
│   │   ├── profile.tsx         # User profile
│   │   └── _layout.tsx
│   ├── _layout.tsx             # Root layout
│   └── globals.css             # Global styles
├── components/                   # Reusable components
│   ├── CartButton.tsx
│   ├── CartItem.tsx
│   ├── CustomButton.tsx
│   ├── CustomHeader.tsx
│   ├── CustomInput.tsx
│   ├── Filter.tsx
│   ├── MenuCard.tsx
│   └── SearchBar.tsx
├── constants/                    # App constants
│   └── index.ts
├── lib/                         # Utilities & API
│   ├── appwrite.ts            # Appwrite integration
│   ├── data.ts                # Data utilities
│   ├── useAppwrite.ts         # Custom hook for Appwrite
│   └── seed.ts                # Database seeding
├── store/                       # Zustand stores
│   ├── auth.store.ts          # Authentication state
│   └── cart.store.ts          # Shopping cart state
├── assets/                      # Images, fonts, icons
│   ├── fonts/
│   ├── icons/
│   ├── images/
│   └── readme/
└── package.json

```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Expo CLI (`npm install -g expo-cli`)
- Appwrite account and project set up

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/zishanalam752/Food-Ordering-System.git
   cd food_ordering
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Appwrite**
   - Create a `.env` file in the root directory
   - Add your Appwrite credentials:
     ```env
     EXPO_PUBLIC_APPWRITE_ENDPOINT=your_appwrite_endpoint
     EXPO_PUBLIC_APPWRITE_PROJECT_ID=your_project_id
     ```

4. **Start the development server**
   ```bash
   npm start
   ```

### Running on Different Platforms

**iOS**
```bash
npm run ios
```

**Android**
```bash
npm run android
```

**Web**
```bash
npm run web
```

## 🎯 Usage

1. **Sign Up** - Create a new account with email and password
2. **Browse** - Explore available food items and categories from the home tab
3. **Search** - Use the search tab to find specific food items
4. **Filter** - Filter items by categories to narrow down choices
5. **Add to Cart** - Tap items to add them to your shopping cart
6. **Adjust Quantities** - Increase or decrease item quantities in the cart
7. **Checkout** - Review cart and proceed with order (feature can be extended)
8. **Profile** - View and update user information

## 🔧 Key Components

### Authentication Store (`store/auth.store.ts`)
Manages user authentication state including login, logout, and user session.

### Cart Store (`store/cart.store.ts`)
Handles shopping cart operations - adding/removing items, calculating totals, persisting cart state.

### Appwrite Integration (`lib/appwrite.ts`)
Manages all backend API calls and database operations with Appwrite.

### Custom Hook (`lib/useAppwrite.ts`)
React hook for fetching data from Appwrite with loading and error states.

## 📝 Scripts

- `npm start` - Start Expo development server
- `npm run ios` - Run on iOS simulator
- `npm run android` - Run on Android emulator
- `npm run web` - Run on web browser
- `npm run lint` - Run ESLint to check code quality
- `npm run reset-project` - Reset project to initial state

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for bugs and feature requests.

## 📄 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Zishan Alam**

- GitHub: [@zishanalam752](https://github.com/zishanalam752)
- Repository: [Food-Ordering-System](https://github.com/zishanalam752/Food-Ordering-System)

---

**Happy Ordering! 🍕🍟🌮**