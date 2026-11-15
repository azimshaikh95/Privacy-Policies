# Privacy Policy for Khutbah Minbar

**Effective Date:** November 14, 2026  
**App Name:** Khutbah Minbar (منبر الخطب)  
**Package / Bundle ID:** `com.azim.khutbat`  
**Developer / Contact Email:** [azim.zaytunweb@gmail.com](mailto:azim.zaytunweb@gmail.com)

---

## 1. Overview

Khutbah Minbar ("we," "our," or "the App") is a digital Friday sermon (*khutbah*) reader, archive, and editorial manuscript management application designed for Imams, Khatibs, and community readers. We respect your privacy and are committed to transparency regarding the limited information processed to provide core app functionality.

> We do **not** sell personal data, display third-party advertisements, or use behavioral tracking or analytics SDKs.

---

## 2. Information We Collect

### A. Usage Without an Account (Guest Access)
You can browse published sermons, read in the Minbar Reader, bookmark sermons, customize reading fonts/themes, and export sermons to PDF or DOCX without creating an account or providing personal information.

### B. Account Information (Optional Sign-In)
If you choose to sign in (using Email & Password, Passwordless Email Sign-In Link, or Google Sign-In), Firebase Authentication processes:
* Email address
* Display name (if provided by your Google account or profile)
* Authentication User ID (UID) and authentication provider metadata

This information is used solely to authenticate your session and determine role-based access permissions (Reader, Author/Editor, or Super Admin).

### C. Editorial & Manuscript Content (Authors & Admins Only)
When an authorized Author or Administrator creates, edits, imports, or publishes a sermon manuscript, the manuscript text and metadata (title, subtitle, body text, category, tags, dates, optional Khatib/author display name, and account identifier/email associated with the record) are stored in Google Cloud Firestore so sermons can be synced across devices.

### D. Locally Stored Preferences & Offline Cache (On-Device)
To support offline reading inside mosques with limited connectivity and remember your preferences, the App stores the following strictly on your device (`localStorage` and browser/WebView `IndexedDB`):
* **Offline Sermon Cache:** Previously loaded published sermons cached via Firestore IndexedDB persistence and local storage.
* **Reading Preferences:** Selected Arabic reading font, reader text size, and reader color theme (Parchment, White, Dark).
* **Bookmarks:** IDs of sermons you bookmark.
* **Session & Role Preferences:** Cached authentication session state and, during passwordless email link sign-in, the temporary email address used to complete verification.

You can clear all locally stored data at any time by clearing your browser/app storage or uninstalling the application.

---

## 3. Document Exports & File Imports

* **PDF & DOCX Downloads:** Sermon exports (`.pdf` and `.docx`) are generated locally on your device. No sermon content is transmitted to an external conversion server.
* **JSON Backup / Restore / Import:** Backup files are generated locally on your device, and imported JSON files are read locally before authorized manuscripts are saved to Cloud Firestore.

---

## 4. Third-Party Services

The App relies on the following essential infrastructure providers:
* **Google Firebase (Firebase Authentication & Cloud Firestore):** Used for optional user sign-in, access control, and cloud sermon storage/synchronization. Governed by the Google Privacy Policy and Firebase Privacy & Security Documentation.
* **Font Delivery Networks (Google Fonts & jsDelivr CDN):** Used to load Arabic and UI typefaces (such as *Noto Naskh Arabic*, *Amiri*, *Scheherazade New*, *Cairo*, *KFGQPC Uthman Taha Naskh*, and *Al Qalam Quran Majeed*). When fetching font files over the network, these services may receive standard HTTP request metadata (such as IP address and browser user-agent) in accordance with their respective privacy policies.

---

## 5. Device Permissions

Khutbah Minbar does **not** request access to device location (GPS), camera, microphone, contacts, SMS, or call logs. Network access is used solely to fetch/sync sermons, load web fonts, and perform optional user authentication.

---

## 6. Data Security & Retention

* All network communications between the App and Firebase services are encrypted in transit via HTTPS/TLS.
* Account data is retained only as long as your account remains active.
* Draft manuscripts remain restricted to authorized editorial users in the app UI and are not displayed to the general public until published.

---

## 7. Your Rights & Account / Data Deletion

You have the right to:
* Access or update your account details.
* Sign out at any time from the Profile tab, which clears your active local session.
* Clear local data (bookmarks, font/theme settings, offline cache) via your device or browser settings.
* Request permanent deletion of your Firebase Authentication account and associated user records by emailing `[Support Email]` from your registered email address. Deletion requests are processed within **30 days**.

---

## 8. Children's Privacy

Khutbah Minbar is a general-audience religious and educational reference application. We do not knowingly collect personal information from children under the age of 13 (or the applicable age of digital consent in your jurisdiction). If you believe a child has submitted personal data through an account, please contact us so we can delete it promptly.

---

## 9. Changes to This Privacy Policy

We may update this Privacy Policy periodically to reflect app updates or legal requirements. Any revisions will be posted with an updated "Effective Date" at the top of this policy.

---

## 10. Contact Us

If you have any questions or feedback regarding this Privacy Policy or the technical functionality of the App, please reach out to:

* **Email:** [azim.zaytunweb@gmail.com](mailto:azim.zaytunweb@gmail.com)
