# 🌤️ Weather App - Android Kotlin University Project

## 📱 Overview

The **Weather App** is an Android application developed in **Kotlin** using **Jetpack Compose** as the UI toolkit. The purpose of the app is to allow users to easily view the current weather of selected cities and current location via a clean and responsive user interface.

The application fetches real-time weather data from an external API, for the current location, for saved locations or when the user searches a city, demonstrating API integration, asynchronous programming, and clean architectural practices. It serves as a learning tool to explore Android development, user interface design, API consumption, and software architecture following best practices.

---

## 🎯 Core Features

- **🌡️ Real-Time Weather Display**  
  Retrieves and shows the weather in the current location or selected cities by making HTTP requests to an online weather API.

- **🏙️ City Selection via Search**  
  Users can search for a city and save it in a list built with Jetpack Compose.

- **🔀 Multi-Screen Navigation**  
  The app consists of two screens: a search screen and a weather display screen. Navigation is handled using Jetpack Navigation.

---

## 🛠️ Technology Stack

| Component          | Technology/Library               |
|--------------------|----------------------------------|
| Language           | Kotlin                           |
| UI Toolkit         | Jetpack Compose                  |
| Navigation         | Jetpack Navigation               |
| API Integration    | Retrofit                         |

---

## 🧭 App Navigation Flow

1. **Current Location Weather Screen**
   The application starts on the screen that displays the weather for the current location. From here, the user can navigate to the city search screen. 

2. **City search screen**  
   The user can search for a city to see the current weather there, and save the city in a list in order to have easy access to information about weather in that location.

---

## 🚀 Setup Instructions

To run this project locally, follow the steps below:

1. **Clone the Repository**

2. **Open the project in Android Studio**

3. **Add your API key:**
   Sign up at OpenWeatherMap to get an API key and insert this key into the appropriate field (in Core->Utils->Constants).

4. **Build and Run the Project on an Android device.**

---

## 🌐 API Integration

This app uses the **OpenWeatherMap API** to fetch real-time weather data. The API allows querying current temperature, humidity, and other weather details using city names. The integration is handled via the **Retrofit** HTTP client for Android.

---

## 📐 Architecture

This project follows the **MVVM (Model-View-ViewModel)** architecture pattern, which separates responsibilities across three main layers to improve code maintainability, testability, and scalability:

- **Model**  
  Responsible for managing data and business logic. This includes data classes (e.g., weather response models), Retrofit API interfaces, and the Repository layer that abstracts API access.

- **ViewModel**  
  Serves as a bridge between the UI and the Model. It holds UI-related state and handles logic such as API requests and data transformation.

- **View (UI)**  
  Built with **Jetpack Compose**, it displays state provided by the ViewModel.

---

## 🧑‍💻 Author

- **Name:** Mihaita-Catalin Pavel