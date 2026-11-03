# BalenceDiet — Features (v1)

Status: DRAFT — freeze after review. No new features after freeze.
Late ideas go to "Not doing" unless they fix a bug or missing detail.

## A. User profile
- ★ A1 Setup questionnaire — first-run flow collecting all profile data
- ★ A2 Body data — age, sex, height, current weight, target weight
- ★ A3 Diet type — veg / non-veg / eggetarian / vegan / Jain / custom rules
- ★ A4 Activity level — how active the user is; optional gym vs rest days
- ★ A5 Allergies — hard block; "possible allergen" dishes shown with warning
- ★ A6 Intolerances & dislikes — avoided or ranked low, not hard-blocked
- ★ A7 Known deficiencies — entered by user from a diagnosis/lab report;
      planner favours foods that help. Never diagnoses.
- ★ A8 Skipped meal slots — e.g. "I don't eat breakfast"
- A9 Units — kg/lb, and personal spoon/ladle calibration
- ★ A10 Multiple users — separate private profiles sharing one menu

## B. Food modes
- ★ B1 Goal modes — fat loss, maintenance, lean bulk, bulk, recomposition
- B2 Performance modes — strength/high-protein, endurance, exam week
- B3 Eating-pattern modes — high-protein, low-carb, intermittent fasting window
- ★ B4 Mode stacking — combine goal + diet type + extra mode;
      warn when combinations conflict
- B5 Health-support modes — diabetes-friendly, heart-healthy, low-sodium;
      general guidance only, with a medical disclaimer
- B6 Fasting days — religious/fasting day rules on chosen dates
- ★ B7 Pause / sick-day mode — suspend goal pressure, keep history

## C. Menu input & understanding
- ★ C1 Upload weekly menu — paste text (PDF/image later if feasible)
- ★ C2 Rebuild day × meal table from messy text
- ★ C3 Dish name cleanup — spelling variants map to one dish
- ★ C4 Confirm screen — user checks parsed menu before planning
- ★ C5 Unknown dish handling — ask once, never guess silently
- ★ C6 Teach-once dish library — saved per menu/institution, shared by its users
- C7 Menu reuse — reuse last menu with warning if none uploaded
- ★ C8 Same-day change — "dish X replaced by Y" correction

## D. Nutrition knowledge
- ★ D1 Dish database — calories, protein, carbs, fat, fibre
- ★ D2 Key micronutrients — iron, B12, calcium, vitamin D, zinc, vitamin C
- ★ D3 Estimates with confidence — every value is a range, not a fact
- ★ D4 Source shown — where each number came from
- ★ D5 Dish components — e.g. egg curry = eggs + gravy, portioned separately

## E. Targets & portions
- ★ E1 Daily targets — calories and macros from profile + mode
- ★ E2 Safety floor & safe rate — minimum intake, maximum loss/gain speed
- ★ E3 Goal reached — suggest switching to maintenance
- ★ E4 Portion advice in mess units — "3 eggs + 3–4 spoons rice"
- ★ E5 Protein split across meals
- ★ E6 "Why this amount?" — explanation of target and portion

## F. Planning
- ★ F1 Weekly plan — whole week considered, not day-by-day
- ★ F2 Staples used to fill gaps — curd, eggs, dal, fruit, milk
- ★ F3 Swap one meal — replace a single meal without redoing the week
- ★ F4 Replan after reality — missed meal, ate less/more, ate outside
- F5 Day-specific targets — gym day vs rest day
- ★ F6 My stash — foods the user keeps (peanuts, whey, bananas) used for gaps
- F7 Outside food library — canteen/shop items with optional budget
- F8 Water intake target — based on body weight and activity
- F9 Caffeine timing — tea/coffee/Boost counted and timed away from sleep

## G. Logging & progress
- ★ G1 Quick log — "ate as planned", "half", "skipped", "extra"
- ★ G2 Saved meals — one-tap logging of repeated meals
- ★ G3 Weight tracker — trend line, not single readings
- ★ G4 Weekly summary — nutrient gaps with honest error ranges
- G5 Target adjustment — only after enough real data
- G6 Export / print weekly plan

## H. Privacy & data
- ★ H1 Health data private per user
- ★ H2 Export and delete my data
- ★ H3 Medical disclaimer shown in setup and health modes

## Not doing (consciously rejected)
- Barcode scanning
- Photo / AI food recognition
- Recipes and cooking instructions
- Grocery lists and delivery
- Social / community / challenges
- Wearable and fitness-tracker sync
- Diagnosing deficiencies or conditions
- Kidney-disease and weight-restoration modes (need medical supervision)

## Undecided until design stage
- Reminders (water/meals) — depends on platform
- PDF/image menu upload — depends on parsing feasibility
