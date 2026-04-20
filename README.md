# Trivia Quiz App

## Overview

This is a Flutter quiz app that fetches questions from QuizAPI and displays them in a multiple-choice format.

The app demonstrates:

* API integration using HTTP
* JSON parsing into Dart models
* Stateful UI updates
* Basic user interaction and feedback

---

## Features

* Fetches quiz questions from QuizAPI
* Displays multiple-choice answers
* Shuffles answer options
* Tracks user score
* Shows correct/incorrect feedback
* Displays final result screen

---

## Project Structure

```
lib/
├── app_config.dart
├── main.dart
├── models/
│   └── question.dart
├── services/
│   └── trivia_service.dart
├── screens/
│   ├── quiz_screen.dart
│   └── result_screen.dart
```

---

## API

* API: https://quizapi.io
* Endpoint: /api/v1/questions
* Uses Bearer token authentication

---

## Setup

Install dependencies:

```
flutter pub get
```

Run the app:

```
flutter run --dart-define=QUIZ_API_KEY=YOUR_API_KEY
```

---

## Build APK

```
flutter build apk --release --dart-define=QUIZ_API_KEY=YOUR_API_KEY
```

---

## Testing Criteria

* App runs without crashing
* Questions load from API
* Answers can be selected
* Score updates correctly
* Result screen appears

---

## Notes

* Do not hardcode the API key
* Requires internet connection
* API rate limits may apply