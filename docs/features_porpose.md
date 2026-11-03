# BalenceDiet — Feature Purpose

For every feature: what problem it solves, and how it helps the app.
Read with docs/FEATURES.md (same IDs).

## A. User profile
Purpose of section: the app cannot personalise anything without knowing the user.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| A1 | Setup questionnaire | New users don't know what data the app needs | Collects everything in one guided flow so planning works from day one |
| A2 | Body data | Calorie needs depend on age, sex, height, weight | Base input for calculating daily targets; target weight defines the goal |
| A3 | Diet type | A veg/Jain user must never be shown non-veg or root-vegetable dishes | Filters the menu before any planning happens |
| A4 | Activity level | Two people of same body burn different calories | Adjusts daily targets; fallback when no activity is logged (I6) |
| A5 | Allergies | Recommending an allergen can cause real harm | Hard block — safety rule the planner can never break |
| A6 | Intolerances & dislikes | A plan the user won't eat is useless | Ranks those dishes low instead of blocking, keeps plans realistic |
| A7 | Known deficiencies | User may have low iron, B12 etc. and food can help | Planner favours helpful foods; nutrient tracking focuses on them |
| A8 | Skipped meal slots | Many people never eat breakfast | Splits the day's target over meals actually eaten, avoiding overeating at others |
| A9 | Units & spoon calibration | "1 spoon" differs between messes and people | Makes portion advice match the user's real spoon/ladle |
| A10 | Multiple users | Hard rule: not built for one person only | Each person gets their own plan from one shared menu |

## B. Food modes
Purpose of section: different goals need different targets and food rules.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| B1 | Goal modes | Fat loss, bulk, maintenance need different calories | Sets the calorie and macro targets the planner aims for |
| B2 | Performance modes | Gym/endurance/exam weeks change needs | Shifts protein, carbs and meal timing for the situation |
| B3 | Eating-pattern modes | Some users follow low-carb or fasting windows | Adds rules on which foods and when, on top of the goal |
| B4 | Mode stacking | Real users combine modes (lean bulk + veg + exam week) | Lets modes combine and warns when they conflict |
| B5 | Health-support modes | Diabetic or heart-conscious users eat differently | Prefers suitable dishes; general guidance only, never treatment |
| B6 | Fasting days | Religious fasts change what can be eaten on some days | Applies special rules only on chosen dates |
| B7 | Pause / sick-day mode | Illness, exams or travel break normal eating | Stops goal pressure without corrupting history or progress |

## C. Menu input & understanding
Purpose of section: the menu is the app's main input — if it is misread, every plan is wrong.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| C1 | Upload weekly menu | The menu changes every week and is shared | Gets the week's food options into the app |
| C2 | Rebuild day × meal table | Shared menus (PDF grids) become jumbled text | Knows which dish is on which day and meal |
| C3 | Dish name cleanup | "BIRIYANI / BIRYANI", "UGANNI / UGGANI" | One dish = one record, so nutrition data is reused correctly |
| C4 | Confirm screen | Automatic reading can make mistakes | User catches errors before they reach the plan |
| C5 | Unknown dish handling | Guessing a dish's nutrition creates silent errors | Asks the user instead of inventing data |
| C6 | Teach-once dish library | Same unknown dish shouldn't be asked every week | Answers are saved and shared by everyone using that menu |
| C7 | Menu reuse | User may forget to upload a new menu | Plan still works, with a warning it may be outdated |
| C8 | Same-day change | Mess often replaces a dish on the day | Plan updates to what is actually served |

## D. Nutrition knowledge
Purpose of section: the app must know what is in each dish to give portions.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| D1 | Dish database | Planning needs calories and macros per dish | Core data every calculation depends on |
| D2 | Key micronutrients | Deficiency support needs iron, B12, calcium etc. | Makes A7 and the weekly summary possible |
| D3 | Estimates with confidence | Mess oil, gravy and portions vary | Honest ranges instead of false precision; planner can be cautious |
| D4 | Source shown | User should know where numbers come from | Builds trust; makes wrong data easy to find and fix |
| D5 | Dish components | Egg curry = eggs + gravy; they matter differently | Allows portion advice per part ("3 eggs, little gravy") |

## E. Targets & portions
Purpose of section: turn nutrition goals into something a person can act on at the counter.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| E1 | Daily targets | User needs a clear calorie/macro goal | Gives the planner its numbers to hit |
| E2 | Safety floor & safe rate | Extreme cuts or bulks are unhealthy | Planner can never suggest dangerous intake or speed |
| E3 | Goal reached | Users keep cutting after hitting target weight | Suggests maintenance so the plan doesn't overshoot |
| E4 | Portion advice in mess units | "300 kcal" is useless at the counter | Core promise: "3 eggs + 3–4 spoons rice" |
| E5 | Protein split across meals | All protein in one meal is less effective | Spreads protein, important for bulk and recomposition |
| E6 | "Why this amount?" | Unexplained numbers aren't trusted | Shows the reasoning; user can spot and correct mistakes |

## F. Planning
Purpose of section: combine menu + profile + targets into a usable week.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| F1 | Weekly plan | Day-by-day planning misses weak/strong days | Balances the whole week (e.g. plan around chicken day) |
| F2 | Staples fill gaps | Some days' main dish is low in protein | Uses curd, eggs, dal, fruit, milk to hit targets |
| F3 | Swap one meal | User dislikes a dish or it runs out | Changes one meal without rebuilding the whole week |
| F4 | Replan after reality | People skip, eat less/more, or eat outside | Plan stays correct instead of becoming useless by Tuesday |
| F5 | Day-specific targets | Gym days need more than rest days | Different targets per day type |
| F6 | My stash | Mess food can't always meet protein goals | Uses foods the user keeps (peanuts, whey, bananas) |
| F7 | Outside food library | Users eat at canteens and shops | Counts outside food correctly, optional budget |
| F8 | Water intake target | Hydration matters and is easy to forget | Daily water goal based on weight and activity |
| F9 | Caffeine timing | Tea/coffee/Boost add up and affect sleep | Counts caffeine and suggests cut-off times |

## G. Logging & progress
Purpose of section: the app must know what actually happened, not just what was planned.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| G1 | Quick log | Long logging forms get abandoned | Fast "as planned / half / skipped / extra" keeps data flowing |
| G2 | Saved meals | Staples repeat every week | One-tap logging of repeated meals |
| G3 | Weight tracker | Daily weight jumps around | Trend shows real progress toward target weight |
| G4 | Weekly summary | User needs to see gaps and progress | Shows nutrient gaps with honest error ranges |
| G5 | Target adjustment | Formulas are only a starting guess | Corrects targets using real results, only after enough data |
| G6 | Export / print plan | Phone may not be handy at the mess | Plan available offline / on paper |

## H. Privacy & data
Purpose of section: health data is sensitive and the app has multiple users.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| H1 | Private health data | Allergies, weight, deficiencies are personal | Users sharing a menu never see each other's data |
| H2 | Export & delete | Users must control their own data | Trust; user can leave and take data with them |
| H3 | Medical disclaimer | The app gives guidance, not diagnosis | Sets clear limits and protects users and the project |

## I. Activity
Purpose of section: calories burned change how much a person should eat.

| ID | Feature | Why we need it | How it helps the app |
|---|---|---|---|
| I1 | Daily activity entry | Any watch, gym machine or estimate can be used | Works for every user, with or without a watch |
| I2 | Activity-adjusted targets | Active days need more food | Raises that day's target, partially, since device numbers are inexact |
| I3 | Mode-aware activity | Same burn means different things per goal | Fat loss adds back little; bulk more; gym adds protein/carbs |
| I4 | Auto gym-day detection | Users forget to mark gym days | Logged workout switches the day to training targets |
| I5 | Reality check | Watch calorie numbers often overestimate | Weight trend overrides entered numbers if they disagree |
| I6 | No-entry fallback | Blank day ≠ zero activity | Uses profile activity level so targets aren't wrongly lowered |
