# Privacy Policy — Massar

**Last updated:** 12 May 2026
**Effective date:** 20 May 2026

This Privacy Policy describes how **Massar** ("we", "us", "our") collects, uses, stores, and shares personal information when you use our mobile applications:

- **Massar Transporteur** (bus owners)
- **Massar Chauffeur** (drivers)
- **Massar Voyageur** (passengers)

By using any of our applications, you agree to the practices described in this policy.

---

## 1. Who We Are

Massar is a real-time bus transport platform operating in Algeria.

- **Operator:** yanis mazouz
- **Address:** bouira ville , bouira , algeria 
- **Contact:** massarsystem@gmail.com
- **Country of operation:** Algeria

---

## 2. Information We Collect

We collect only the information needed to operate the service. Categories vary by app.

### 2.1 Account information (all apps)
- Email address
- Password (stored hashed by Firebase Authentication; we never see your plaintext password)
- Phone number (when used for authentication)
- Display name
- Role (owner, driver, passenger, admin)
- Profile photo (optional)

### 2.2 Location information
- **Chauffeur app:** Live GPS coordinates of the driver's device while a trip is active. Coordinates are broadcast to passengers tracking that bus. We only collect location during active trips, with a minimum movement threshold of 20 meters or a 30-second heartbeat.
- **Voyageur app:** Your current location is read **on-device only** to show nearby buses on the map. We do not store passenger locations on our servers.
- **Transport app & Admin web:** No passenger or driver location data is collected beyond what is needed for fleet management dashboards.

Background location is collected by the Chauffeur app **only while a trip is in progress**. It stops when the trip ends or the driver goes off-duty.

### 2.3 Bus, trip, and fleet data
- Vehicle information (license plate, line name, capacity, type)
- Trip history (start/end times, route, status)
- Maintenance records (entered by owners)

### 2.4 Payment and subscription data (Transport app only)
- Subscription plan, billing history, payment confirmation references
- We do **not** store full credit card numbers. Payments are processed by yanis mazouz.

### 2.5 Device and technical information
- Firebase Cloud Messaging (FCM) device token (for push notifications)
- App version, OS version, device model (automatically collected by Firebase)
- Crash reports and diagnostic data (Firebase Crashlytics)
- Approximate IP address (for security and abuse prevention)

### 2.6 Usage data
- Anonymous usage analytics (screen views, feature usage) via Firebase Analytics
- We do not use this data to build advertising profiles

---

## 3. How We Use Your Information

We use your data only to:

1. Provide the core service — connecting bus owners, drivers, and passengers in real time.
2. Authenticate you and protect your account.
3. Enable real-time bus tracking on the map.
4. Send operational push notifications (trip alerts, maintenance reminders, payment confirmations).
5. Process subscription payments for bus owners.
6. Provide customer support.
7. Detect, prevent, and respond to fraud, abuse, or security incidents.
8. Comply with applicable law.

We do **not** sell your personal information to anyone, and we do not use it for advertising profiling.

---

## 4. Legal Basis (Algerian Law 18-07 & General Principles)

We process your personal data under the following legal bases:

- **Performance of a contract** — providing the service you signed up for.
- **Consent** — for optional features (e.g., promotional notifications) which you can withdraw at any time.
- **Legitimate interest** — security, fraud prevention, and service improvement.
- **Legal obligation** — when required to comply with Algerian law.

Our data processing complies with **Algerian Law No. 18-07 of June 10, 2018** on the protection of natural persons in the processing of personal data.

---

## 5. Sharing of Information

We share data only with the following categories of recipients, and only as needed to operate the service:

| Recipient | Purpose | Data shared |
|---|---|---|
| **Google / Firebase** | Authentication, database, push notifications, analytics, crash reporting | Account info, FCM token, device info, usage data |
| **Supabase** | File storage (vehicle photos, documents), backend functions | Files you upload, account ID |
| **Mapbox** | Map tiles and routing | Anonymized location queries (start/end coordinates) |
| **[PAYMENT PROVIDER]** | Subscription payment processing | Transaction info |
| **Drivers and passengers using our apps** | Real-time bus tracking | Bus location, line name, plate (during active trips only) |
| **Algerian authorities** | Compliance with legal orders | Only as required by law |

We do not transfer personal data to recipients outside Algeria except to the international cloud providers listed above, which apply standard data protection practices.

---

## 6. Data Retention

- **Account data:** kept while your account is active and for up to **12 months** after you delete it (for legal and dispute-resolution reasons), after which it is permanently deleted.
- **Location data (drivers):** kept for **90 days** for operational and dispute purposes, then deleted.
- **Payment records:** kept for **10 years** as required by Algerian commercial law.
- **Crash logs and diagnostics:** retained for **90 days** by Firebase Crashlytics.

---

## 7. Your Rights

You have the right to:

1. **Access** your personal data we hold.
2. **Correct** inaccurate or incomplete data — you can update most fields directly in the app.
3. **Delete** your account and associated personal data.
4. **Object to** or **restrict** certain processing.
5. **Withdraw consent** for optional processing at any time.
6. **Export** a copy of your data in a structured, machine-readable format.

To exercise any of these rights, contact us at **massarsystem@gmail.com**. We will respond within 30 days.

### Account deletion
You can delete your account directly from the app:

- **Transporteur app:** Settings → Account → Delete Account
- **Chauffeur app:** Settings → Account → Delete Account
- **Voyageur app:** Settings → Account → Delete Account

Or request deletion by email at **massarsystem@gmail.com**.

---

## 8. Security

We protect your data using:

- HTTPS/TLS encryption for all network traffic
- Firebase Authentication for credential management
- Firestore Security Rules to enforce strict access control on every read/write
- Hashed and salted passwords (handled by Firebase)
- Role-based access (drivers can only see their own bus data; passengers can only see public bus tracking; owners only see their fleet)

No system is 100% secure. If we discover a data breach affecting your personal data, we will notify you and the competent Algerian authority as required by law.

---

## 9. Children's Privacy

Our apps are not intended for children under **13 years old**. We do not knowingly collect personal data from children under 13. If you believe we have collected data from a child under 13, please contact us so we can delete it.

The Voyageur app may be used by minors aged 13 and above with parental consent.

---

## 10. Third-Party Services

Our apps integrate with the following third parties, each governed by their own privacy policy:

- **Google Firebase** — https://policies.google.com/privacy
- **Supabase** — https://supabase.com/privacy
- **Mapbox** — https://www.mapbox.com/legal/privacy

---

## 11. Permissions Used

| Permission | App(s) | Why we need it |
|---|---|---|
| Internet | All | Communicate with our servers |
| Location (precise) | Chauffeur, Voyageur | Driver GPS broadcasting; passenger nearby-bus search |
| Background location | Chauffeur (only) | Continue broadcasting GPS while the driver's phone is in their pocket during a trip. We **only** access background location while a trip is active. |
| Camera | Transporteur, Chauffeur | Take photos of vehicles, insurance documents, maintenance receipts |
| Storage / Photos | Transporteur, Chauffeur | Upload vehicle and document photos |
| Notifications | All | Send trip alerts, maintenance reminders, payment confirmations |
| Phone state | All | Phone-number-based authentication |

You can revoke any permission at any time in your device settings. Some features will stop working when the corresponding permission is revoked.

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of significant changes through an in-app notice or email, and post the updated version with a new "Last updated" date.

---

## 13. Contact Us

For any privacy-related question or to exercise your rights, contact:

**Email:** massarsystem@gmail.com
**Address:** bouira ville , bouira , algeria 

For complaints, you may also contact the Algerian National Authority for the Protection of Personal Data (Autorité Nationale de Protection des Données Personnelles — ANPDP).

---

## Appendix — Google Play Data Safety Declaration

This appendix summarizes what to declare in the Google Play Console "Data Safety" form for each app.

### Massar Voyageur (passenger)
- **Personal info:** Name, Email, User ID — Collected, linked to user, **not** shared, used for account management.
- **Location:** Approximate location — **Not collected** by server (read on-device only).
- **App activity:** App interactions — Collected (Firebase Analytics), not shared, used for analytics.
- **App info and performance:** Crash logs, diagnostics — Collected (Crashlytics), not shared, used for app functionality.
- **Device or other IDs:** Device ID (FCM token) — Collected, linked to user, used for app functionality (notifications).
- **Encrypted in transit:** Yes
- **Users can request deletion:** Yes

### Massar Chauffeur (driver)
All of the Voyageur items, plus:
- **Location:** Precise location — Collected, linked to user, shared with other users (passengers tracking the bus), used for app functionality. Collected only during active trips.
- **Photos:** Collected (vehicle/document uploads), linked to user, not shared, used for app functionality.

### Massar Transporteur (owner)
All of the Voyageur items, plus:
- **Financial info:** Purchase history (subscription only — no card data) — Collected, linked to user, not shared, used for app functionality.
- **Photos:** Collected (vehicle/document uploads), linked to user, not shared, used for app functionality.

---

*This document is provided as a starting template. We strongly recommend a final review by a lawyer familiar with Algerian Law 18-07 before publishing the apps.*
