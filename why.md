**Research + Feature Plan (Web Asset Audit → App Surface Map → Booking Integrations)**

**Scope:** University Union only (North + South).

**Explicit non-goal:** This is **not** the campus indoor navigation project.

---

## 1) Why this app (problem → opportunity)

CSUEB describes the University Union as the campus gathering place—student-funded and a hub for programs, services, meals, and interaction. ([California State University, East Bay](https://www.csueastbay.edu/uu/?utm_source=chatgpt.com))

But the UU experience is fragmented:

- “What’s in the UU?” is spread across multiple pages (floor plans, gamezone, meeting rooms, policies, BaySync, dining).
- The UU “Events” page is currently being updated (“digital dust”), which signals a real gap in a single, reliable “what’s happening” feed. ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/events.html?utm_source=chatgpt.com))

**Opportunity:** build a **single digital front door** for UU—showcase everything it has, drive attendance/engagement, and connect users to the existing booking systems when needed.

---

## 2) What info the CSUEB website already gives us (North + South audit)

### 2.1 North University Union (Old UU) — floor-by-floor inventory

CSUEB publishes a **North UU floor plan page** with concrete items we can surface as app content. ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

**North UU – First Floor (published items)**

- Access to West Loop road
- “UU102 OFFLINE, Wellbeing Suite coming soon!”
- Water bottle refill station
- Chartwells offices
- Stairs/elevator/restrooms ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

**North UU – Second Floor (published items)**

- Study/lounge areas, printer station, charging
- Game Room + Game Cave
- Dining area: Fry Shack, Taco Bell Express, Wild Blue, Market
- Black Student Success Center
- Stairs/elevator/restrooms ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

**North UU – Third Floor (published items)**

- Study/lounge areas + balcony
- UU311
- UU307ABC – ASI Board Offices
- ASI Offices
- Stairs/elevator/restrooms ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

**App implication:** North UU already has a *structured content list* (amenities + dining + offices + centers) that can become an in-app directory immediately.

---

### 2.2 South University Union (New UU) — floor-by-floor inventory

CSUEB publishes a **South UU floor plan page** with key services and centers. ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html))

**South UU – First Floor (published items)**

- Dining room area, microwave station, vending machines
- Panda Express, Halal Bites of Chicago
- DISARC (Diversity & Inclusion Student and Affinity Research Centers)
- QUSSC (Queer Unity Student Success Center)
- Charging station + bulletin board
- UU Customer Service/Operations Assistant Desk
- Water bottle refill station
- Multipurpose Room (MPR)
- Outdoor stage / UU/MI lawn access
- Stairs/elevator/restrooms ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html))

**South UU – Second Floor (published items)**

- Bayview Room
- SLIC (Student Leadership and Involvement Center)
- Study/lounge areas, printer station
- The Gallery (Room 2010)
- API Student Resource Center, Undocumented Student Resource Center, Latinx Student Resource Center
- DISARC + Student Resource Center Admin Office
- Stairs/elevator/restrooms ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html))

**App implication:** South UU is a *student services + events engine* (SLIC, resource centers, MPR/Bayview, outdoor stage). This should be front-and-center in the app.

---

### 2.3 Meeting rooms + virtual tours (great for an app)

CSUEB’s UU pages include a **Meeting Rooms** section listing North + South rooms. ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/index.html))

Some rooms have **3D/virtual tour links** (examples: UU311, Bayview Room, MPR). ([Vivid Media Virtual Tours](https://www.tours.vividmediany.com/3d-model/calstateeastbay-uu311/fullscreen/?utm_source=chatgpt.com))

**App idea:** “Preview the space” cards that open the 3D tour instantly.

---

## 3) What UU services we can surface as “features” in the app (mapped to sources)

Below is a “surface map” (what exists today → how it becomes an app module).

### A) “Explore UU” Directory (high impact, low risk)

**What we already have:** floor plan item lists for North + South (amenities, centers, offices, dining). ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

**App surface:**

- Search: “MPR”, “Bayview”, “GameCave”, “QUSSC”, “SLIC”, “Black Student Success Center”
- Categories:
    - Spaces (MPR, Bayview, The Gallery, balcony, study lounges)
    - Student support centers (QUSSC, DISARC, API, USRC, Latinx Center, Black Student Success Center)
    - Services (Customer Service desk, printer stations, charging, microwaves, refill stations)
    - ASI offices (ASI + Board offices) ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

### B) “GameZone” module (already well-documented)

**What we already have:** GameZone description, hours, contact email. ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/))

Also:

- GameRoom features (billiards, air hockey, foosball; tournaments). ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/gameroom.html?utm_source=chatgpt.com))
- GameCave equipment description (consoles, VR). ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/gamecave.html?utm_source=chatgpt.com))
- Policies that clearly define time limits + cooldown + no concurrent bookings. ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/policies.html))
- GameZone Events list exists. ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/events.html?utm_source=chatgpt.com))
    
    **App surface:**
    
- “Reserve / How to play” flow (even if it links out initially)
- Live “Today’s hours”
- “What’s happening” (tournaments, Party Play, etc.) ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/party-play.html))

### C) “Dining in the UU” module (needs integration, but we can still surface it)

**What we already have on UU pages:** dining tenants listed in North + South floor plans. ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

CSUEB materials point users to CampusDish for dining menus/hours (menus/hours vary). ([California State University, East Bay](https://www.csueastbay.edu/ccc/ccc-directions.pdf?utm_source=chatgpt.com))

**App surface (practical):**

- Show tenant list + “Open menus” (deep link to CampusDish)
- “Hours may vary” disclaimer
- Optional: dining filters (halal/veg) as a later phase

### D) “Reserve a Space” module (booking integration)

**What we already have:**

- UU reservation entrypoint explains: faculty/staff/departments use **25Live**, external clients use an external reservation form, and student clubs/orgs are routed through **SLIC/BaySync**. ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/))
- The **UU Reservation & Facilities Procedures Guide** explains first-come/first-served handling and that requests are entered into 25Live and managed by UU staff. ([California State University, East Bay](https://www.csueastbay.edu/uu/files/docs/uu-reservation-policies-and-procedures-guide.pdf))
- A published **Pricing** page includes equipment fees and notes some resources require Fire Marshal review and ~45 days lead time. ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/pricing.html))
    
    **App surface:**
    
- “Book a room” wizard that routes users correctly:
    - Student org → BaySync event request pathway (with SLIC guidance)
    - Faculty/staff → 25Live sign-in
    - External/community → external reservation form ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/))

### E) “UU Staff / Contact / Help Desk”

**What we already have:** a UU Staff page listing key contacts + phone numbers. ([California State University, East Bay](https://www.csueastbay.edu/uu/about-us/staff.html?utm_source=chatgpt.com))

Also the UU Reservation Procedures PDF includes an operations contact for event assistance. ([California State University, East Bay](https://www.csueastbay.edu/uu/files/docs/uu-reservation-policies-and-procedures-guide.pdf))

**App surface:**

- “Get help now” button
- “Call UU ops / email reservations / email GameZone”
- “Where to go” (Customer Service desk is listed on South floor plan). ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html))

---

## 4) Booking integration plan (how we do it without breaking campus workflows)

### 4.1 Reality check: we should NOT replace 25Live/BaySync

UU already runs reservations through **25Live** and BaySync workflows, with rules, approvals, and staffing constraints. ([California State University, East Bay](https://www.csueastbay.edu/uu/files/docs/uu-reservation-policies-and-procedures-guide.pdf))

So the first implementation should be:

**Phase 1: “Smart routing + pre-filled forms”**

- In-app booking wizard
- Based on user type + booking type, the app routes to:
    - BaySync (students/RSOs)
    - 25Live (faculty/staff)
    - External inquiry form (community) ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/index.html))

**Phase 2: “Embedded booking experience”**

- Embed the booking pages in-app (webview) with a clean wrapper + instructions + FAQ

**Phase 3 (only if campus approves): API-level integration**

- If 25Live/BaySync integrations are available/approved, the app could display:
    - availability windows
    - request status
    - confirmations

### 4.2 GameZone booking: policies already define how a booking system should behave

GameZone policies explicitly include:

- 60-minute maximum services (unless stated)
- 10-minute cooldown before reserving same service again
- no multiple concurrent or back-to-back bookings without cooldown ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/policies.html))

**That’s perfect requirements text** for a future “reserve console/table” system if they ever want true in-app reservations.

---

## 5) “God-level” feature set for the UU app (what we can surface)

Think of the app as 4 pillars:

### Pillar 1 — Discover (Showcase everything)

- “What’s in the UU?” directory (North/South)
- Featured services of the week (SLIC, QUSSC, DISARC, etc.) ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html))
- Amenities finder (microwaves, printers, charging, water refill) ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

### Pillar 2 — What’s Happening (Events)

- Union events feed (needs rebuild because UU events page is under update) ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/events.html?utm_source=chatgpt.com))
- GameZone tournaments/events feed (already listed) ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/events.html?utm_source=chatgpt.com))
- BaySync events “in the Union” (future: tag/location filter) ([California State University, East Bay](https://www.csueastbay.edu/baysync/?utm_source=chatgpt.com))

### Pillar 3 — Book / Reserve (connect workflows)

- Meeting rooms / event space booking wizard (routes to correct system) ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/))
- “Before you book” checklist (lead time, equipment fees, etc.) ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/pricing.html))

### Pillar 4 — Eat / Play (sticky daily use)

- Dining tenants + menus linkouts (CampusDish) ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))
- GameZone hours + how it works + policies ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/))

---

## 6) Mockups and designs (screen-by-screen blueprint you can turn into Figma)

### Screen 1 — UU Home

**Top modules:**

- “What’s happening today” (3 cards)
- “Book a space”
- “Dining now”
- “GameZone now”
- “Find a service”

**Home cards (examples):**

- Party Play / Tournament / Workshop (event card)
- “MPR available? Start request”
- “Microwave station (South UU 1st floor)”

### Screen 2 — Explore (Directory)

Tabs:

- Spaces
- Services & Centers
- Dining
- Amenities

Each item page includes:

- What it is
- Where it is (North/South + Floor)
- Hours (if applicable)
- Contact
- Links (website / BaySync / reservation flow)

### Screen 3 — Events

Filters:

- Today / This week
- North / South
- GameZone / SLIC / Centers / Dining promos
- “Student org events” (BaySync feed later)

### Screen 4 — Book / Reserve Wizard

Step 1: What do you want to book?

- Meeting room (UU)
- Event space (MPR/Bayview)
- GameZone Friday reservation info

Step 2: Who are you?

- Student org
- Faculty/staff
- Community/external

Step 3: Route + checklist

- Correct system link (BaySync / 25Live / External form)
- Required lead time reminders
- Equipment fees reminder ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/pricing.html))

### Screen 5 — GameZone

- Hours + email contact ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/))
- “How it works” (policies summary) ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/policies.html))
- Events/tournaments list ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/events.html?utm_source=chatgpt.com))

### Screen 6 — Dining

- List North + South tenants (from floor plan pages)
- “Menus & hours” opens CampusDish (deep link) ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/old-uu/index.html))

---

## 7) How we advertise this app (UU growth plan)

### On-site (UU)

- QR codes at:
    - South UU customer service desk ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html))
    - entrances
    - dining seating areas
    - GameZone front counter (with “Reserve info / events”) ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/))
- “Digital bulletin board” concept: the South UU page literally lists a bulletin board—turn that into a digital version in-app. ([California State University, East Bay](https://www.csueastbay.edu/uu/meeting-rooms/new-uu/index.html))

### Student behavior channels

- BaySync announcements (since BaySync is the engagement platform) ([California State University, East Bay](https://www.csueastbay.edu/baysync/?utm_source=chatgpt.com))
- SLIC communications (Weeks of Welcome, involvement) ([California State University, East Bay](https://www.csueastbay.edu/slic/?utm_source=chatgpt.com))
- Partner with QUSSC/DISARC/resource centers to cross-promote inside their event pages/socials ([California State University, East Bay](https://www.csueastbay.edu/qussc/events.html?utm_source=chatgpt.com))

### “Sticky reasons to open weekly”

- Event reminders (“today in UU”)
- GameZone tournament schedule ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/events.html?utm_source=chatgpt.com))
- Dining quick links

---

## 8) “Survey + feedback” (what you meant by “bring that survey and implement it”)

Add a lightweight in-app feedback module from day 1:

**Micro-survey (15 seconds):**

1. What did you come to UU for today?
- Food / Study / Event / Student services / GameZone / Meeting / Other
1. Did you find what you needed?
- Yes / No
1. What should the UU app show better?

**Booking-specific feedback:**

- “Was the booking routing correct?” (BaySync vs 25Live vs external)

This gives you data to justify the next phase.

---

## 9) Implementation plan (committee-friendly, approval-ready)

### Phase 0 — Confirm owners + content governance (2–3 weeks)

- UU Operations owns: spaces, hours, meeting rooms, policies ([California State University, East Bay](https://www.csueastbay.edu/uu/about-us/staff.html?utm_source=chatgpt.com))
- GameZone owns: hours, events, policies ([California State University, East Bay](https://www.csueastbay.edu/uu/gamezone/))
- SLIC owns: student org workflows + BaySync guidance ([California State University, East Bay](https://www.csueastbay.edu/slic/?utm_source=chatgpt.com))
- Dining owner: Pioneer Dining/CampusDish linkouts ([California State University, East Bay](https://www.csueastbay.edu/ccc/ccc-directions.pdf?utm_source=chatgpt.com))

### Phase 1 — MVP (6–8 weeks)

- UU directory (North + South)
- GameZone module
- “Reserve a space” routing wizard
- Events: start with GameZone + featured UU items (because UU events page is under update) ([California State University, East Bay](https://www.csueastbay.edu/uu/reservations/events.html?utm_source=chatgpt.com))
- Feedback survey

### Phase 2 — Event feed improvement (4–6 weeks)

- Pull from BaySync (location-tagged UU events) ([California State University, East Bay](https://www.csueastbay.edu/baysync/?utm_source=chatgpt.com))
- Center/service cards (QUSSC, DISARC, etc.)

### Phase 3 — Optional deeper booking UX

- Embedded 25Live/BaySync flows
- If approved: availability + status surfaces

---

## 10) The exact “approval ask” you can use when pitching

Ask them to approve **process**, not “build me an app.”

**Approval request:**

1. Recognize the need for a dedicated UU digital hub experience
2. Identify the UU content owner + ITS/app publishing contact
3. Approve an MVP pilot scope (directory + events + booking routing)
4. Set a 30-day checkpoint for feasibility + MVP requirements

---

If you want, I can turn this into:

- a **1-page executive brief** (super tight for leadership), and
- a **mockup checklist** you can hand to a designer (Figma frames + components + copywriting for each screen).