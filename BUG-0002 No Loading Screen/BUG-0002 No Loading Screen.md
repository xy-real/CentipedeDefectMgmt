# Title: CP v1.0 FirstPass UI [Competitions] [Navigation]: No loading screen when navigating to competition settings

## 📝 Bug Metadata
* **Defect ID:** BUG-0002
* **Related Test Case ID:** none
* **Severity:** Low
* **Date Reported:** 2026-06-07
* **Status:** Open

## 💻 Environment Setup
* **Application Version:** v1.0.x (deployed)
* **Operating System:** Fedora Linux 42
* **Hardware:** Intel Core i5 10th Gen, NVIDIA GTX 1650
* **Network/Browser:** WiFi, Brave browser (desktop)

## 🛠️ Prerequisites
* User is logged into an Organizer account.
* There is at least one active or existing competition listed in the Problem Bank / Competitions tab.
* The site is the deployed production/staging instance.

## 🚶 Steps to Reproduce
1. Log into the system using an Organizer account.
2. Navigate to the **Competitions** tab.
3. Locate an existing competition and click the three dots (kebab menu) next to it.
4. Click the option to navigate to the competition settings page.
5. Observe the screen transition and system response during the navigation.

## 🎯 Expected Behavior
* A dedicated loading screen, spinner, or skeleton loader should appear immediately after clicking the option. This provides visual feedback to the user that the system is fetching the competition settings.

## 🐞 Actual Behavior
* There is no loading screen or visual feedback during the transition. The application directly snaps to the competition settings page (or appears unresponsive for a moment before snapping), creating a jarring and confusing experience for the user.

## 📎 Artifacts & Attachments
* **Screenshots:** * `![image.png](image.png)`
  * `![image2.png](image2.png)`
* **System Logs / Console Errors:** none

## Additional Notes
* UX improvement request: The abrupt transition can make the application feel like it's glitching. Implementing a standard loading state will make the routing feel significantly smoother.