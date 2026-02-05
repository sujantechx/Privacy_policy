# Google Play Console Data Safety Questionnaire
**App Name:** SZ Ride Book

Use this guide to answer the "Data Safety" section in the Google Play Console.

## 1. Data Collection and Security

| Question | Answer | Notes |
| :--- | :--- | :--- |
| **Does your app collect or share any of the required user data types?** | **Yes** | |
| **Is all of the user data collected by your app encrypted in transit?** | **Yes** | HTTPS/SSL is standard for Firebase/APIs. |
| **Do you provide a way for users to request that their data be deleted?** | **Yes** | Required. You must provide an email or in-app option. |

---

## 2. Data Types

Select the following data types that your app collects or shares:

### 📍 Location
*   **Approximate location** (Collected)
*   **Precise location** (Collected)
    *   *Purpose:* App functionality (Booking rides)
    *   *Sharable?* No (unless you share with drivers, then Yes) -> **Usually "No" for basic apps, "Yes" if sharing with 3rd party drivers.**
    *   *Ephemeral?* No

### 👤 Personal Info
*   **Name** (Collected)
    *   *Purpose:* App functionality, Account Management
*   **Phone number** (Collected)
    *   *Purpose:* App functionality, Account Management

### 💳 Financial Info
*(Only select if you process payments directly. If you use a 3rd party gateway webview, you might not "collect" it, but it's safer to declare if stored).*
*   **User Payment Info**: [Select if applicable]
*   **Purchase History**: (Collected - "Ride History")
    *   *Purpose:* App functionality

### 📷 Photos and Videos
*(Select if users upload profile pics)*
*   **Photos** (Collected)
    *   *Purpose:* App functionality (User profile/Verification)

### 🆔 Device or Other IDs
*   **Device or other IDs** (Collected)
    *   *Purpose:* Analytics, App Functionality, Fraud Prevention (Firebase ID)

### 📲 App Info and Performance
*   **Crash logs** (Collected)
    *   *Purpose:* Analytics
*   **Diagnostics** (Collected)
    *   *Purpose:* Analytics

---

## 3. Usage & Handling (For each selected type)

For most items (Name, Phone, Location, Device ID):

*   **Is this data collected, shared, or both?** -> **Collected** (Share only if you send to external partners like ad networks or separate dispatch services).
*   **Is this data processed ephemerally?** -> **No** (You store history/profiles).
*   **Is this data required for your app?** -> **Yes** (Users can't book without it).
*   **Why is this data collected?** -> Select: **App Functionality**, **Account Management**, **Fraud Prevention** (Device IDs).

---

## 4. Privacy Policy Link
Ensure your store listing links to your Google Site URL:
`https://sites.google.com/view/[your-site-name]/privacy/sz-ride-book`
