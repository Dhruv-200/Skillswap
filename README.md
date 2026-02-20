# SkillSwap
[![Ask DeepWiki](https://devin.ai/assets/askdeepwiki.png)](https://deepwiki.com/Dhruv-200/Skillswap)

SkillSwap is a peer-to-peer skill exchange platform built on a time-based economy. Instead of money, users trade their time and skills for credits. Teach an hour of Python to earn a credit, and then use that credit to learn an hour of UI/UX design from another expert. It's a community-driven ecosystem where everyone's time holds equal value.

## ✨ Core Features

*   **Skill Marketplace**: Post skills you can teach and browse a rich marketplace of skills offered by others.
*   **Credit-Based Economy**: Earn credits by teaching and spend them to learn. One hour of any skill is equivalent to one credit.
*   **Advanced Booking System**: Schedule sessions with providers, manage your calendar, and get automatic meeting links.
*   **Real-time Messaging**: An in-app chat system allows users to communicate and coordinate sessions.
*   **Programming Quiz Challenge**: Test your knowledge in over 10 programming languages, earn badges, and climb the leaderboard.
*   **AI-Powered Learning Assistant**: Get personalized skill recommendations, discover auto-generated learning paths, and explore a skill compatibility matrix.
*   **Comprehensive User Dashboard**: Manage your skills, track upcoming sessions, view transaction history, and see incoming requests from learners.
*   **Feedback & Rating System**: A multi-step feedback process allows users to rate sessions and provide detailed reviews to build a trusted community.
*   **Community Hub**: Explore community stats, see top-performing providers, and view a live feed of recent activity on the platform.
*   **Google Calendar Integration**: Automatically create calendar events for confirmed sessions, complete with meeting links and reminders.

## 🛠️ Tech Stack

*   **Frontend**: React, Vite, TypeScript
*   **UI Framework**: Tailwind CSS, shadcn/ui
*   **State Management**: React Query
*   **Routing**: React Router
*   **Backend & Database**: Firebase (Authentication, Firestore, Cloud Functions, Storage)

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   Node.js (v18 or later)
*   npm or yarn

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/dhruv-200/Skillswap.git
    cd Skillswap
    ```

2.  **Install dependencies:**
    ```sh
    npm install
    ```

3.  **Set up Firebase:**
    *   Create a project on the [Firebase Console](https://console.firebase.google.com/).
    *   In your project dashboard, go to **Project Settings** > **General** and find your web app's configuration object.
    *   Create a `.env.local` file in the root of the project.
    *   Copy the following environment variables into your `.env.local` file and replace the placeholder values with your Firebase config keys:
        ```env
        VITE_FIREBASE_API_KEY=your-api-key-here
        VITE_FIREBASE_AUTH_DOMAIN=your-project-id.firebaseapp.com
        VITE_FIREBASE_PROJECT_ID=your-project-id
        VITE_FIREBASE_STORAGE_BUCKET=your-project-id.appspot.com
        VITE_FIREBASE_MESSAGING_SENDER_ID=your-sender-id
        VITE_FIREBASE_APP_ID=your-app-id
        ```
    *   In the Firebase Console, navigate to **Authentication** > **Sign-in method** and enable the **Email/Password** and **Google** providers.
    *   Under **Authentication** > **Settings** > **Authorized domains**, add `localhost`.
    *   The required Firestore database rules and indexes are located in `firestore.rules` and `firestore.indexes.json`. You will need to deploy these to your project using the Firebase CLI.

4.  **Run the development server:**
    ```sh
    npm run dev
    ```
    The application will be available at `http://localhost:8080`.
