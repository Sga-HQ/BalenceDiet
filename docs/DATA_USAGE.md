# BalenceDiet — How User Data Improves the Experience

Rule: every piece of data must change a decision. If it changes nothing, don't collect it.

## 1. The core loop
PLAN → USER EATS → USER LOGS (ate / skipped / partial / outside / fasted)
→ RECALIBRATE TODAY → WEEKLY: LEARN TRUE BURN FROM WEIGHT TREND → BETTER PLAN

- Short loop (same day): fix today's remaining meals.
- Long loop (weekly): fix the targets themselves.

## 2. What each data point is used for
| Data | Used for |
|---|---|
| Body data, activity level | Starting calorie target (a guess, corrected later) |
| Diet type, day rules, allergies | Filtering which dishes are allowed |
| Deficiencies | Choosing which nutrients the plan favours |
| Meal logs | Today's recalibration + weekly learning |
| Weight entries | Weight trend → learning true calorie burn |
| Activity entries | That day's target (counted partially) |
| Refusals and swaps | Learning preferences; future plans stay realistic |

## 3. Logging that a meal was eaten
Options: as planned / partly (¼, ½, ¾) / skipped / extra.
- Remaining meals today absorb the difference, within safe portion limits.
- If today can't absorb it, spread the remainder over the next 1–2 days.
  Never compensate by forcing one huge meal or one starvation meal.
- An unlogged meal is "unknown", not "skipped": ask later, don't guess.

## 4. Refusing a dish
- "Not today" → swap that one meal (F3); nothing else changes.
- "Never" → added to the user's dislike list (A6) and removed from all
  future plans; the user can undo it in their profile.
- If a "never" dish was the main protein of a meal, the planner makes up
  protein from staples or the user's stash.

## 5. Fasting on a chosen day
- One-off fasts (today / a date) and recurring fasts (every Ekadashi etc.).
- Fasting types: full fast, fruit/milk only, one meal only, custom food rules.
- The day's target is not added to the next day all at once; it is spread
  gently or simply dropped. Weekly protein is redistributed.
- Safety: repeated fasts close together trigger the underfuelling check (§6).

## 6. "You need to eat something now" (underfuelling check)
Uses energy availability = (food eaten − exercise burn) ÷ lean body mass.
- About 45 kcal/kg lean mass/day or more is the healthy reference.
- Below about 30 is the commonly cited danger zone.
Triggers:
- By a set time of day, intake is far below the safety floor.
- Multiple skipped meals in a row, or a fast plus high logged activity.
- Several low days in a row (rolling 3–7 day average).
Response: a clear, calm prompt naming a quick available food (staple or
stash item). Never a guilt message. If it repeats over days, suggest the user
talk to a doctor or nutritionist.
Lean mass is estimated (from body fat % if given, otherwise a conservative
approximation), so thresholds are applied with a safety margin.

## 7. Eating outside the menu
After logging an outside item:
- Show its effect calmly: "This uses about 40% of today's remaining
  calories; dinner will be lighter."
- If it filled the protein target, reduce protein portions for the rest of
  the day and favour vegetables and fibre instead.
- If the user is in fat-loss mode and goes over, spread the excess over the
  next days only within the safe-rate limits. Otherwise accept it; one
  meal doesn't ruin a goal.
- Tone: informative, never moralising.

## 8. Estimating outside-food calories without making the user work
Tiers, from least to most effort for the user:
1. Pick from the food library (burger, ice cream, samosa...) with size
   choice: small / regular / large. Each item has a range, not one number.
2. "Similar to": if the exact item isn't listed, the user picks the closest
   item; the estimate is marked low-confidence.
3. Category guess: "fried snack", "dessert", "sweet drink"; a wide range.
4. Manual entry: only if the user knows the number (e.g. from a label).
The library starts from public Indian databases (INDB recipes, IFCT 2017)
and grows when users teach new items (same as C6).

Why rough estimates are acceptable: the weekly learning loop (§1) compares
logged intake with the weight trend. If a user always underestimates by a
similar amount, the learned burn shifts too, and targets still produce the
intended weight change. Rough but consistent logging still works;
inconsistent or missing logging is what breaks it.

## 9. Learning the user's true burn (weekly)
- Weight trend = smoothed average, not raw daily weight.
- Needs about 2–4 weeks of reasonably regular logging + weigh-ins.
- Until then, the formula target is used and labelled "starting estimate".
- Changes are limited per week and always explained (E6).
- If logging is too sparse, do NOT recalibrate. Say why instead.
