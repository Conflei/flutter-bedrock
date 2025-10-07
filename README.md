# Flutter Bedrock 🏗️

A comprehensive Flutter project template designed to serve as the foundation for all your Flutter applications. This bedrock includes essential features, modern architecture patterns, and third-party integrations that you can selectively enable based on your project needs.

## 🎯 Purpose

This project eliminates the repetitive setup work for new Flutter projects by providing a ready-to-use foundation with:

- **MVVM Architecture** - Clean separation of concerns
- **State Management** - Riverpod for reactive state management
- **Authentication** - Multiple auth providers (Apple, Google, Phone/SMS)
- **Monetization** - RevenueCat integration for subscriptions and purchases
- **Navigation** - AutoRouting for type-safe navigation
- **Example Screens** - Capability showcase and paywall examples

## 🚀 Features

### Core Architecture

- **MVVM Pattern** - Model-View-ViewModel architecture for scalable code
- **Riverpod State Management** - Modern, reactive state management
- **AutoRouting** - Type-safe navigation with code generation

### Authentication Options

- **Apple Sign-In** - Native iOS authentication
- **Google Sign-In** - Cross-platform Google authentication
- **Phone/SMS Authentication** - Phone number verification

### Monetization

- **RevenueCat Integration** - Subscription and in-app purchase management
- **Paywall Examples** - Ready-to-use subscription screens

### Development Features

- **Modular Design** - Enable only the features you need
- **Example Screens** - Capability showcase and implementation examples
- **Forkable Template** - Just change API keys and start building

## 📋 Prerequisites

- Flutter SDK (3.9.0 or higher)
- Dart SDK
- iOS development: Xcode (for Apple Sign-In)
- Android development: Android Studio
- RevenueCat account (for monetization features)
- Firebase project (for authentication)

## 🛠️ Setup Instructions

### 1. Clone and Setup

```bash
git clone <your-repo-url>
cd flutter_bedrock
flutter pub get
```

### 2. Configure Third-Party Services

#### RevenueCat Setup

1. Create a RevenueCat account at [revenuecat.com](https://www.revenuecat.com)
2. Add your API keys to the configuration files
3. Configure your products and subscriptions in RevenueCat dashboard

#### Firebase Authentication

1. Create a Firebase project at [console.firebase.google.com](https://console.firebase.google.com)
2. Enable Authentication methods (Apple, Google, Phone)
3. Download and add configuration files:
   - `google-services.json` (Android)
   - `GoogleService-Info.plist` (iOS)

#### Apple Sign-In

1. Configure Apple Sign-In in your Apple Developer account
2. Add the Sign In with Apple capability in Xcode
3. Update your app's bundle identifier

#### Google Sign-In

1. Configure OAuth 2.0 credentials in Google Cloud Console
2. Add your SHA-1 fingerprint for Android
3. Configure iOS URL schemes

### 3. Enable Features

The project is designed to be modular. You can enable/disable features by:

- Commenting/uncommenting dependencies in `pubspec.yaml`
- Removing unused service configurations
- Customizing the feature flags in your app configuration

## 📱 Example Screens

### Capability Showcase

A demonstration screen showing all integrated features:

- Authentication methods
- State management examples
- Navigation patterns
- UI components

### RevenueCat Paywall

A complete subscription paywall implementation:

- Product display
- Purchase flow
- Subscription management
- Restore purchases

## 🏗️ Project Structure

```
lib/
├── core/                 # Core utilities and base classes
├── features/            # Feature-based modules
│   ├── auth/           # Authentication feature
│   ├── monetization/   # RevenueCat integration
│   └── showcase/       # Example screens
├── shared/             # Shared components and utilities
├── main.dart          # App entry point
└── app.dart           # App configuration
```

## 🔧 Customization

### Adding New Features

1. Create a new feature module in `lib/features/`
2. Follow the MVVM pattern with separate folders for models, views, and viewmodels
3. Add necessary dependencies to `pubspec.yaml`
4. Update the main app configuration

### Removing Unused Features

1. Remove dependencies from `pubspec.yaml`
2. Delete unused feature folders
3. Remove service configurations
4. Update app initialization code

## 📚 Dependencies

### Core Dependencies

- `flutter_riverpod` - State management
- `auto_route` - Navigation
- `revenuecat_purchases_flutter` - Monetization
- `firebase_auth` - Authentication
- `google_sign_in` - Google authentication
- `sign_in_with_apple` - Apple authentication

### Development Dependencies

- `flutter_lints` - Code quality
- `build_runner` - Code generation
- `auto_route_generator` - Route generation

## 🤝 Contributing

This is a personal bedrock project, but suggestions and improvements are welcome! Feel free to:

- Fork the project
- Create feature branches
- Submit pull requests
- Open issues for bugs or feature requests

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🔗 Resources

- [Flutter Documentation](https://docs.flutter.dev/)
- [Riverpod Documentation](https://riverpod.dev/)
- [RevenueCat Documentation](https://docs.revenuecat.com/)
- [AutoRoute Documentation](https://autoroute.vercel.app/)
- [Firebase Documentation](https://firebase.google.com/docs)

---

**Happy Coding! 🚀**

_This bedrock is designed to save you time and provide a solid foundation for your Flutter projects. Customize it to fit your needs and build amazing apps!_
