#  TripPlanner AI – Your Personal Smart Travel Companion

An AI-powered Android app that intelligently plans trips based on user preferences such as destination, duration, and budget. Integrates OpenAI API for generating personalized travel itineraries and uses Google Maps SDK  to visualize optimized routes, hotel suggestions, and attractions — all within a clean, modern UI built using MVVM, Coroutines .

##  Flow Overview

###  1. Sign Up / Login  
- Users can create an account or log in securely using email/password or Google sign-in.  
- Once logged in, users are greeted with an AI chat interface ready to assist them.

###  2. Chat with TripPlanner AI  
- The AI assistant (powered by OpenAI API or Gemini) asks users for:
  - Travel destination  
  - Number of days   
  - Interests (nature, culture, nightlife, food, etc.)   
- It then generates **personalized itineraries** dynamically based on preferences and weather, optimized routes, and best local spots.

###  3. AI-Generated Itineraries  
- Beautifully designed itinerary cards displayed in a horizontal **image carousel**.  
- Each itinerary contains:
  - Cover image of the destination  
  - Brief summary  
  - “View Details” button to explore more  

###  4. Itinerary Details Screen  
- Opens when the user taps an itinerary card.  
- Displays a **day-by-day travel plan** including:
  - Attractions   
  - Restaurants   
  - Must-visit places   
  - Maps integration (Google Maps) showing route and location pins.  
- Each day is shown as a collapsible card or timeline for easy navigation.

###  5. Trip Cart (Booking Assistant)  
- After finalizing an itinerary, the user can move the trip to the **Trip Cart**.  
- The app provides direct links to booking platforms for:
  - Hotels   
  - Flights   
  - Activities   
- Opens the browser for seamless in-app booking experience.

##  Features

✅ AI-powered trip generation using LLM  
✅ Dynamic itinerary creation with images & links  
✅ Day-by-day detail screen with maps & categorized spots  
✅ Interactive chat interface with context memory  
✅ Login & Signup with Firebase Authentication  
✅ Save, update, and manage itineraries locally or via Firestore  
✅ Trip Cart integration for easy booking  
✅ Modern Android UI built with **Jetpack Compose**

##  Tech Stack

| Layer | Technology |
|-------|-------------|
| **Frontend** | Jetpack Compose, Material 3, Kotlin Coroutines, Navigation Component |
| **Architecture** | MVVM (Model-View-ViewModel), Clean Architecture |
| **Backend / AI** | OpenAI / Gemini API for AI-based itinerary generation |
| **Database** | Firebase Firestore / Room (for offline support) |
| **Authentication** | Firebase Auth (Email/Password, Google Sign-In) |
| **Networking** | Retrofit / Ktor Client |
| **Maps** | Google Maps SDK |
| **Image Loading** | Coil / Glide |
| **Dependency Injection** | Dagger Hilt |
| **Async Handling** | Kotlin Coroutines, Flow |
| **UI Animations** | Lottie, MotionLayout, Compose Animations |


##  UI Highlights

- **Login / Signup Screens:** Clean modern layout with Material3 components.  
- **Chat Screen:** AI interaction with typing animation and message bubbles.  
- **Itinerary Cards:** Carousel view with location image, title, and short summary.  
- **Itinerary Details:** Map view, attractions list, and timeline visualization.  
- **Trip Cart:** Sleek booking screen linking to external services.


##  Architecture Diagram
com.tripplanner
├── data
│   ├── model/
│   ├── repository/
│   └── remote/
├── ui
│   ├── auth/
│   │   ├── SignUpScreen.kt
│   │   ├── LoginScreen.kt
│   │   └── AuthViewModel.kt
│   ├── itinerary/
│   │   ├── ItineraryDetailScreen.kt
│   │   ├── DayPlanCard.kt
│   │   └── TripHeaderCard.kt
│   ├── chat/
│   │   ├── ChatScreen.kt
│   │   └── ChatViewModel.kt
│   └── tripcart/
│       ├── TripCartScreen.kt
│       └── TripCartViewModel.kt
└── utils/
    └── Extensions.kt

##  Example User Journey

1. **Sign Up / Login** → Secure Firebase Authentication  
2. **Chat with AI** → “Plan a 5-day trip to Paris”  
3. **AI Generates Itineraries** → Carousel with image + summary  
4. **Click a Card** → Detailed daily itinerary + Google Map  
5. **Open Trip Cart** → Redirects to hotel and activity booking sites  

##  Future Enhancements

-  Multi-destination trip planning  
-  Save trips for offline access  
-  Voice-based AI chat  
-  Budget optimizer (AI estimates total trip cost)  
-  Real-time weather suggestions  
-  Calendar integration for syncing trip dates

## Installation
Clone the repository:

1. git clone https://github.com/Trip-Planner-AI-Agent-app.git
2. Open the project in Android Studio
3. Sync Gradle and build the project
4. Run the app on an emulator or a physical device

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## Contact

For questions or feedback, contact:
Email: seethaindhiran@gmail.com
GitHub: SeethaIndiran

## Screen shots
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/14937982e53fdfd047ebdba52b8b97d5baadbd88/Screenshot%202025-11-19%20225811.png)   
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20230111.png)
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20230302.png)
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20230539.png)
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20230653.png)
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20230825.png)
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20231008.png)
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20231136.png)
 ![image_alt](https://github.com/SeethaIndiran/Trip-Planner-AI-Agent-app/blob/e0c925eb347f291a6753b18305e959a30c41fac2/Screenshot%202025-11-19%20231253.png)


