# S3XY Buttons Mapping Plan — Tesla Model Y Juniper (4 Buttons + Commander)

## System Overview

**Hardware:** 4 × S3XY Buttons + S3XY Commander (Gen 2) OBD adapter
**Vehicle:** 2025 Model Y Juniper with FSD (Supervised)
**Placement:** Under center console armrest, left to right
**Ergonomics:** Left = easiest to reach → Right = least easy to reach

### How Each Button Works

Each S3XY button supports **3 press types**:

| Press Type | How to Trigger | Notes |
|---|---|---|
| **Single press** | Quick tap | Primary action. Note: enabling double/long press adds ~300ms delay to single press detection |
| **Double press** | Two quick taps | Secondary action |
| **Long press** | Press and hold ~1s | Tertiary action |

This gives you **4 buttons × 3 presses = 12 function slots** total.

> **Important trade-off:** When you assign double-press and long-press macros to a button, the system introduces a slight delay on single-press because it needs to wait and see if you're going to tap again or hold. This is acceptable for most functions, but worth knowing.

---

## Recommended Button Layout

```
┌──────────────────────────────────────────────────────────────┐
│                    CENTER CONSOLE ARMREST                     │
│                                                              │
│   ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐      │
│   │ BUTTON 1│  │ BUTTON 2│  │ BUTTON 3│  │ BUTTON 4│      │
│   │  DRIVE  │  │  VOICE  │  │ COMFORT │  │ ACCESS  │      │
│   │ ← EASY  │  │         │  │         │  │ HARD →  │      │
│   └─────────┘  └─────────┘  └─────────┘  └─────────┘      │
│                                                              │
│   Most used                              Least used          │
│   while driving                          while driving       │
└──────────────────────────────────────────────────────────────┘
```

---

## Button 1 — DRIVE (Leftmost, Easiest to Reach)

**Why leftmost:** This is your most-used button while actively driving. Your fingers naturally rest here. FSD engagement and follow-distance are constant adjustments.

| Press | Function | What It Does |
|---|---|---|
| **Single** | **Autopilot ON** | Engages FSD / Autosteer immediately. No need to reach for the scroll wheel. |
| **Double** | **Follow Distance −** | Decreases following distance one step (car follows closer). Quick double-tap to tighten the gap. |
| **Long** | **Follow Distance +** | Increases following distance one step (more space). Hold to create more room. |

**Mental model:** Tap = GO (engage). Double-tap = CLOSER. Hold = BACK OFF.

**Juniper-specific note:** The Model Y Juniper lacks TACC as a standalone feature. FSD/Autosteer is the primary automated driving mode. Consider also enabling the Commander's **Continuous Autopilot** automation so FSD automatically re-engages after lane changes (set up via the Commander tab in the S3XY app, not on a button).

---

## Button 2 — VOICE (Center-Left)

**Why here:** Second-most used while driving. Quick access to navigation, calls, and AI assistance.

| Press | Function | What It Does |
|---|---|---|
| **Single** | **Voice Command** | Activates Tesla's native voice assistant. Use for: "Navigate to [place]", "Call [contact]", "Set temperature to 72", "Play [song/playlist]", "Open charge port". This is what actually controls your car. |
| **Double** | **Grok** | Activates Grok AI assistant. Use for: asking questions, getting information, having a conversation. Grok is conversational AI — it does NOT control car functions (yet). |
| **Long** | **Play/Pause** | Toggle music/podcast/audiobook playback. Handy when someone starts talking to you or you need quick silence. |

**Critical distinction:** Tesla Voice Command ≠ Grok.
- **Voice Command** (single press) = controls your car. "Navigate to Costco." "Turn on seat heaters." "Call Mom."
- **Grok** (double press) = AI chatbot. "What's the best sushi restaurant nearby?" "Summarize the news." "Tell me a joke."

The user mentioned wanting Grok for "voice commands and set directions" — **Voice Command is actually what you want for directions and car controls.** Grok is the AI chat layer on top. Both are useful, which is why they're on the same button.

**Future-proofing:** Tesla's Spring 2026 update is adding "Hey Grok" voice activation, which may reduce the need for the Grok button. If so, you can remap the double-press to something else later (e.g., Next Song).

---

## Button 3 — COMFORT (Center-Right)

**Why here:** Moderate-use functions that improve comfort and driving feel. Not urgent enough for the leftmost buttons.

| Press | Function | What It Does |
|---|---|---|
| **Single** | **Defog / Defrost** | Immediately clears your windshield. This is a safety-critical function you want accessible without digging through menus on the touchscreen. One tap. |
| **Double** | **Steering Wheel Heater Toggle** | Toggles heated steering wheel on/off. Perfect for cold mornings — double-tap without looking at the screen. |
| **Long** | **Acceleration Toggle (Chill ↔ Sport)** | Switches between Chill and Sport driving modes. Hold when you want to change the car's character — loaning the car to someone (switch to Chill) or hitting an open road (switch to Sport). |

**Alternative options for this button** (if any of the above don't resonate):
- Single: **Fan Speed +** / Double: **Fan Speed −** / Long: **AC Toggle** (if you adjust climate constantly)
- Single: **Regen Up** / Double: **Regen Down** / Long: **Regen 100%** (if you frequently switch regen levels)
- Single: **Fold Mirrors** (great for tight parking)
- Single: **Heated Seats toggle** (if you use these more than steering wheel heater)

---

## Button 4 — ACCESS (Rightmost, Least Easy to Reach)

**Why rightmost:** Vehicle access functions are used when stopped or parking — not while actively driving. Lower urgency = further from resting fingers.

| Press | Function | What It Does |
|---|---|---|
| **Single** | **Lock / Unlock Toggle** | Locks or unlocks the car. Single tap. Useful when sitting in the car and you want to ensure doors are locked, or when unlocking for a passenger. |
| **Double** | **Open Trunk** | Pops the rear trunk. Double-tap when loading groceries, luggage, etc. |
| **Long** | **Open Frunk** | Opens the front trunk. Hold to open. Less commonly used than trunk, so it gets the long-press slot. |

**Note:** Tesla auto-locks when you walk away with your phone. The lock button is most useful for:
- Locking while sitting in the car (safety)
- Unlocking from inside for someone approaching
- Quick confirmation that the car is secured

---

## Complete Summary Table

| Button | Position | Single Press | Double Press | Long Press |
|---|---|---|---|---|
| **1 — DRIVE** | Left (easiest) | Autopilot ON | Follow Distance − | Follow Distance + |
| **2 — VOICE** | Center-left | Voice Command | Grok | Play/Pause |
| **3 — COMFORT** | Center-right | Defog/Defrost | Steering Wheel Heater | Chill ↔ Sport |
| **4 — ACCESS** | Right (hardest) | Lock/Unlock | Open Trunk | Open Frunk |

**Total functions mapped: 12** (using all 3 press types on all 4 buttons)

---

## Commander Automations (Set and Forget — No Button Needed)

These are configured in the S3XY app under the Commander tab. They run automatically — you don't need to waste a button on them:

| Automation | What It Does |
|---|---|
| **Continuous Autopilot** | Auto-reengages FSD/Autosteer after lane changes. Huge quality-of-life improvement. |
| **Presenting Doors** | Auto-pops driver door when approaching the car. |
| **Kickdown** | Temporarily switches from Chill to Sport when you floor it. |
| **Auto OFF** | Disables auto high beams and auto wipers (if they annoy you). |
| **Door Handle → Frunk** | Pull driver door handle to open frunk (instead of door). |

**Recommendation:** At minimum, enable **Continuous Autopilot** since you have FSD. This pairs perfectly with Button 1's Autopilot ON function.

---

## Setup Instructions

1. **Install Commander** at the right A-pillar (OBD connection)
2. **Open S3XY App** → Commander tab → enable Continuous Autopilot automation
3. **Pair each button:** S3XY App → Buttons tab → "Add S3XY Button" → hold button until connected
4. **Assign functions:** Tap the button in the app → tap the assigned function → search/browse the 130+ actions → select → use "Try Action" to test before saving
5. **Assign macros:** After setting the single-press function, tap "Add Macro" for double-press and long-press
6. **Mount buttons** under the center console armrest using the adhesive backing, left to right: DRIVE, VOICE, COMFORT, ACCESS
7. **Label them** (optional): rename in the app's visualization screen for easy reference

---

## Design Rationale

**Why this layout works:**

1. **Frequency-based positioning:** Most-used functions (FSD, voice) are on the left where your fingers naturally rest. Least-used (lock, trunk) are on the right.

2. **Logical grouping:** Each button has a clear theme (Drive, Voice, Comfort, Access). You'll never forget which button does what because the categories are intuitive.

3. **Consistent press-type logic across all buttons:**
   - **Single press** = primary/most-used function of that category
   - **Double press** = secondary function (or "decrease/closer" on Button 1)
   - **Long press** = tertiary function (or "increase/further" on Button 1)

4. **Safety-first:** Defog/Defrost is a single tap (no fumbling with touchscreen in an emergency). Autopilot engagement is a single tap. Lock is a single tap.

5. **No muscle-memory conflicts:** The press patterns are natural — you won't accidentally trigger the wrong thing because related functions are grouped together.

---

## Sources

- [Enhance Auto - S3XY Buttons Functions (Complete List)](https://www.enhauto.com/pages/buttons-functions)
- [Enhance Auto - The Commander](https://www.enhauto.com/pages/commander)
- [Enhance Auto - Full Walkthrough](https://www.enhauto.com/blogs/all/s3xy-buttons-for-your-tesla-full-walkthrough)
- [Enhance Auto - Autosteer Reengagement (Juniper)](https://www.enhauto.com/blogs/all/automatic-reengagement-of-the-autosteer-for-the-2025-model-y)
- [Enhance Auto - FAQ](https://www.enhauto.com/pages/faq)
- [T Sportline - S3XY Buttons Functions](https://tsportline.com/blogs/tesla-aftermarket-support/s3xy-buttons-functions)
- [Tesla Support - Grok](https://www.tesla.com/support/grok)
- [Tesla Oracle - 2026 Spring Update (Hey Grok)](https://www.teslaoracle.com/2026/04/16/the-complete-guide-to-teslas-2026-spring-update-hey-grok-fsd-app-cyberhog-pet-mode-more/)
- [Tesla Owner's Manual - FSD (Supervised)](https://www.tesla.com/ownersmanual/modely/en_us/GUID-2CB60804-9CEA-4F4B-8B04-09B991368DC5.html)
