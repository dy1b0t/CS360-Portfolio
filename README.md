# Project Three: Dylan Miller

**Course:** Mobile Architecture and Programming  

---

## 1. Project Overview

For Project Three, I developed a fully functional Android mobile application called **EventTracker**, based on the UI designs from Project Two. This is a simple event logging and tracking app that allows users to record events with timestamps and view them in a structured format. The goal was to provide users with a clean, user-centered interface for managing personal events or recurring logs in a lightweight and accessible way.

---

## 2. Requirements & Goals

- **Essential Requirements:**
  - Implement the main screens and navigation structure
  - Build features that meet user needs based on the UI design
  - Follow mobile development best practices
  - Ensure the interface is responsive, accessible, and intuitive

- **Goals:**
  - Translate visual designs into working code
  - Apply clean architecture and consistent styling
  - Provide seamless user experience across screens

---

## 3. UI Design & Features

I implemented the following screens and features to meet user needs:

- **LoginActivity:** Basic login screen (local only, no external auth)
- **SMSPermissionActivity:** Requests runtime SMS permissions
- **MainActivity:** Home screen that displays event records using a RecyclerView
- **AddEventActivity:** Lets users add new events with a timestamp
- **Records Adapter & Data Model:** Handles the display and structure of stored event data

**User-centered design strategies implemented:**

- Simple, clean layout with clear input fields and buttons
- Large tap targets and readable font sizes for accessibility
- Logical screen transitions with intuitive flow
- Local database used for persistent storage with `SQLiteOpenHelper`

These design choices ensured the app was functional, reliable, and easy to use.

---

## 4. Development Approach

### Coding Techniques

- Architecture followed MVC principles
- Java with native Android SDK
- `DbHelper` class for SQLite database interactions
- `RecyclerView` and custom `EventAdapter` for dynamic data presentation
- Intents for activity transitions

### Strategy Highlights

- Built and tested each activity individually
- Modularized database access logic in `DbHelper`
- Designed layout XMLs in parallel with Java functionality
- Used Android Studio emulator for fast feedback loops

These methods promoted code clarity and scalability for future feature additions.

---

## 5. Testing & Quality Assurance

- Manual walkthroughs of each activity to verify UI behavior and data flow
- Tested SMS permission handling across different device profiles
- Ensured input validation on `AddEventActivity` to prevent blank submissions
- Verified data persistence using `SQLite` and correct rendering in the `RecyclerView`

**Why it mattered:**  
Testing helped identify and fix early bugs related to navigation, empty inputs, and permissions. It ensured that the app functioned smoothly and predictably in its core use cases.

---

## 6. Challenges & Innovation

One notable challenge was managing SQLite data storage and display consistency between `MainActivity` and `AddEventActivity`.  
To solve this, I:

- Built a clear contract in the `DbHelper` class
- Used an `EventAdapter` to decouple logic from UI rendering
- Ensured the `MainActivity` refreshes its list on resume to reflect new entries

This improved the app’s responsiveness and made event tracking seamless.

---

## 7. Key Accomplishment

I was particularly successful in implementing the SQLite data layer and integrating it smoothly with the RecyclerView display. By structuring my database logic in a dedicated helper class and using a custom adapter, I delivered a modular and functional system that:

- Stores user-generated data locally
- Displays data in an organized list format
- Demonstrates my understanding of Android components, UI interaction, and persistent storage

---

## What’s Uploaded

1. **`DylanMillerEventTracking_project3.zip`**  
   - Final Java source code from Project Three

2. **`README.md`**  
   - This document with full project reflection

---
