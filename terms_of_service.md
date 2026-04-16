# TxTTone

## Privacy Policy

**Last Updated:** April 15, 2026 • Version 1.3

Charles Hall ("we," "our," or "us") operates the TxTTone mobile application (the "App"). This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our App.

Please read this Privacy Policy carefully. By using the App, you agree to the collection and use of information in accordance with this policy. If you do not agree with the terms of this Privacy Policy, please do not use the App.

---

## 1. Information We Collect

### 1.1 Contact Information

We access your device's contact list to allow you to assign custom ringtones and notification sounds to specific contacts. This information is stored locally on your device and is never transmitted to our servers.

When the per-contact ringtone queue feature is enabled, TxTTone writes a ringtone URI to the standard `CUSTOM_RINGTONE` field in your device's Contacts database. This is a standard Android field read by the native dialer to play the assigned ringtone when that contact calls. No other contact data is read or modified. This change is made locally on your device and is never transmitted externally.

### 1.2 Notification Metadata

TxTTone uses the Android Notification Access permission to detect incoming message and call notifications. The app reads only notification metadata (sender name and originating app identifier). It does not access, read, store, or transmit message content or notification bodies. All notification processing occurs locally on your device and no data is retained after processing. TxTTone does not collect this data — it is processed in real time and discarded.

### 1.3 Audio Files

The App allows you to select and use audio files as ringtones and notification sounds. These audio files are stored locally on your device. We do not upload, transmit, or store your audio files on our servers.

You may also record or import custom audio clips directly within the App. These user-created or user-imported sound files are stored locally on your device in the App's private storage directory. They are never transmitted to our servers, shared with third parties, or used for any purpose other than playback within the App. You can delete these files at any time by removing them within the App or by clearing the App's data via Android Settings → Apps → TxTTone → Clear app data.

When TxTTone copies a sound file for use as a native ringtone, it stores a managed copy in `Ringtones/TxTTone/` in your device's shared storage. This folder and its contents may persist after the app is uninstalled, as Android does not automatically delete files in shared storage on uninstall. You can delete these files manually using any file manager app.

### 1.4 System Settings and Ringtone Staging

When the Custom Ringtones feature is enabled by the user, TxTTone uses the WRITE_SETTINGS permission to manage your system ringtone as follows:

- **Ringtone suppression for text tones:** TxTTone temporarily suppresses the system notification sound while a custom text tone is playing, so your custom sound plays cleanly. Your original ringtone is not modified by this process.
- **Per-contact ringtone staging:** TxTTone writes the contact's assigned ringtone URI to their `CUSTOM_RINGTONE` field in your Contacts database so Samsung's native dialer plays it when that person calls.
- **Global native ringtone randomization:** When this optional feature is enabled, TxTTone stages the next sound in your playlist as the system default ringtone ahead of incoming calls. Your original ringtone URI is saved locally and restored when the feature is disabled.

All system setting changes are made locally on your device and are never transmitted externally. You can restore your original ringtone manually at any time via the Restore button in Settings.

### 1.5 Usage and Diagnostic Data

TxTTone itself does not collect usage data. However, third-party SDKs integrated into the App collect the following on our behalf:

- **Crash reports and error logs** — via Firebase Crashlytics (stack traces and device state only, no personal data)
- **App usage statistics and analytics** — via Firebase Analytics

These SDKs operate under their own privacy policies, linked in Section 4.

---

## 2. How We Use Your Information

We use the collected information for the following purposes:

- **To provide and maintain the App:** Enable core functionality including contact-based sound assignments
- **To improve user experience:** Analyze usage patterns to enhance features and performance
- **To fix bugs and crashes:** Use crash reports to identify and resolve technical issues
- **To display advertisements:** Show relevant ads to support the free version of the App
- **To process purchases:** Handle in-app purchases for the ad-free premium version
- **To communicate with you:** Respond to support requests and send important updates
- **To comply with legal obligations:** Meet legal and regulatory requirements

---

## 3. Data Storage

### 3.1 Local Storage

Contact associations, audio selections, and app settings are stored locally on your device. This data is not transmitted to external servers.

### 3.2 Backup

TxTTone includes an optional local backup feature that exports your settings and sound library to a zip file on your device. This backup file is stored wherever you choose to save it on your device or cloud storage of your choice. We do not operate any cloud backup service. The backup file contains only sound files and app settings — no notification content or contact details.

### 3.3 Security Measures

We implement appropriate technical measures to protect your information. Third-party SDKs (AdMob, Firebase) use encrypted data transmission (HTTPS). No method of electronic storage is 100% secure, and we cannot guarantee absolute security.

---

## 4. Third-Party Services

### 4.1 Advertising

We use Google AdMob to display advertisements in the free version of the App. AdMob may collect device identifiers, IP address, and usage data.
AdMob Privacy Policy: https://policies.google.com/privacy

### 4.2 Analytics

We use Firebase Analytics to understand app usage and improve our services. Firebase may collect app usage data, device information, and crash reports.
Firebase Privacy Policy: https://firebase.google.com/support/privacy

### 4.3 Crash Reporting

We use Firebase Crashlytics to collect crash reports and diagnostic information. Crashlytics collects device state information, stack traces, and app logs. Crash reports contain no notification content, contact names, or personal data.

### 4.4 In-App Purchases

We use Google Play Billing to process in-app purchases. Google handles payment processing and may collect payment information.
Google Play Terms of Service: https://play.google.com/about/play-terms/

---

## 5. Permissions

The App requires or may request the following permissions:

- **BIND_NOTIFICATION_LISTENER_SERVICE:** To detect incoming message and call notifications so custom sounds can be played at the right moment
- **READ_CONTACTS:** To access your contact list for assigning custom sounds to specific contacts
- **WRITE_CONTACTS:** To write a custom ringtone URI to the per-contact ringtone field in your Contacts database. Required for the per-contact ringtone queue feature. No other contact data is modified.
- **READ_PHONE_STATE:** To detect incoming call state so TxTTone knows when to play custom ringtones and when to stop them. TxTTone does not read call logs, record calls, or access call content.
- **WRITE_SETTINGS:** To manage the system ringtone setting when Custom Ringtones is enabled. This is required for the feature to function, is user-initiated, and is fully reversible.
- **READ_EXTERNAL_STORAGE / READ_MEDIA_AUDIO:** To access audio files on your device for use as custom sounds
- **POST_NOTIFICATIONS:** To post notifications on Android 13 and above
- **INTERNET:** To display advertisements and send crash/analytics reports
- **ACCESS_NETWORK_STATE:** To determine network connectivity
- **ROLE_CALL_SCREENING (optional):** If granted, gives TxTTone advance notice of incoming calls for more reliable custom ringtone playback. This role is optional and can be skipped or revoked at any time.

You can manage these permissions in your device settings at any time.

---

## 6. Data Sharing and Disclosure

We do not sell, trade, or rent your personal information to third parties. We may share your information in the following circumstances:

### 6.1 With Your Consent

We may share information when you explicitly give us permission to do so.

### 6.2 Service Providers

We may share information with third-party service providers who perform services on our behalf (e.g., analytics, advertising, crash reporting).

### 6.3 Legal Requirements

We may disclose your information if required to do so by law or in response to valid requests by public authorities.

### 6.4 Business Transfers

If we are involved in a merger, acquisition, or sale of assets, your information may be transferred. We will provide notice before your information is transferred and becomes subject to a different Privacy Policy.

---

## 7. Children's Privacy

The App is not intended for use by children under the age of 13. TxTTone does not directly collect any personal information from any user, including children. However, third-party SDKs used in the App (Google AdMob, Firebase) may collect device identifiers and usage data per their own privacy policies. If you are a parent or guardian with concerns about your child's use of the App, please contact us at devtexttone@gmail.com.

---

## 8. Your Rights and Choices

### 8.1 Access and Correction

You can access and update your information within the App settings.

### 8.2 Data Deletion

You can delete your data by:

- Uninstalling the App (deletes all private app data; shared storage files in `Ringtones/TxTTone/` must be deleted manually)
- Contacting us at devtexttone@gmail.com
- Using Android Settings → Apps → TxTTone → Clear app data

### 8.3 Opt-Out of Ads

You can:

- Purchase the premium ad-free version of the App
- Adjust ad personalization settings on your device
- Opt-out of interest-based ads: https://www.aboutads.info/choices/

---

## 9. Data Retention

- **Local app data:** Stored on your device until you uninstall the App or clear app data
- **Ringtone copies in shared storage:** Files in `Ringtones/TxTTone/` persist until manually deleted and are not removed on uninstall
- **Per-contact ringtone assignments:** Ringtone URIs written to contacts via the `CUSTOM_RINGTONE` field persist in your Contacts database and may remain after uninstall
- **Analytics data:** Retained for 12 months then automatically deleted
- **Crash reports:** Retained for 90 days for debugging purposes

---

## 10. International Data Transfers

Your information may be transferred to and processed in countries other than your country of residence. These countries may have data protection laws different from your country. We ensure appropriate safeguards are in place to protect your information in accordance with this Privacy Policy.

---

## 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. We will notify you of changes by posting the new Privacy Policy in the App and updating the "Last Updated" date. We encourage you to review this Privacy Policy periodically.

---

## 12. California Privacy Rights (CCPA)

If you are a California resident, you have the right to know what personal information is collected, whether it is sold or disclosed, opt-out of the sale of personal information, request deletion, and not be discriminated against for exercising your privacy rights. We do not sell your personal information. To exercise these rights, contact us at devtexttone@gmail.com.

---

## 13. GDPR Rights (European Users)

If you are in the European Economic Area (EEA), you have the right to access, rectify, erase, restrict processing of, port, and object to processing of your personal data, and to withdraw consent at any time. To exercise these rights, contact us at devtexttone@gmail.com.

---

## 14. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy, please contact us:

**Email:** devtexttone@gmail.com

---

## 15. Consent

By using the App, you hereby consent to this Privacy Policy and agree to its terms.

---

*Charles Hall • TxTTone • Privacy Policy • Versio
