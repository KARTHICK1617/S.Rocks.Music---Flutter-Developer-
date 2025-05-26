S.Rocks.Music - Flutter Developer Assignment

Mini Project: Music Services Module (Single Screen)

This project replicates the "Home Screen" UI from the provided Figma design and integrates with Firebase Firestore to dynamically display a list of music services.


---

Features

✅ UI Implementation

Fully responsive and clean layout

Styled to match the original Figma design

Includes a search bar, demo banner, and a list of service cards

Bottom navigation bar (as per design)


✅ Dynamic Data Loading (Firebase Firestore)

Firestore integration to fetch music services (title, description, icon)

No hardcoded service data

Uses Firestore collection named services


✅ Navigation

Tapping on a service card navigates to a simple detail screen showing:

You tapped on: <Service Name>


✅ MVVM Architecture

Model: ServiceModel

ViewModel: ServiceViewModel (with Provider)

Repository: ServiceRepository

Views: HomeScreen, ServiceDetailScreen


✅ State Management

Uses Provider for managing service list state and loading states

lib/
├── models/
│   └── service_model.dart
├── repositories/
│   └── service_repository.dart
├── viewmodels/
│   └── service_viewmodel.dart
├── views/
│   ├── home_screen.dart
│   └── service_detail_screen.dart
└── main.dart
