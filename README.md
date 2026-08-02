# 📝 Notes App

Notes App is a lightweight, clean, and intuitive Android application built to help users seamlessly organize their thoughts, draft daily tasks, and manage personal logs. Featuring a distraction-free user interface, the app makes capturing ideas fast, responsive, and reliable.

---

### 🚀 Features

* 📝 **Quick Note Creation** — Draft and save thoughts instantly.
* 🔍 **Search Functionality** — Easily locate specific notes by keyword.
* 🔄 **Auto-Save System** — Never lose progress while typing.
* 🗑️ **Trash Management** — Safely restore accidentally deleted notes.
* 🎨 **Custom Themes & Colors** — Personalize individual notes with custom color palettes and canvas layouts.
* 🔒 **Data Privacy** — Local storage ensures information stays entirely offline.

---

### 🏗️ Project Architecture

This project follows **Clean Architecture** patterns to ensure clean separation of concerns, high testability, and scalability:

* **Presentation Layer (UI)** — Handles ViewModels, Views, and UI rendering logic.
* **Domain Layer** — Contains pure business logic, UseCases, and core Models.
* **Data Layer** — Manages database instances, repositories, and API network clients.

---

### 📁 Project Structure

```text
app
 └── src
      ├── main
      │    ├── java
      │    │    └── com
      │    │         └── notesapp
      │    │              ├── data
      │    │              │    ├── local (Room DB, DAOs)
      │    │              │    └── repository
      │    │              ├── domain
      │    │              │    ├── model
      │    │              │    └── usecase
      │    │              └── presentation
      │    │                   ├── notes
      │    │                   └── viewmodel
      │    ├── res
      │    │    ├── drawable
      │    │    ├── layout
      │    │    ├── values
      │    │    └── xml
      │    └── AndroidManifest.xml
      ├── test
      │    └── ExampleUnitTest
      └── androidTest
           └── ExampleInstrumentedTest
