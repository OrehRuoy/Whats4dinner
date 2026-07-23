# Privacy Policy for **What's 4 Dinner**

**Last updated:** July 23, 2026  

**Package name:** `com.whats4dinner.whats4dinner`

This Privacy Policy describes how the mobile application **What's 4 Dinner** (“the App”) handles information when you use it. By using the App, you agree to this policy.

---

## 1. Who we are

The App is provided by:

**Brock Hall**  
**Contact email:** hallanhype@gmail.com  

---

## 2. Summary

- The App creates an **anonymous account** in the background (no name, email, or password required from you) so recipe search, daily limits, and subscriptions can work.
- **Recipes** are generated using **Google Gemini** (Google AI) via our **Firebase Cloud Functions**, and may be stored in **Cloud Firestore** / **Cloud Storage** so they can be reused.
- **Your filters for a spin** (such as food type, dietary preference, cook time, kid-friendly mode, servings, and allergy selections) are sent to our backend and to Google Gemini to generate a matching recipe.
- **Favorites, meal plans, passport progress, and similar preferences** are stored **locally on your device** (they are not uploaded as a personal cookbook to our servers).
- The App shows **advertisements** using **Google AdMob** (with Google’s consent tools where required) and may use **Firebase Analytics**.
- Optional **Premium** uses **Google Play Billing**.

---

## 3. Information the App processes

### 3.1 Data stored on your device (local)

The App may store data in the app’s private storage on your device (for example Godot `user://` files), including:

- Saved **favorite** / liked recipes and recipes you have marked as **disliked**
- **Meal plan** entries
- **Culinary Passport** progress (for example streaks, badges, cooked history)
- **Dinner preferences** (servings, cook-time bias, dietary filters, kid-friendly option, meal categories, allergy-related selections, reminder and timer settings)
- **Recent recipes** used for “don’t repeat too soon” behavior (also mirrored server-side for the anonymous account — see below)
- Anonymous **Firebase Auth** tokens
- Local **subscription** status cache
- Other app settings (locale, review-prompt state, ad spin counters, and similar)

Uninstalling the App or clearing app data typically removes this local data (depending on your device and backup settings).

### 3.2 Anonymous authentication (Firebase)

When you use the App, it signs you in **anonymously** with **Firebase Authentication**. You do not create a username or password. Firebase assigns an opaque user ID so our backend can:

- Enforce free daily search limits
- Remember recently served recipes for your account
- Associate a Google Play subscription with your App install/session

We do not ask for your name, email address, or phone number for this account.

### 3.3 Recipe search, AI generation, and cloud storage

When you spin for a dinner idea, the App calls our **Firebase Cloud Functions**. Those functions may:

| Service | Purpose |
|---------|---------|
| **Google Gemini (Google AI)** | Generate a recipe (and sometimes a dish image) from your spin filters and related prompt text. |
| **Cloud Firestore** | Store generated recipes in a shared recipe library; store per-anonymous-user search quota, recent served recipes, and subscription verification fields. |
| **Cloud Storage** | Store generated recipe images that can be loaded over HTTPS. |
| **Pixabay** | Fallback stock-image search if AI image generation is unavailable. |
| **TheMealDB** | Occasional client-side fallback for locating a matching dish photo. |

**What may be sent for a spin:** food-type / category choices, dietary option, cook-time option, kid-friendly flag, servings, allergy selections, recently served recipe titles/IDs (to avoid repeats), and technical request metadata required to run the service.

**What we do not upload from your local cookbook:** your full favorites list, meal plan, passport progress, or disliked-recipe list are not sent as a personal profile. Dislikes are used on-device to filter results.

Recipe text and images created by the service may be stored in our cloud databases so later users (including you) can receive a matching cached recipe. Those stored recipes are not labeled with your real-world identity.

Google’s handling of data sent to Gemini / Google AI is also governed by Google’s policies (see links below).

### 3.4 Subscriptions (Google Play Billing)

If you purchase **Premium**, the App uses **Google Play Billing**. A purchase token and product identifier may be sent to our Cloud Functions so we can verify the subscription with Google Play and update your anonymous account’s entitlement (for example unlimited searches / ad-free experience, depending on the product).

Google processes payment details under Google Play’s terms and privacy policy. We do not receive your full payment card number.

### 3.5 Advertising and consent (Google AdMob / UMP)

The App uses **Google AdMob** to display ads (for example banner and interstitial ads). In regions where required (such as the EEA/UK), the App may show Google’s **User Messaging Platform (UMP)** consent form. You may reopen privacy choices from Settings when available.

Google may use identifiers such as the **advertising ID** on Android, device information, and interaction data to show and measure ads, prevent fraud, and (where allowed) personalize ads.

### 3.6 Analytics (Firebase Analytics)

On Android, the App may use **Firebase Analytics** for basic usage metrics (for example screen views and events such as whether a recipe came from cache or was newly generated, with recipe id/category). This helps us understand how the App is used and improve it. Analytics is provided by Google.

### 3.7 Feedback

If you send in-app feedback, your message (and basic app/device context such as app version and device model) may be delivered through a form provider (**Web3Forms**) to reach us by email. Do not include sensitive personal information in feedback unless you are comfortable sharing it.

### 3.8 Technical data

Our backend providers and third-party APIs receive standard technical data involved in network requests (for example IP address, user agent, timestamps, and security tokens), as determined by their infrastructure and policies.

---

## 4. We do not sell your personal data

We do not sell your personal information. We use the data described above to operate the App (recipe search, limits, subscriptions, ads, analytics, and support).

---

## 5. Children’s privacy

The App is not directed at children under 13 (or the minimum age required in your country). We do not knowingly collect personal information from children for our own use beyond what third parties (such as Google) may process as part of normal ad, analytics, and network operations. If you believe a child has provided personal data in a way that concerns you, contact us at the email above.

---

## 6. Security

We use industry-standard providers (Firebase / Google) and keep favorites and many preferences on the device. No method of transmission or storage is 100% secure; use the App at your own discretion.

---

## 7. International users

If you use the App from outside your home country, data may be processed in countries where Google (Firebase, Gemini, AdMob, Analytics, Play), Pixabay, TheMealDB, Web3Forms, or their infrastructure operate.

---

## 8. Your choices

- **Ads / privacy choices:** Use the in-app Settings privacy choices (where available), and/or your device and Google account settings to limit ad personalization.
- **Local data:** Clear app data or uninstall the App to remove locally stored preferences, favorites, and the anonymous auth session on that device.
- **Subscription:** Manage or cancel Premium through Google Play.
- **Questions:** Email us at the contact address at the top of this policy.

---

## 9. Changes to this policy

We may update this Privacy Policy from time to time. The **“Last updated”** date at the top will change when we do. Continued use of the App after changes means you accept the updated policy. For material changes, we may also update the policy URL in the Google Play listing.

---

## 10. Third-party services

The App relies on third parties whose own privacy policies apply to their processing, including:

- [Google Privacy Policy](https://policies.google.com/privacy) (Firebase, Gemini / Google AI, AdMob, Analytics, Play)
- [How Google uses information from sites or apps that use our services](https://policies.google.com/technologies/partner-sites)
- [Pixabay](https://pixabay.com/service/privacy/)
- [TheMealDB](https://www.themealdb.com)

---

*This document is provided for **What's 4 Dinner**. It is not legal advice. You may wish to have a lawyer review it for your jurisdiction (for example GDPR, UK GDPR, or US state laws) before publishing.*
