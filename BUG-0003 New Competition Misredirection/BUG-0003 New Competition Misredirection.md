# Title: CP v1.0 FirstPass UI [Competitions] [Creation]: Redirected to previous competition review page upon creating a subsequent competition

## 📝 Bug Metadata
* **Defect ID:** BUG-0003
* **Related Test Case ID:** none
* **Severity:** High
* **Date Reported:** 2026-06-07
* **Status:** Open

## 💻 Environment Setup
* **Application Version:** v1.0.x (deployed)
* **Operating System:** Fedora Linux 42
* **Hardware:** Intel Core i5 10th Gen, NVIDIA GTX 1650
* **Network/Browser:** WiFi, Brave browser (desktop)

## 🛠️ Prerequisites
* User is logged into an Organizer account.
* The site is the deployed production/staging instance.

## 🚶 Steps to Reproduce
1. Log into the system and navigate to the **Competitions** tab.
2. Click the button to create a new competition (Competition A).
3. Fill out the necessary details and successfully submit/save Competition A.
4. Navigate back to the main **Competitions** tab.
5. Click the button to create a second new competition (Competition B).
6. Fill out the necessary details and submit/save Competition B.
7. Observe the page redirection after submission.

## 🎯 Expected Behavior
* After successfully creating the second competition, the system should redirect the user to the review/settings page specifically for that newly created competition (Competition B). 

## 🐞 Actual Behavior
* The system redirects the user to the review page of the *first* competition (Competition A) instead of the new one. 

## 📎 Artifacts & Attachments
* **Screenshots:** * `![image.png](image.png)`
  * `![image2.png](image2.png)`
* **System Logs / Console Errors:** none

## Additional Notes
* This appears to be a state management issue. The frontend is likely holding onto the ID of the first created competition in its global state or cache and failing to clear/reset it when the "Create Competition" flow is triggered a second time.