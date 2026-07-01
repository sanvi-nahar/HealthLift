# HealthLift - Health Monitoring Android App

HealthLift is a comprehensive Android application designed to help users track and monitor their vital health statistics. Built using Java and SQLite, the app provides a user-friendly interface to record and visualize health data such as Blood Pressure, Sugar Levels, and Calorie Intake over time.

## 🚀 Features

### 1. User Authentication & Profile
- **Secure Login/Register**: Users can create an account and securely log in.
- **Session Management**: Maintains user session for a seamless experience.
- **Profile Management**: Users can update their personal details including Name, Date of Birth, Height, and Weight.
- **Profile Picture**: Support for uploading and displaying a profile image.

### 2. Blood Pressure Tracking
- **Record Readings**: Save Systolic, Diastolic, and Pulse readings.
- **Automatic Timestamp**: Logs the date and time of each entry.
- **History View**: Review all past blood pressure records in a clean list format.
- **Graphical Reports**: Visualize blood pressure trends using interactive charts (Weekly, Monthly, Yearly).

### 3. Sugar Level Monitoring
- **Log Glucose Levels**: Record Glycemic Index readings and status.
- **Tracking**: Monitor fluctuations in sugar levels over different periods.
- **Detailed Reports**: Graphical representation of sugar level history for better health insights.

### 4. Calorie Intake Tracker
- **Log Daily Calories**: Keep track of daily calorie consumption.
- **Progress Monitoring**: View calorie intake history and trends.
- **Visual Analytics**: Use charts to understand dietary habits over time.

### 5. Advanced Data Visualization
- **MPAndroidChart Integration**: Beautiful and interactive line/bar charts for health data analysis.
- **Health Statistics**: View Average, Minimum, and Maximum values for all tracked metrics.
- **Dynamic Reports**: Switch between Weekly, Monthly, and Yearly views for all health parameters.

### 6. User Experience
- **Splash Screen**: Professional intro screen.
- **Onboarding**: Informative slides for first-time users.
- **Lottie Animations**: Engaging UI transitions and feedback.
- **Circular Progress Bars**: Visual progress indicators for health targets.

---

## 🛠️ Technology Stack

- **Platform**: Android
- **Language**: Java (JDK 8)
- **Database**: SQLite (Local Storage)
- **Architecture**: Model-View-Controller (MVC) pattern
- **UI Components**: Material Design, ConstraintLayout, RecyclerView, Fragments
- **Libraries Used**:
  - `MPAndroidChart`: For data visualization.
  - `Lottie`: For high-quality animations.
  - `CircularProgressBar`: For progress tracking.
  - `Balloon`: For interactive tooltips.
  - `NumberPicker`: For easy data entry.

---

## 📂 Project Structure

```text
app/src/main/java/com/example/healthlift/
├── AdapterClasses/   # RecyclerView and ViewPager adapters
├── Common/           # Splash, Welcome, and Onboarding screens
├── Database/         # DbHelper.java for SQLite operations
├── Entities/         # Data models for BP, Sugar, and Calories
├── Sessions/         # Session management logic
└── User/             # Main Activities and Fragments for user features
```

---

## ⚙️ How to Run

### Prerequisites
- **Android Studio** (Electric Eel or newer recommended)
- **Android SDK** (API 33 supported)
- **Java Development Kit (JDK)** 8 or higher

### Steps to Install & Run
1. **Clone/Download**: Download the project ZIP and extract it.
2. **Open in Android Studio**:
   - Open Android Studio.
   - Click on `File` > `Open`.
   - Navigate to the project directory and select the inner `Health-Monitoring-App-Android-Java-master` folder.
3. **Gradle Sync**:
   - Wait for Android Studio to sync the project with Gradle files.
   - Ensure you have an active internet connection to download dependencies.
4. **Setup Emulator/Device**:
   - Use a Physical Device via USB Debugging OR
   - Create a Virtual Device (Emulator) with at least **API 25 (Android 7.1.1)**.
5. **Run the App**:
   - Click the green **Run** button (or press `Shift + F10`).
   - The app will build and install on your device.

---

## 📋 Database Schema

The app uses an internal SQLite database named `healthLiftDb` with the following tables:
- `tbl_users`: Stores user credentials and physical attributes.
- `tbl_blood_pressure`: Stores BP readings (Systolic, Diastolic, Pulse).
- `tbl_sugar_levels`: Stores glucose readings.
- `tbl_calories`: Stores daily calorie logs.
- `tbl_profiles`: Stores user profile images in BLOB format.

---

## 🛡️ License
This project is for educational purposes. Feel free to use and modify it.

---

**Developed with ❤️ for Health Awareness.**
