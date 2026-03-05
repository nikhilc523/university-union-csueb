Below is the **screen-by-screen UI architecture** you can build in Figma for a **premium iOS “University Union Hub”** experience (North + South only), using a **black + CSUEB red** system and a layout that can surface *every* UU detail without making Home feel cluttered.

Everything “tiny” is placed intentionally: **Home = time-sensitive**, **Explore = the full UU encyclopedia**, **Book = policy + routing**, **More = operations & governance**.

---

## 0) Figma file structure (so it feels Apple-level, not random)

Create one Figma file with these pages:

1. **00 – Foundations (Tokens)**

   * Color styles, type, spacing, radius, shadows, blur
2. **01 – Components**

   * Nav bar, tab bar, cards, list rows, chips, callouts, empty states
3. **02 – Patterns**

   * Search pattern, filter sheet, detail template, booking wizard template
4. **10 – App Screens (Hi-Fi)**

   * Frames in order of the user journey
5. **90 – Content Map**

   * A master “inventory” of every UU item and where it appears

---

## 1) Design language (premium iOS, black + red)

### Colors (Figma styles)

* **CSUEB Black / Background**: #0B0B0D (use for full-screen base)
* **Surface 1**: #121216 (cards)
* **Surface 2**: #1A1A21 (raised cards / sheets)
* **Hairline**: white @ 10–14% opacity
* **Text Primary**: #FFFFFF
* **Text Secondary**: white @ 70%
* **Text Tertiary**: white @ 45%
* **CSUEB Red / Accent**: “Brand Red” token (use for primary CTA, chips, highlights)
* **Status**: Green/Yellow/Red for “Open / Closing Soon / Closed” pills

### Type

* **SF Pro** (iOS default)
* Large Title for tab roots
* Title 3 for section headers
* Body for list rows
* Footnote for policies + “tiny details”

### iOS feel

* Bottom **Tab Bar**
* **Large Title + Search** on Explore
* **Sheets** for filters
* **Cards** for “UU Today”
* “Quiet” UI: minimal borders, strong spacing, subtle shadows

---

## 2) Navigation map (tabs + what lives where)

**Tab bar (5):**

1. **Today**
2. **Explore**
3. **Events**
4. **Book**
5. **More**

This lets you surface *everything* without bloating a single screen.

---

## 3) Content model (how we can show “every tiny info” cleanly)

Everything in the app becomes one of these objects:

### A) Place

Example: “QUSSC”, “SLIC”, “Black Student Success Center”, “ASI Offices”

Fields:

* Building: North (Old) / South (New)
* Floor: 1 / 2 / 3
* Category: Center / Office / Service / Amenity / Dining / Room / Outdoor
* Short description (1–2 lines)
* Hours (if available)
* Contact (email/phone if available)
* Rules (if relevant)
* Links (website / booking / 3D tour)

### B) Reservable Space

Example: Bayview Room, MPR, MPR A/B, UU311

* Capacities by layout
* Equipment available
* Setup/clearing time policy
* Restrictions (no confetti, etc.)
* Booking route (25Live / BaySync / external form)
  This is pulled directly from UU room pages + policies. ([California State University, East Bay][1])

### C) Policy / Rule

Example: cancellation rules, insurance requirements, GameZone rules, smoke-free
Policies should be viewable as “cards” with short summaries + “Read full details”.

---

## 4) Screen-by-screen plan (what each screen contains)

### 4.1 Onboarding (3 screens)

**Screen O1 — Welcome**

* “University Union Hub”
* Two building chips: North + South (just visual, not required)
* CTA: “Continue”

**Screen O2 — Choose your role**

* Student
* Faculty/Staff
* Guest/External
  This role only affects booking routing (Book tab). ([California State University, East Bay][2])

**Screen O3 — Preferences**

* Toggle: “Notify me about UU events”
* Toggle: “GameZone tournaments”
* Toggle: “Dining links”
* Toggle: “Booking reminders”

---

## 4.2 TODAY tab (time-sensitive, not encyclopedic)

**Screen T1 — Today (Home)**
Top (hero strip):

* **Open/Closed** status with hours
* “North UU • South UU”
* Address quick action + “Parking info” quick action ([California State University, East Bay][3])

Section 1 — “What’s happening today”

* Card stack (pull from Events tab; even if empty, show “No featured events”)
  Important: the UU Events webpage is currently “digital dust”, so this area needs an app-native feed later. ([California State University, East Bay][4])

Section 2 — “Quick actions”

* Explore North
* Explore South
* Book a space
* GameZone
* Dining

Section 3 — “UU Essentials (tiny but useful)”
Small icon row:

* **Charging stations available** (tappable → details screen)
* **Water refill**
* **Microwave station**
* **Printer stations** ([California State University, East Bay][5])

> Strategy: Today shows only “what changes today,” and pushes the “everything” inventory into Explore.

---

## 4.3 EXPLORE tab (the UU encyclopedia)

This is where you satisfy the requirement: **every UU detail exists as a searchable item**.

**Screen E1 — Explore (Search-first)**

* Large title: “Explore”
* Search: “MPR”, “Bayview”, “QUSSC”, “GameCave”, “UU311”
* Building segmented control: **North / South / All**
* Filters sheet:

  * Floor (North: 1/2/3, South: 1/2)
  * Category (Dining, Centers, Rooms, Amenities, Offices, Outdoor)

**Screen E2 — Explore results (Directory list)**
Each row shows:

* Name
* “South • Floor 1” chip
* Category icon
* Optional: “Reservable” or “Open now”

**Screen E3 — Place detail template**
Header:

* Title
* Chips: Building + Floor + Category
* “Save” + “Share”

Body modules (only show what exists for that place):

1. “About”
2. “Where in the UU”
3. “Hours” (if known)
4. “Contact” (if known)
5. “Related”
6. “Policies” (if relevant)

---

### 4.3.1 Full content inventory (this is what Explore MUST include)

Build these as directory entries.

#### NORTH University Union (Old UU) — Floor 1 ([California State University, East Bay][5])

* Access to West Loop road
* **UU102 OFFLINE → Wellbeing Suite coming soon** (special status badge) ([California State University, East Bay][6])
* Water fountain / water bottle refill station
* Chartwells offices
* Staircase access
* Elevator access
* Restrooms

#### NORTH — Floor 2 ([California State University, East Bay][5])

* Study/lounge areas
* Printer station
* Charging station (**North: one on 2nd floor**) ([California State University, East Bay][7])
* Game Room
* GameCave
* Dining area:

  * Fry Shack
  * Taco Bell Express
  * Wild Blue
  * Market
* Black Student Success Center
* Staircase access
* Elevator access
* Restrooms

#### NORTH — Floor 3 ([California State University, East Bay][5])

* Study/lounge areas
* Balcony
* UU311 (reservable)
* UU307ABC – ASI Board Offices
* ASI Offices
* Charging station (**North: one on 3rd floor**) ([California State University, East Bay][7])
* Staircase access
* Elevator access
* Restrooms

---

#### SOUTH University Union (New UU) — Floor 1 ([California State University, East Bay][8])

* Dining room area
* Microwave station
* Vending machines
* Panda Express
* Halal Bites of Chicago
* DISARC
* QUSSC
* Charging station (**South: one on 1st floor**) ([California State University, East Bay][7])
* Bulletin board (turn into “Digital Bulletin” feature later)
* UU Customer Service / Operations Assistant Desk
* Water fountain / water bottle refill station
* Multipurpose Room (MPR)
* Outdoor Stage / UU/MI lawn access
* Staircase access
* Elevator access
* Restrooms

#### SOUTH — Floor 2 ([California State University, East Bay][8])

* Bayview Room (reservable)
* SLIC (Student Leadership and Involvement Center)
* Study/lounge areas
* Printer station
* The Gallery (Room 2010) (reservable)
* Asian Pacific Islander Student Resource Center (API)
* Undocumented Student Resource Center (USRC)
* Latinx Student Resource Center
* DISARC + Student Resource Center Administrative Office
* Charging station (**South: one on 2nd floor**) ([California State University, East Bay][7])
* Staircase access
* Elevator access
* Restrooms

---

### 4.3.2 “UU Essentials” detail screens (tiny info deserves its own place)

**Screen E4 — Essentials**
A grouped list:

* Charging Stations (counts + where) ([California State University, East Bay][7])
* Hand sanitizer stations (near elevators) ([California State University, East Bay][7])
* Cleaning schedule (public areas cleaned several times; rooms after events) ([California State University, East Bay][7])
* Daily parking permits ($10/day; where to buy; parking contact) ([California State University, East Bay][7])
* Smoke & tobacco-free campus note ([California State University, East Bay][7])
* Open flame restrictions (no candles, sparklers, etc.) ([California State University, East Bay][7])
* Special accommodations guidance (Accessibility Services + UU desk) ([California State University, East Bay][7])

---

## 4.4 EVENTS tab (single source of truth)

Because the UU Events page is currently a placeholder, the app should treat **Events as an internal feed** long-term. ([California State University, East Bay][4])

**Screen V1 — Events**
Top filter row:

* Today / This week / This month
* Location: North / South / Both
* Type: UU / GameZone / Student Orgs / Dining

**Section: Featured**

* 3 large cards

**Section: All events**

* List rows

**Screen V2 — Event detail**

* Title + location chip (“North UU • Room 311”)
* Date/time
* “Add to calendar”
* “Share”
* “How to attend” (check-in, RSVP link, etc.)

**Seed content source you can show immediately: GameZone Events**
Their page includes tournaments/leagues and even references RSVP tooling (“Download FusionPlay to RSVP”). ([California State University, East Bay][9])

---

## 4.5 BOOK tab (wizard: routes to the right system, shows all rules)

This tab is where you surface the “policy + pricing + insurance + lead times” without scaring casual users elsewhere.

**Screen B1 — Book**
2 big tiles:

* **Book a Room / Space**
* **GameZone Services (rules + how reservations work)**

**Screen B2 — What are you booking?**
Options:

* Meeting room (UU311, Bayview, Gallery)
* Event space (MPR, MPR A, MPR B)
* Outdoor (Stage/lawn) → routed inquiry (if applicable)

**Screen B3 — Who are you?**

* Student org (BaySync path) ([California State University, East Bay][2])
* Faculty/Staff (25Live path) ([California State University, East Bay][10])
* Guest/External (external request form path) ([California State University, East Bay][10])

**Screen B4 — Policies that matter (smart checklist)**
Show as “I understand” chips:

* **Cancellation rule** (email by 9am two business days prior; fees possible) ([California State University, East Bay][2])
* **Insurance** (COI due 10 working days before; Risk Management contact exists) ([California State University, East Bay][2])
* **Decorations** (no confetti/glitter; painters tape only; etc.) ([California State University, East Bay][7])
* **Clearing room** (30 minutes before/after) ([California State University, East Bay][1])

**Screen B5 — Pricing preview (transparent, not overwhelming)**
Show a “common fees” card:

* Chairs $5
* Rectangle tables $12
* Round tables $15
* Projector/screen $45
* Laptop $30
* PA system $45
* “Other fees”: admin 5%, no-call/no-show $100, policy violation $100, late cancellation $50 ([California State University, East Bay][11])

Also show the **45-day lead time** callout for stage/dance floor requests due to Fire Marshal review. ([California State University, East Bay][11])

**Screen B6 — Route out (final step)**

* Button: “Continue to Request Form”
* Under it: “What happens next” (confirmation email timing, tentative vs confirmed) ([California State University, East Bay][2])

---

## 4.6 GAMEZONE (as a featured “module” reachable from Today/Explore)

GameZone is content-rich; give it a mini-hub.

**Screen G1 — GameZone hub**
Tiles:

* GameRoom
* GameCave
* Board Games Catalog
* Tournaments & Events
* Rules

**Screen G2 — GameRoom**

* “Free to use” messaging
* What’s inside: 3 billiards tables, air hockey, foosball, board/card games
* Checkout rules: equipment at service desk with Baycard ([California State University, East Bay][12])

**Screen G3 — GameCave**

* Equipment list: five 50" HDTVs, PS4/PS5, Xbox One/360, VR station
* Seating: gamer rocking chairs
* “Retro games seasonally” note ([California State University, East Bay][13])

**Screen G4 — Board Games Catalog**

* Search field + A–Z list (use the published list) ([California State University, East Bay][14])

**Screen G5 — GameZone Rules**
Must include:

* Food/drink restrictions (sealed container) ([California State University, East Bay][15])
* 60-minute reservation norm + 10-minute cooldown ([California State University, East Bay][15])
* No concurrent/back-to-back bookings ([California State University, East Bay][15])
* Billiards specifics: red table 30 mins; green/blue 60; no jump shots; no table-hop; no gambling ([California State University, East Bay][15])
* Conduct + equipment return consequences ([California State University, East Bay][15])

---

## 4.7 MORE tab (operations, hours, staff, about, resources)

**Screen M1 — More**
List groups:

* Hours & Location
* Staff directory
* About UU
* Policies & Resources
* Feedback / Survey

**Screen M2 — Hours & Location**
This should match the official Hours page:

* Spring Term 2026 hours
* Holiday closures
* Spring recess modified hours
* Address + driving directions + campus map + parking info ([California State University, East Bay][3])

**Important note (design decision):**
There’s a mismatch between the reservation policies hours (includes weekend hours) and the Hours page (weekends closed for Spring 2026). Your app should treat **Hours & Location** as the “source of truth,” and label other hours as “reservation policy defaults.” ([California State University, East Bay][3])

**Screen M3 — Staff Directory**
Cards with:

* Name
* Role
* Tap to email / call
  Use published staff contacts. ([California State University, East Bay][16])

**Screen M4 — About UU**

* Mission-style copy (“living room and hub…”) ([California State University, East Bay][17])
* “Union Stats” section:

  * 2 buildings
  * North: 58,000 sq ft, opened 1985
  * South: 29,000 sq ft, opened 2007
  * What’s located there (ASI, Student Life Leadership Programs, centers, etc.) ([California State University, East Bay][18])

**Screen M5 — Resources**
Quick links style (in-app summaries):

* Title IX
* University Scheduling
* Smoke & Tobacco-Free policy note ([California State University, East Bay][7])

**Screen M6 — Feedback (Survey)**

* The 15-second micro-survey you drafted
* * “Report incorrect info” (directory hygiene)

---

## 5) Reservable room detail screens (these are “premium” pages)

For each reservable room, create a consistent template:

**Template modules**

1. Hero image / 3D tour CTA
2. Capacity by setup
3. Equipment available
4. Scheduling steps
5. Rules (decorations, clearing room)
6. Book CTA (routes to wizard)

### Rooms to build:

* **UU311** ([California State University, East Bay][19])
* **Bayview Room** ([California State University, East Bay][20])
* **MPR** (plus A & B as separate capacity/gear pages) ([California State University, East Bay][1])
* **MPR A** (the most detailed: capacities + “no confetti/glitter/paint/candles”, blue tape only, etc.) ([California State University, East Bay][1])
* **MPR B** ([California State University, East Bay][21])
* **The Gallery** ([California State University, East Bay][22])
* **Room 102 OFFLINE** (status page: closed, planned Wellbeing Suite) ([California State University, East Bay][6])

---

## 6) What you should mock up first (the “money screens”)

If you want the cleanest pitch deck + wow factor, do these first in hi-fi:

1. **Today (T1)**
2. **Explore (E1 + E3 detail)**
3. **Book Wizard (B1 → B6)**
4. **Room Detail: MPR A (because it’s packed with real rules + capacity)**
5. **GameZone hub + Rules screen**
6. **Hours & Location**

---

## 7) If you want, I can generate the hi-fi “fake screenshots” next

If you say “generate 6 screens,” I’ll produce **6 premium iPhone mockup images** (black + red, iOS style) for:

* Today
* Explore
* Place Detail (QUSSC example)
* Book Wizard
* MPR A Detail
* GameZone Hub

You can drop them straight into Figma as the visual baseline.

[1]: https://www.csueastbay.edu/uu/meeting-rooms/new-uu/mpr-a.html "https://www.csueastbay.edu/uu/meeting-rooms/new-uu/mpr-a.html"
[2]: https://www.csueastbay.edu/uu/reservations/policies.html "https://www.csueastbay.edu/uu/reservations/policies.html"
[3]: https://www.csueastbay.edu/uu/about-us/hours.html "
            Hours and Location
        "
[4]: https://www.csueastbay.edu/uu/reservations/events.html "https://www.csueastbay.edu/uu/reservations/events.html"
[5]: https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html "https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html"
[6]: https://www.csueastbay.edu/uu/meeting-rooms/old-uu/room-102.html "https://www.csueastbay.edu/uu/meeting-rooms/old-uu/room-102.html"
[7]: https://www.csueastbay.edu/uu/files/docs/uu-reservation-policies-and-procedures-guide.pdf "University Union Reservation Procedure Guide"
[8]: https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html "https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html"
[9]: https://www.csueastbay.edu/uu/gamezone/events.html "https://www.csueastbay.edu/uu/gamezone/events.html"
[10]: https://www.csueastbay.edu/uu/reservations/index.html "https://www.csueastbay.edu/uu/reservations/index.html"
[11]: https://www.csueastbay.edu/uu/reservations/pricing.html "https://www.csueastbay.edu/uu/reservations/pricing.html"
[12]: https://www.csueastbay.edu/uu/gamezone/gameroom.html "https://www.csueastbay.edu/uu/gamezone/gameroom.html"
[13]: https://www.csueastbay.edu/uu/gamezone/gamecave.html "https://www.csueastbay.edu/uu/gamezone/gamecave.html"
[14]: https://www.csueastbay.edu/uu/gamezone/board-games.html "https://www.csueastbay.edu/uu/gamezone/board-games.html"
[15]: https://www.csueastbay.edu/uu/gamezone/policies.html "https://www.csueastbay.edu/uu/gamezone/policies.html"
[16]: https://www.csueastbay.edu/uu/about-us/staff.html "https://www.csueastbay.edu/uu/about-us/staff.html"
[17]: https://www.csueastbay.edu/uu/about-us/about.html "
            About University Union
        "
[18]: https://www.csueastbay.edu/uu/about-us/university-stats.html "
            University Union Stats
        "
[19]: https://www.csueastbay.edu/uu/meeting-rooms/old-uu/room-311.html "https://www.csueastbay.edu/uu/meeting-rooms/old-uu/room-311.html"
[20]: https://www.csueastbay.edu/uu/meeting-rooms/new-uu/bayview-room.html "https://www.csueastbay.edu/uu/meeting-rooms/new-uu/bayview-room.html"
[21]: https://www.csueastbay.edu/uu/meeting-rooms/new-uu/mpr-b.html "https://www.csueastbay.edu/uu/meeting-rooms/new-uu/mpr-b.html"
[22]: https://www.csueastbay.edu/uu/meeting-rooms/new-uu/the-gallery.html "https://www.csueastbay.edu/uu/meeting-rooms/new-uu/the-gallery.html"
