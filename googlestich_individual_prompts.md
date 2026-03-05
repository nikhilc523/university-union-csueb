This file contains **15 separate prompts**. 



Each prompt contains the global design rules to keep the app visually consistent, followed by the exact data and UI requirements for just that single screen.

---

### PROMPT 1: Welcome Screen (O1)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Welcome" Onboarding Screen for the "University Union Hub" (CSU East Bay) app.

Design System Rules:
- Theme: Dark Mode ONLY. True black background (#0B0B0D).
- Accent Color: Brand Red (#C8102E).
- Typography: SF Pro. 
- Touch Targets: >= 44x44pt.

UI Specifications for this screen:
- Visual: A beautiful, premium hero graphic/image of a modern University Union building at the top.
- Title (Large text): "University Union Hub"
- Subtitle: "Your digital front door to North + South UU."
- Call to Action (CTA): A large, pill-shaped Brand Red button at the bottom that says "Continue".
```

---

### PROMPT 2: Choose Role Screen (O2)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Choose Role" Onboarding Screen for the "University Union Hub" app.

Design System Rules:
- Theme: Dark Mode ONLY. True black background (#0B0B0D).
- Typography: SF Pro. 

UI Specifications for this screen:
- Top Navigation: A simple back arrow `<` on the top left.
- Title (Large text): "Who are you?"
- Subtitle: "Select your role to personalize booking and routing options."
- Interactive Elements (Cards or Radio Buttons): Three distinct, large selectable areas:
  1. "Student / Student Org"
  2. "Faculty & Staff"
  3. "Guest & External"
- Call to Action (CTA): A Brand Red button at the bottom that says "Next".
```

---

### PROMPT 3: Preferences Screen (O3)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Preferences" Onboarding Screen for the "University Union Hub" app.

Design System Rules:
- Theme: Dark Mode ONLY. True black background (#0B0B0D), cards/rows in Surface 1 (#121216).
- Typography: SF Pro. 

UI Specifications for this screen:
- Top Navigation: A simple back arrow `<` on the top left.
- Title (Large text): "Tailor your Hub"
- Subtitle: "What do you want to see?"
- Interactive Elements (iOS Toggle rows): Four distinct rows, each with an iOS-style toggle switch on the right side:
  1. "Notify me about UU events"
  2. "GameZone tournaments"
  3. "Dining hours & links"
  4. "Booking status reminders"
- Call to Action (CTA): A Brand Red button at the bottom that says "Get Started".
```

---

### PROMPT 4: Today Tab Root Screen (T1)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Today" Home Screen for the "University Union Hub" app.

Design System Rules:
- Theme: Dark Mode ONLY (#0B0B0D). Use Liquid Glass (blur) effects.
- Typography: SF Pro with dynamic headers.
- Global Navigation: Include a 5-tab iOS Bottom Nav Bar (Today, Explore, Events, Book, More). Highlight "Today" as active.

UI Specifications for this screen:
- Top Strip: Large Title "Today". Below it, a bright Green pill matching iOS HIG that says "OPEN NOW". Next to it, secondary text: "North UU • South UU".
- Event Section: Header "What's happening today". Below it, a large, swipeable, premium image card titled "ASI Board Meeting" with text "Starts at 3:00 PM".
- Quick Actions Section (Row of 5 square buttons with icons): [Explore North], [Explore South], [Book Space], [GameZone], [Dining].
- UU Essentials Section: Header "UU Essentials". Below it, a row of 4 circular icon buttons with labels: [Charging], [Water Refill], [Microwaves], [Printers].
```

---

### PROMPT 5: Essentials Detail Modal (E4)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Essentials: Microwaves" Bottom Sheet overlay.

Design System Rules:
- Theme: Dark Mode ONLY. The background should be the "Today" screen blurred out and darkened, with a Sheet (Surface 2: #1A1A21) pulled up to 50% height.
- Typography: SF Pro.

UI Specifications for this modal sheet:
- Top of Sheet: A small horizontal grab indicator for dismissing the sheet, and an (X) close button on top right.
- Title: "Microwave Stations"
- List Content (Use location pin icons for each):
  - Row 1: "South UU • Floor 1 (Near Vending Machines)"
  - Row 2: "North UU • Floor 2 (Near Market)"
- Footer Text (Small footnote): "Please clean up after use to keep our Union beautiful."
- Include the 5-tab Bottom Nav Bar visible at the very bottom of the screen.
```

---

### PROMPT 6: Explore Tab Root (E1)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Explore" Tab Root screen for the "University Union Hub" app.

Design System Rules:
- Theme: Dark Mode ONLY. 
- Global Navigation: Include the 5-tab Bottom Nav Bar. Highlight "Explore" as active.

UI Specifications for this screen:
- Top Area: Large Title "Explore". Below it, an iOS-style Search Bar with placeholder text: "Search 'MPR', 'Bayview', 'GameCave'".
- Segmented Control row: Three tabs: [North] | [South] | [All].
- Recent Searches Section: 3 small chips reading "Dining", "ASI Offices", "Charging".
- Filtered Results List (Directory view): 
  - Row 1: "Multipurpose Room (MPR)" | Subtitle: "South • Floor 1" | Badge: Red "Reservable".
  - Row 2: "GameCave" | Subtitle: "North • Floor 2" | Badge: Green "Open".
  - Row 3: "Washrooms / Restrooms" | Subtitle: "All Floors • Wheelchair Accessible (figure.roll icon)".
```

---

### PROMPT 7: Explore Filter Bottom Sheet (E1b)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Explore Filters" Bottom Sheet overlay.

Design System Rules:
- Theme: Dark Mode ONLY. Sheet (Surface 2: #1A1A21) pulled up to 75% height.

UI Specifications for this modal sheet:
- Top: Title "Filters", with a "Clear All" button on the top left and an (X) close button on the right.
- Section 1 "Building": Checkboxes for [North UU], [South UU].
- Section 2 "Floor": Checkboxes for [Floor 1], [Floor 2], [Floor 3 (North Only)].
- Section 3 "Category": A grid of tappable chips: [Rooms], [Dining], [Centers], [Amenities], [Washrooms], [Offices].
- CTA: A massive Brand Red button at the bottom of the sheet saying "Apply Filters (32 results)".
```

---

### PROMPT 8: Place Detail Room Page (E3)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Multipurpose Room (MPR) Detail" screen.

Design System Rules:
- Theme: Dark Mode ONLY. Pushed navigation style (Top Nav Bar has `< Explore` back arrow).

UI Specifications for this screen:
- Top Hero Image: A stunning edge-to-edge photo of a large event auditorium (the MPR). 
- Title area: "Multipurpose Room (MPR)".
- Detail Badges Row: [South UU] | [Floor 1] | [Wheelchair Route `figure.roll` icon].
- Action Buttons Row: [View 3D Tour] (Pill shape) and [Share icon].
- About text: "The UU's largest event space. Reservation Only. Contact: UU Customer Service."
- Capacity Table List:
  - Theater: 400 guests
  - Banquet: 240 guests
  - Classroom: 150 guests
- Equipment Chips: [Projector], [PA System], [Stage], [Dimmable Lighting].
- Bottom overlay CTA: A floating Brand Red button above the empty space: "Book this space".
```

---

### PROMPT 9: Events Tab Root (V1)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Events" Tab Root screen.

Design System Rules:
- Theme: Dark Mode ONLY. 
- Global Navigation: 5-tab Bottom Nav Bar. Highlight "Events" as active.

UI Specifications for this screen:
- Top: Large Title "Events".
- Filters Strip (horizontally scrolling chips): [Today], [This Week], [This Month], [North], [South].
- Featured Section: Header "Featured". A large image card for "GameZone Friday Tournament", showing subtitle "North UU Floor 2 • 5:00 PM".
- All Events List (Rows): 
  - Row 1: "Student Org Rally" - Subtitle: "Outdoor Stage • Starts in 1 hr".
  - Row 2: "DISARC Community Meeting" - Subtitle: "South UU Floor 1 • 6:00 PM".
```

---

### PROMPT 10: Event Detail Page (V2)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "GameZone Friday Tournament Event Detail" screen.

Design System Rules:
- Theme: Dark Mode ONLY. Pushed navigation (`< Events` back arrow).

UI Specifications for this screen:
- Hero Image: A high-quality photo of gamers playing on consoles/PCs.
- Title: "GameZone Friday Tournament: Smash Bros"
- Details Row: "Friday, Nov 12 • 5:00 PM - 9:00 PM".
- Location Box: "GameRoom • North UU Floor 2". Includes an arrow ">" implying tap for map/directions.
- Action Buttons: A row of two buttons: [Add to Calendar] and [Share].
- Info text: "Monthly Super Smash Bros tournament. 10-minute cooldown rules applied to free play stations during event."
- CTA (Brand Red pill): "RSVP Now on FusionPlay".
```

---

### PROMPT 11: Book Tab Root (B1)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Book & Reserve" Tab Root.

Design System Rules:
- Theme: Dark Mode ONLY. 
- Global Navigation: 5-tab Bottom Nav Bar. Highlight "Book" as active.

UI Specifications for this screen:
- Top: Large Title "Book & Reserve". Subtitle: "Select a category to start your reservation."
- Body Content (Two massive, beautiful image-background tiles stacked vertically):
  1. Tile 1 Image + Overlay Text: "Book a Room/Space" (Subtitle under it: "Meeting halls, creative studios, and event spaces").
  2. Tile 2 Image + Overlay Text: "GameZone Services" (Subtitle under it: "Reserve PC stations, consoles, or tables").
```

---

### PROMPT 12: Select Space Category (B2)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Select Space Category" page.

Design System Rules:
- Theme: Dark Mode ONLY. Pushed navigation (`< Book` back arrow).

UI Specifications for this screen:
- Top Title: "What are you booking?"
- List Rows (Cards with right-facing `>` arrows):
  - Card 1: "Meeting Rooms" (Subtitle: "UU311, Bayview, The Gallery. Small to medium capacities.")
  - Card 2: "Event Spaces" (Subtitle: "MPR A, MPR B. Large capacities, banquets, lectures.")
  - Card 3: "Outdoor Spaces" (Subtitle: "Stage / Lawn access.")
```

---

### PROMPT 13: Rules & Pricing Checklist (B4 & B5)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Review Policies" Checklist page.

Design System Rules:
- Theme: Dark Mode ONLY. Pushed navigation (`< Back`).

UI Specifications for this screen:
- Top Title: "Review Policies"
- Warning Alert Box (Yellow/Orange tint): "Important: Some requests, including stage/dance floors, require 45 days for Fire Marshal review."
- Checklist Options (User must tap these check circles):
  1. "( ) Cancellation: Email by 9am two business days prior."
  2. "( ) Decorations: No confetti or glitter; painters tape only."
  3. "( ) Clearing room: Please allow 30 minutes before and after your event."
  4. "( ) Insurance: COI due 10 working days before."
- Pricing Table Summary Section: "Chairs $5 • Rect Tables $12 • Round Tables $15 • Projector $45 • PA System $45 • Admin Fee 5%."
- CTA Bottom Button (Brand Red): "Acknowledge & Continue".
```

---

### PROMPT 14: Final Booking Gateway (B6)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "Final Request Routing" gateway page.

Design System Rules:
- Theme: Dark Mode ONLY. Pushed navigation (`< Back`).

UI Specifications for this screen:
- Top Title: "Ready to Request"
- Success Checkmark Icon (Large, centered).
- Body Text: "Because your role is set to Student Org, your reservation will be instantly routed to BaySync."
- Rule Note: "Requests are reviewed and confirmed by UU staff. You will receive confirmation by email. Note: Late cancellation fees ($50) or Policy Violation fees ($100) may apply."
- Primary Action CTA (Brand Red): "Open BaySync Form (Leaves App)"
- Secondary Action Text (Underneath the button): "Change my role to Faculty / External Guest"
```

---

### PROMPT 15: More Tab Root (M1)
```text
You are an expert iOS Product Designer. Generate ONE screen: The "More" (Operations) Tab Root.

Design System Rules:
- Theme: Dark Mode ONLY. iOS Settings app style (Groupेड lists).
- Global Navigation: 5-tab Bottom Nav Bar. Highlight "More" as active.

UI Specifications for this screen:
- Top: Large Title "More".
- Group 1 Title: "Union Details"
  - Row 1: "Hours & Location (Note: Spring weekends closed)" (Has `>` chevron).
  - Row 2: "Staff Directory" (Has `>` chevron).
  - Row 3: "About UU (North: 58k sqft • South: 29k sqft)" (Has `>` chevron).
- Group 2 Title: "Policies & Help"
  - Row 1: "GameZone Rules (60-min max, 10-min cooldown)"
  - Row 2: "Smoke & Tobacco-Free Campus Policy"
- Group 3 Title: "App"
  - Row 1: "Give Feedback / Report Errors"
```
