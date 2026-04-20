TxTTone

Privacy Policy
Last Updated: April 20, 2026 • Version 1.4

Charles Hall ("we," "our," or "us") operates the TxTTone mobile application (the "App"). This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our App.

Please read this Privacy Policy carefully. By using the App, you agree to the collection and use of information in accordance with this policy. If you do not agree with the terms of this Privacy Policy, please do not use the App.

## 1. Information We Collect

### 1.1 Contact Information
We access your device's contact list to allow you to assign custom ringtones and notification sounds to specific contacts. This information is stored locally on your device and is not transmitted to our servers for this feature.

When the per-contact ringtone queue feature is enabled, TxTTone writes a ringtone URI to the standard `CUSTOM_RINGTONE` field in your device's Contacts database. This is a standard Android field read by the native dialer to play the assigned ringtone when that contact calls. No other contact data is modified for this feature. This change is made locally on your device.

### 1.2 Notification Metadata
TxTTone uses Android's Notification Access permission to detect incoming message and call notifications so it can trigger the sound rules you configure. The app processes only the notification metadata needed for this function, such as the originating app identifier and, when available from the notification itself, sender or conversation labels. It does not read, store, or transmit message bodies or notification content to our servers.

Notification processing for sound selection occurs locally on your device in real time and is not retained after processing. This section describes TxTTone's own notification handling. Separate data practices for third-party SDKs are described in Section 4.

### 1.3 Audio Files
The App allows you to select and use audio files as ringtones and notification sounds. These audio files are stored locally on your device. We do not upload your sound files to our servers for this feature.

You may also record or import custom audio clips directly within the App. These user-created or user-imported sound files are stored locally on your device in the App's private storage directory. They are not transmitted to our servers for playback functionality, shared with third parties for playback functionality, or used for any purpose other than playback within the App. You can delete these files at any time by removing them within the App or by clearing the App's data via Android Settings → Apps → TxTTone → Clear app data.

When TxTTone copies a sound file for use as a native ringtone, it stores a managed copy in `Ringtones/TxTTone/` in your device's shared storage. This folder and its contents may persist after the app is uninstalled, as Android does not automatically delete files in shared storage on uninstall. You can delete these files manually using any file manager app.

### 1.4 System Settings and Ringtone Staging
When the Custom Ringtones feature is enabled by the user, TxTTone may use call-state, contacts, and system-setting access to prepare or restore ringtone behavior as follows:

- **Ringtone suppression for text tones:** TxTTone briefly suppresses the system notification sound while a custom text tone is starting, so your selected sound can play cleanly. Your system default ringtone is not changed by this process.
- **Per-contact ringtone staging:** TxTTone writes the contact's assigned ringtone URI to that contact's `CUSTOM_RINGTONE` field in your Contacts database so the native dialer can play it when that person calls.
- **Global native ringtone randomization:** When this optional feature is enabled, TxTTone stages the current selected ringtone for eligible enrolled contacts by updating their `CUSTOM_RINGTONE` field ahead of incoming calls. TxTTone is designed to preserve your actual system default ringtone as your fallback ringtone rather than replace it with a TxTTone-managed sound.
- **Restore behavior:** If TxTTone temporarily restores or re-applies your fallback ringtone for compatibility or recovery purposes, those changes are made locally on your device and can be reversed by disabling the feature or using the Restore option in Settings.

All ringtone staging and system-setting changes described here are performed locally on your device.

### 1.5 Usage and Diagnostic Data
TxTTone itself performs core sound personalization locally on your device. However, third-party SDKs integrated into the App may collect certain data on our behalf, including:

- **Crash reports and error logs** — via Firebase Crashlytics (such as stack traces, app state, and device information for debugging)
- **App usage statistics and analytics** — via Firebase Analytics
- **Advertising-related data** — via Google AdMob, which may process identifiers, IP address, and usage information for ads

These SDKs operate under their own privacy policies, linked in Section 4.

## 2. How We Use Your Information
We use the collected information for the following purposes:

- **To provide and maintain the App:** Enable core functionality including contact-based sound assignments, app-based sound rules, and call-related ringtone behavior
- **To improve user experience:** Analyze usage patterns to enhance features and performance
- **To fix bugs and crashes:** Use crash reports to identify and resolve technical issues
- **To display advertisements:** Show ads in the free version of the App
- **To process purchases:** Handle in-app purchases for the ad-free version
- **To communicate with you:** Respond to support requests and send important updates
- **To comply with legal obligations:** Meet legal and regulatory requirements

## 3. Data Storage

### 3.1 Local Storage
Contact associations, audio selections, ringtone assignments, and app settings are stored locally on your device. This feature data is not transmitted to our servers.

### 3.2 Backup
TxTTone includes an optional local backup feature that exports your settings and sound library to a zip file on your device. This backup file is stored wherever you choose to save it on your device or cloud storage of your choice. We do not operate any cloud backup service. The backup file contains sound files and app settings only. It does not include notification bodies or message content.

### 3.3 Security Measures
We implement appropriate technical measures to protect your information. Third-party SDKs (such as AdMob and Firebase) may use encrypted transmission (such as HTTPS) when sending data. No method of electronic storage or transmission is 100% secure, and we cannot guarantee absolute security.

## 4. Third-Party Services

### 4.1 Advertising
We use Google AdMob to display advertisements in the free version of the App. AdMob may collect device identifiers, IP address, and usage data. AdMob Privacy Policy: https://policies.google.com/privacy

### 4.2 Analytics
We use Firebase Analytics to understand app usage and improve our services. Firebase may collect app usage data, device information, and crash-related data. Firebase Privacy Policy: https://firebase.google.com/support/privacy

### 4.3 Crash Reporting
We use Firebase Crashlytics to collect crash reports and diagnostic information. Crashlytics may collect device state information, stack traces, and app logs. Crash reports are not intended to include notification bodies or message content.

### 4.4 In-App Purchases
We use Google Play Billing to process in-app purchases. Google handles payment processing and may collect payment information. Google Play Terms of Service: https://play.google.com/about/play-terms/

## 5. Permissions
The App requires or may request the following permissions:

- **BIND_NOTIFICATION_LISTENER_SERVICE:** To detect incoming message and call notifications so custom sounds can be played at the right moment
- **READ_CONTACTS:** To access your contact list for assigning custom sounds to specific contacts
- **WRITE_CONTACTS:** To write a custom ringtone URI to the per-contact ringtone field in your Contacts database when features that depend on contact ringtone staging are used
- **READ_PHONE_STATE:** To detect incoming call state so TxTTone knows when to prepare, play, or stop custom ringtone behavior. TxTTone does not read call logs, record calls, or access call content
- **WRITE_SETTINGS:** To restore or maintain fallback ringtone behavior and support ringtone-related system setting flows when enabled by the user
- **READ_EXTERNAL_STORAGE / READ_MEDIA_AUDIO:** To access audio files on your device for use as custom sounds
- **POST_NOTIFICATIONS:** To post notifications on Android 13 and above
- **INTERNET:** To support ads, billing, and analytics/crash reporting services
- **ACCESS_NETWORK_STATE:** To determine network connectivity for supported services
- **ROLE_CALL_SCREENING (optional):** If granted, gives TxTTone earlier notice of incoming calls for more reliable ringtone handling. This role is optional and can be skipped or revoked at any time

You can manage these permissions in your device settings at any time.

## 6. Data Sharing and Disclosure
We do not sell, trade, or rent your personal information to third parties. We may share information in the following circumstances:

### 6.1 With Your Consent
We may share information when you explicitly give us permission to do so.

### 6.2 Service Providers
We may share information with third-party service providers who perform services on our behalf, such as analytics, advertising, crash reporting, and billing support.

### 6.3 Legal Requirements
We may disclose your information if required to do so by law or in response to valid requests by public authorities.

### 6.4 Business Transfers
If we are involved in a merger, acquisition, or sale of assets, your information may be transferred. We will provide notice before your information is transferred and becomes subject to a different Privacy Policy.

## 7. Children's Privacy
The App is not intended for use by children under the age of 13. TxTTone does not intentionally collect personal information directly from children for its core local personalization features. However, third-party SDKs used in the App (such as Google AdMob and Firebase) may collect device identifiers and usage data under their own privacy policies. If you are a parent or guardian with concerns about your child's use of the App, please contact us at devtexttone@gmail.com.

## 8. Your Rights and Choices

### 8.1 Access and Correction
You can access and update relevant in-app information within the App settings.

### 8.2 Data Deletion
You can delete your data by:

- Uninstalling the App (this deletes private app data; shared storage files in `Ringtones/TxTTone/` may need to be deleted manually)
- Contacting us at devtexttone@gmail.com
- Using Android Settings → Apps → TxTTone → Clear app data

### 8.3 Opt-Out of Ads
You can:

- Purchase the ad-free version of the App
- Adjust ad personalization settings on your device
- Opt out of interest-based ads: https://www.aboutads.info/choices/

## 9. Data Retention
- **Local app data:** Stored on your device until you uninstall the App or clear app data
- **Ringtone copies in shared storage:** Files in `Ringtones/TxTTone/` persist until manually deleted and are not removed automatically on uninstall
- **Per-contact ringtone assignments:** Ringtone URIs written to contacts via the `CUSTOM_RINGTONE` field may remain in your Contacts database after uninstall until you change or clear them
- **Analytics data:** Retained according to the settings and policies of the analytics provider
- **Crash reports:** Retained according to the settings and policies of the crash-reporting provider

## 10. International Data Transfers
Your information may be transferred to and processed in countries other than your country of residence by third-party service providers. These countries may have data protection laws different from your country. We rely on those providers' applicable safeguards and contractual protections where required.

## 11. Changes to This Privacy Policy
We may update this Privacy Policy from time to time. We will notify users of material changes by posting the updated Privacy Policy in the App and revising the "Last Updated" date. We encourage you to review this Privacy Policy periodically.

## 12. California Privacy Rights (CCPA/CPRA)
If you are a California resident, you may have rights to know what personal information is collected, whether it is sold or disclosed, request deletion, correct certain information, and not be discriminated against for exercising your privacy rights, subject to applicable law. We do not sell your personal information. To exercise these rights, contact us at devtexttone@gmail.com.

## 13. GDPR / EEA Rights
If you are in the European Economic Area (EEA), United Kingdom, or Switzerland, you may have rights to access, rectify, erase, restrict processing of, port, and object to processing of your personal data, and to withdraw consent where processing is based on consent. To exercise these rights, contact us at devtexttone@gmail.com.

## 14. Contact Us
If you have any questions, concerns, or requests regarding this Privacy Policy, please contact us:

Email: devtexttone@gmail.com

## 15. Consent
By using the App, you consent to this Privacy Policy and agree to its terms.

*Charles Hall • TxTTone • Privacy Policy • Version 1.4*
