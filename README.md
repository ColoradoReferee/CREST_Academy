[README_Academy.md](https://github.com/user-attachments/files/27167484/README_Academy.md)
# CREST Academy
**Colorado Referee Education & Supplemental Training**
*A Colorado Soccer Association Program*

[![Live](https://img.shields.io/badge/status-live-brightgreen)](https://coloradoreferee.github.io/CREST_Academy)
[![Free](https://img.shields.io/badge/cost-free-blue)](https://coloradoreferee.github.io/CREST_Academy)
[![Offline](https://img.shields.io/badge/works-offline-orange)](https://coloradoreferee.github.io/CREST_Academy)

**Live URL:** [coloradoreferee.github.io/CREST_Academy](https://coloradoreferee.github.io/CREST_Academy)

---

## What Is This

CREST Academy is the classroom toolkit for the C.R.E.S.T. (Colorado Referee Education and Supplemental Training) program — Colorado Soccer Association's in-school referee development initiative. It is designed for use by students, lead instructors, and school teachers delivering the nine-week CREST curriculum.

It runs as a single HTML file — no installation, no app store, no account required for students. It works on any device, completely offline, once loaded.

---

## The Program

C.R.E.S.T. trains and certifies middle and high school students as licensed U.S. Soccer Grassroots referees through a structured nine-week classroom curriculum, in partnership with Renaissance Secondary School (Denver, CO) and future partner schools.

**Program stats (2024–2026):**
- 47 students enrolled
- 45 certified — 96% completion rate
- 3 years at Renaissance Secondary School
- Every certified student walked onto a field as a licensed official within weeks of completing the course

---

## What It Contains

**4-tab mobile app:**

| Tab | Contents |
|---|---|
| 📖 Journey | 9-week curriculum with progress ring, week-by-week content synced to U.S. Soccer Learning Center |
| ⚖️ Laws | All 17 IFAB Laws of the Game with quizzes and Jeff-eree AI coaching |
| 🗂️ Library | 17 reference modules from Deanna's CREST Referee Resources content |
| 🏫 Instructor | PIN-locked dashboard — class roster, stats, Jeff-eree on/off toggle, quick contacts |

**Library modules (17):**
First Day Guide, How Do I Get Games, Pre-Game Procedures, During the Game, Post-Game Procedures, Game Day Pocket Guide, Assignr Platform Guide, How Do I Upgrade My Grade, Getting Paid, Penalty Kick Procedure, Age Group Standards, RAP Policy, CSA Guide to Referees, Parents of Youth Referees, Definitions & Key Terms, Signals Guide, CSA Contact Directory

**Jeff-eree — AI Referee Coach:**
- Powered by Anthropic Claude API
- Ask mode and Test Me (scenario) mode on every Law
- Instructor-controlled — toggled on/off from the dashboard
- Knows all 17 Laws, CSA-specific rules, 4 Moments of Soccer, 4 whistle patterns, 8 signals, RAP Penalty Matrix, age group standards, and every Colorado-specific rule

---

## PIN System

| PIN | Access Level |
|---|---|
| `5280` | Lead Instructor — change per class in `SCHOOL_CONFIG` |
| `5555` | God Mode (CSA Admin) — works on any school instance |

---

## School Configuration

To rebrand for a new partner school, update 6 lines at the top of the JavaScript:

```javascript
const SCHOOL_CONFIG = {
  name: "Renaissance Secondary School",
  shortName: "Renaissance",
  primaryColor: "#1B2F55",
  secondaryColor: "#C8921A",
  logoUrl: null,           // set to 'logo-school.png' when available
  city: "Denver, CO",
  instructorPin: "5280",   // change per class
  adminPin: "5555",        // CSA admin — do not change
  schoolYear: "2025-2026"
};
```

Drop a `logo-school.png` file in the repo root and set `logoUrl` to display the school logo in the header.

---

## About C.R.E.S.T.

C.R.E.S.T. is Colorado Soccer Association's community outreach initiative, developed in close partnership with U.S. Soccer to integrate the Green Badge referee certification program and Referee Abuse Prevention initiatives — with the shared goal of keeping more youth involved in officiating.

The program was developed by **Jeff Arthurholtz** (Referee Coach and Program Facilitator), **Deanna Duncan-Allen** (Director of Referee Operations), and **Jessica Perkin** (Pilot Instructor, Renaissance Secondary School), with advisory support from **Esse Baharmast** (CSA Director of Referees, FIFA Instructor).

The centerpiece of each year is **First Game Weekend** — a day where every certified student receives one-on-one coaching from experienced national referees on the field, earns pay for their first official game, and celebrates alongside families and CSA leadership.

---

## The CREST Suite

| Tool | URL | Status |
|---|---|---|
| CREST Hub | [coloradoreferee.github.io](https://coloradoreferee.github.io) | ✅ Live |
| CREST Evaluator | [coloradoreferee.github.io/CREST_Evaluator](https://coloradoreferee.github.io/CREST_Evaluator) | ✅ Live |
| CREST Academy | [coloradoreferee.github.io/CREST_Academy](https://coloradoreferee.github.io/CREST_Academy) | ✅ Live |
| CREST Reference Library | [coloradoreferee.github.io/CREST_Reference](https://coloradoreferee.github.io/CREST_Reference) | ✅ Live |
| CREST Team | Coming Soon | 🔜 Planned |
| CREST Game Day | Coming Soon | 🔜 Planned |

---

## Key Contacts

| Role | Contact |
|---|---|
| Director of Referee Operations | Deanna Duncan-Allen — refeducation@coloradoreferees.com — 303.888.6863 |
| Program Facilitator | Jeff Arthurholtz |
| Pilot Instructor | Jessica Perkin — Renaissance Secondary School |
| Head of Refereeing / CSA Director of Referees | Esse Baharmast |
| Media Contact | Krissia Vasquez — kvasquez@coloradosoccer.org |

---

## Technical Notes

- Single HTML file — no build process, no dependencies, no framework
- Deployed via GitHub Pages from the `main` branch root
- All content embedded — works offline after first load
- Student progress stored in `localStorage` — persists across sessions
- Jeff-eree requires Anthropic API access (instructor-controlled, token spend managed by instructor)
- Google Sheets sync hook built in — prompts for Sheet ID, stores in `localStorage`

---

## License & Use

Developed by Colorado Soccer Association. Curriculum content from the U.S. Soccer Learning Center and CREST Referee Resources, authored by Deanna Duncan-Allen, Director of Referee Operations.

U.S. Soccer Laws of the Game content © IFAB. All rights reserved.

For partnership inquiries or to adopt the CREST program in your state association, contact Colorado Soccer Association at ColoradoSoccer.org.

---

*Colorado Soccer Association · Colorado Referee Program · C.R.E.S.T. Referee Development*
*ColoradoSoccer.org · 2025/2026*
