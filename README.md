# MFL Health & Cycle Companion App

A cross-platform mobile application engineered for intuitive tracking of health metrics, menstrual cycles, and personalized nutrition logs.

---

## Tech Stack

* **Frontend:** React Native, Expo CLI
* **Backend & Database:** Supabase (PostgreSQL)
* **Authentication:** Supabase Auth (JWT-based session handling)
* **State Management:** Async local storage with optimistic UI updates

---

## Engineering Highlights

* **Row-Level Security (RLS):** Configured PostgreSQL policies in Supabase ensuring health metrics and personal logs are accessible solely by authenticated account holders.
* **Offline-First Capabilities:** Implemented local state caching so users can log symptoms without connection loss interrupting app state; automatically syncs when network reconnects.
* **Modular Component Tree:** Clean separation of UI views, date math utilities (ovulation & cycle projection algorithms), and API services.

---

## Setup & Running Locally

1. **Clone & Install:**
   ```bash
   git clone [https://github.com/RAdeelAleem/mfl-mobile-app.git](https://github.com/RAdeelAleem/mfl-mobile-app.git)
   cd mfl-mobile-app
   npm install
   ```

2. **Environment Variables:**
   Create a `.env` file based on `.env.example`:
   ```env
   EXPO_PUBLIC_SUPABASE_URL=your_supabase_url
   EXPO_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

3. **Start the Development Server:**
   ```bash
   npx expo start
   ```
   Scan the generated QR code via Expo Go on iOS or Android.

---

## License
MIT License
