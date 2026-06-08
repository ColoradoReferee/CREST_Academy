# CREST Academy

**Colorado Referee Education & Supplemental Training**
*A Colorado Soccer Association Program*

**Live URL:** [coloradoreferee.github.io/CREST_Academy](https://coloradoreferee.github.io/CREST_Academy)
**Developed by:** JAReferee LLC
**Licensed to:** Colorado Soccer Association

---

## What this is

CREST Academy is the classroom toolkit for the C.R.E.S.T. (Colorado Referee Education and Supplemental Training) program — Colorado Soccer Association's in-school referee development initiative. It is designed for use by students, lead instructors, and school teachers delivering the nine-week CREST curriculum.

It runs as a single HTML file — no installation, no app store, no account required for students. It works on any device, completely offline, once loaded.

---

## The program

C.R.E.S.T. trains and certifies middle and high school students as licensed U.S. Soccer referees through a structured nine-week classroom curriculum, in partnership with Renaissance Secondary School (Denver, CO) and future partner schools.

**Program stats (2024–2026):**
- 47 students enrolled
- 45 certified — 96% completion rate
- 3 years at Renaissance Secondary School
- Every certified student walked onto a field as a licensed official within weeks of completing the course

---

## What it contains

**4-tab mobile app:**

| Tab | Contents |
|---|---|
| Journey | 9-week curriculum with progress ring, week-by-week content synced to U.S. Soccer Learning Center |
| Laws | All 17 IFAB Laws of the Game with quizzes and Jeff-eree AI coaching |
| Library | 17 reference modules from CREST Referee Resources content |
| Instructor | PIN-locked dashboard — class roster, stats, Jeff-eree on/off toggle, quick contacts |

**Library modules (17):**
First Day Guide, How Do I Get Games, Pre-Game Procedures, During the Game, Post-Game Procedures, Game Day Pocket Guide, Assignr Platform Guide, How Do I Upgrade My Grade, Getting Paid, Penalty Kick Procedure, Age Group Standards, RAP Policy, Guide to Referees, Parents of Youth Referees, Definitions & Key Terms, Signals Guide, CSA Contact Directory.

**Jeff-eree — AI Referee Coach:**
- Powered by the Anthropic Claude API
- "Ask" mode and "Test Me" (scenario) mode on every Law
- Instructor-controlled — toggled on/off from the dashboard
- Knows all 17 Laws, CSA-specific rules, 4 Moments of Soccer, 4 whistle patterns, 8 signals, RAP Penalty Matrix, age group standards, and Colorado-specific rules

---

## Instructor & administrator access

The Academy uses a PIN-based dashboard system to control access to the Instructor and Admin views. PIN values are **not published in this repository**. They are managed per-school instance via the `SCHOOL_CONFIG` block and provisioned to authorized personnel separately.

If you are an authorized instructor or administrator and need access, contact CSA at refeducation@coloradoreferees.com.

---

## School configuration

To rebrand for a new partner school, update the `SCHOOL_CONFIG` block at the top of the JavaScript with the school's name, colors, logo, city, school year, and PINs. Drop a `logo-school.png` file in the repo root and set `logoUrl` to display the school logo in the header.

The `SCHOOL_CONFIG` block is the only customization needed for a new school instance — the curriculum content, laws, library, and instructor tools are identical across all schools.

---

## About C.R.E.S.T.

C.R.E.S.T. is the Colorado Soccer Association's community outreach initiative, developed in close partnership with U.S. Soccer to integrate the Green Badge referee certification program and Referee Abuse Prevention initiatives — with the shared goal of keeping more youth involved in officiating.

The program was developed by **Deanna Duncan-Allen** (Director of Referee Operations, CSA), **Jeff Arthurholtz** (Referee Coach and Program Facilitator), and **Jessica Perkin** (Pilot Instructor, Renaissance Secondary School), with advisory support from **Esse Baharmast** (Head of Refereeing, CSA).

The centerpiece of each year is **First Game Weekend** — a day where every certified student receives one-on-one coaching from experienced national referees on the field, earns pay for their first official game, and celebrates alongside families and CSA leadership.

---

## The CREST Suite

| Tool | URL | Status |
|---|---|---|
| CREST Hub | [coloradoreferee.github.io](https://coloradoreferee.github.io) | Live |
| CREST Game Day | [coloradoreferee.github.io](https://coloradoreferee.github.io) (in hub) | Live |
| CREST Ref Coach | [coloradoreferee.github.io](https://coloradoreferee.github.io) (in hub) | Live |
| CREST Team | [coloradoreferee.github.io](https://coloradoreferee.github.io) (in hub, per-club) | Live |
| CREST Evaluator | [coloradoreferee.github.io/CREST_Evaluator](https://coloradoreferee.github.io/CREST_Evaluator) | Live — to merge into hub |
| CREST Academy | this repo | Live — to merge into hub |
| CREST Reference Library | [coloradoreferee.github.io/CREST_Reference](https://coloradoreferee.github.io/CREST_Reference) | Live — to merge into hub |

The three currently-separate CREST repos will be consolidated into the main hub repository ahead of the program's full handoff to CSA in January 2027.

---

## Architecture

- Single HTML file — no build process, no dependencies, no framework
- Deployed via GitHub Pages from the `main` branch root
- All content embedded — works offline after first load
- Student progress stored in `localStorage` — persists across sessions
- Jeff-eree requires Anthropic API access (instructor-controlled, token spend managed by instructor)
- Google Sheets sync hook built in — prompts for Sheet ID, stores in `localStorage`

---

## Status

This software is under active development as part of the CREST program. Releases deploy automatically to GitHub Pages from the `main` branch.

---

## License & Use

This software is proprietary, owned by **JAReferee LLC**, and licensed to the **Colorado Soccer Association** for use within the CREST program. See `LICENSE.txt` and `NOTICE.md` for the full terms.

Curriculum content is contributed by CSA. U.S. Soccer Learning Center content is the property of the U.S. Soccer Federation. IFAB Laws of the Game content is the property of IFAB.

Use by parties other than CSA (acting within the scope of the CREST program) requires a separate written license agreement from JAReferee LLC.

**Public visibility of source does not imply public license.**

---

## Contact

**For CREST program questions:**
- Director of Referee Operations: **Deanna Duncan-Allen** — refeducation@coloradoreferees.com — 303.888.6863
- Program Facilitator: **Jeff Arthurholtz**
- Pilot Instructor: **Jessica Perkin** — Renaissance Secondary School
- Head of Refereeing: **Esse Baharmast**
- Media: **Krissia Vasquez** — kvasquez@coloradosoccer.org

**For software licensing or development questions:**
- JAReferee LLC — https://jareferee.com — licensing@jareferee.com
- Principal: **Jeff Arthurholtz**

For partnership inquiries or to adopt the CREST program in your state association, contact the Colorado Soccer Association at ColoradoSoccer.org.

---

*Colorado Soccer Association · Colorado Referee Program · C.R.E.S.T. Referee Development*
*ColoradoSoccer.org · 2025/2026*

© 2026 JAReferee LLC. All rights reserved.
Licensed to the Colorado Soccer Association for use within the CREST program.
