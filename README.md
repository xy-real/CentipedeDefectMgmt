# Mathwiz (Centipede) Defect Management Repository

## Project Information

**Project Name:** MathWiz(Centipede)
**Description:** is a secure, web-based mathematics online competition platform for Mathletes and Coaches. It is built using Next.js for the web application and Supabase (PostgreSQL) for the backend/database. The system supports competitions, problem banks, team mode, open mode, automated scoring, and integrity monitoring (e.g., tab switching logs).
**Tech Stack:**
* Next.js
* Supabase
* Tailwind CSS

**Roles:**
* Organizer
* Participant

---

## Testing Overview

**Test Period:** Q2 2026  
**Total Bugs:** 3  

### Severity Distribution
| Severity | Count | Bug IDs |
| :--- | :---: | :--- |
| **High (Severe / Usability)** | 1 | BUG-0003 |
| **Medium (Usability)** | 1 | BUG-0001 |
| **Low (Minor / UX)** | 1 | BUG-0002 |

---

## Bug Summary Table

| Bug ID | Title | Feature | Severity | Status | Related Test Case |
| :--- | :--- | :--- | :---: | :---: | :--- |
| **[BUG-0001](./BUG-0001%20No%20Preview/BUG-0001%20No%20Preview.md)** | Preview button unresponsive after creating a problem | Problem Bank | Medium | Open | PBANK-0002(partial), PBANK-0003(partial), PBANK-0005(partial) |
| **[BUG-0002](./BUG-0002%20No%20Loading%20Screen/BUG-0002%20No%20Loading%20Screen.md)** | No loading screen when navigating to competition settings | Competitions | Low | Open | COMP-0001(partial), COMP-0003(partial) |
| **[BUG-0003](./BUG-0003%20New%20Competition%20Misredirection/BUG-0003%20New%20Competition%20Misredirection.md)** | Redirected to previous competition review page upon creating a subsequent competition | Competitions | High | Open | COMP-0001(partial), COMP-0003(partial) |

---
