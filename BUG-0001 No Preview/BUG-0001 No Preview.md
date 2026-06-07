# Title: CP v1.0 FirstPass UI [Problem Bank] [Preview]: Preview button unresponsive after creating a problem

## 📝 Bug Metadata
* **Defect ID:** BUG-0001
* **Related Test Case ID:** PBANK-0002(partial), PBANK-0003(partial), PBANK-0005(partial)
* **Date Reported:** 2026-06-07
* **Status:** Open

## 💻 Environment Setup
* **Application Version:** v1.0.x (deployed)
* **Operating System:** Linux
* **Hardware:** Intel Core i5 10th Gen, NVIDIA GTX 1650
* **Network/Browser:** WiFi, Brave browser (desktop)

## 🛠️ Prerequisites
* User is logged in and has permission to add problems to the Problem Bank.
* The site is the deployed production/staging instance (not a local dev server).

## 🚶 Steps to Reproduce
1. Navigate to the Problem Bank page.
2. Click Add Problem (create a new problem entry).
3. Fill in the required fields for the new problem (title, description, any required metadata).
4. After saving/creating the problem entry, press the Preview button to view how the problem will render.

## 🎯 Expected Behavior
* Pressing the Preview button should open a preview of the problem (modal or separate view) showing the rendered content exactly as it will appear to end users.

## 🐞 Actual Behavior
* After creating the problem, the Preview button cannot be pressed / is unresponsive — no preview is shown. The button appears unclickable or clicking it produces no effect.

## 📎 Artifacts & Attachments
* **Screenshots:** [image.png](image.png)
* **System Logs / Console Errors:** none

## Additional Notes
* Browser: Brave on WiFi. Site is already deployed (production/staging).
* Please verify whether the Preview feature relies on a client-side script that may be blocked by Brave shields or an ad/privacy extension. Try disabling shields for the site and reproduce.
* If possible, check the browser console for errors when clicking Preview and include logs here.
