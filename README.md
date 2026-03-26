# P04 · The Cognitive and Emonional Pillars

**Section:** 01 — The Digital Twin Foundation

**Workflow step:** Step 4 of 4

**Current version:** 1.0

**Status:** ✅ Tested and approved

**Last updated:** March 2026

---

## 📌 Prompt Text (v1.0 — current)

```
Role: You are a Lead Sports Psychologist and Performance Consultant for an elite European football club.

Action: Distribute the "Cognitive and Emotional Pillar" (every input) for Player ID [player_id] in a "Neural & Emotional Readiness" table. Return in JSON format.

Context: We are preparing matchday 2. The data is collected from post-game recovery sessions and morning-of-training wellness checks. This table completes the "Digital Twin" model by layering mental fatigue and emotional state over the physical (P02) and tactical (P03) pillars.

Inputs:
- Reaction Time: [react_time] ms
- Cognitive Flexibility: [cog_flex]%
- Neural Readiness: [neural_status]
- Sleep Architecture: [sleep_hr] hr
- HRV (Heart Rate Variability): [hrv_score]
- RPE (Rate of Perceived Exertion): [rpe_score]
- Stress Level: [stress_val]
- Fatigue Level: [fatigue_val]
- Mood Level: [mood_val]

Constraints:
- Create ONE table per each [player_id].
- Maintain a highly analytical, psychological, and clinical tone.

Cognitive/Emotional Data in JSON format:

{
  "la_liga_cognitive_emotional_week_1": [
    { "player_id": "824001", "pos": "GK", "reaction_time_ms": 210, "cognitive_flexibility_pct": 95, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.2, "hrv": 68, "rpe": 4, "stress_level": 2, "fatigue_level": 3, "mood_level": 8 },
    { "player_id": "824002", "pos": "RB", "reaction_time_ms": 245, "cognitive_flexibility_pct": 82, "neural_readiness": "Red", "sleep_architecture_hr": 6.1, "hrv": 52, "rpe": 8, "stress_level": 4, "fatigue_level": 5, "mood_level": 6 },
    { "player_id": "824003", "pos": "CB", "reaction_time_ms": 230, "cognitive_flexibility_pct": 88, "neural_readiness": "Moderate", "sleep_architecture_hr": 7.0, "hrv": 58, "rpe": 7, "stress_level": 3, "fatigue_level": 4, "mood_level": 7 },
    { "player_id": "824004", "pos": "CB", "reaction_time_ms": 238, "cognitive_flexibility_pct": 85, "neural_readiness": "Moderate", "sleep_architecture_hr": 6.8, "hrv": 55, "rpe": 7, "stress_level": 3, "fatigue_level": 4, "mood_level": 7 },
    { "player_id": "824005", "pos": "LB", "reaction_time_ms": 255, "cognitive_flexibility_pct": 78, "neural_readiness": "Red", "sleep_architecture_hr": 5.5, "hrv": 49, "rpe": 9, "stress_level": 5, "fatigue_level": 6, "mood_level": 5 },
    { "player_id": "824006", "pos": "CDM", "reaction_time_ms": 268, "cognitive_flexibility_pct": 74, "neural_readiness": "Red", "sleep_architecture_hr": 6.2, "hrv": 42, "rpe": 9, "stress_level": 4, "fatigue_level": 6, "mood_level": 6 },
    { "player_id": "824007", "pos": "CM", "reaction_time_ms": 275, "cognitive_flexibility_pct": 71, "neural_readiness": "Red", "sleep_architecture_hr": 5.8, "hrv": 40, "rpe": 10, "stress_level": 5, "fatigue_level": 7, "mood_level": 5 },
    { "player_id": "824008", "pos": "CM", "reaction_time_ms": 262, "cognitive_flexibility_pct": 75, "neural_readiness": "Red", "sleep_architecture_hr": 6.0, "hrv": 44, "rpe": 9, "stress_level": 4, "fatigue_level": 6, "mood_level": 6 },
    { "player_id": "824009", "pos": "RW", "reaction_time_ms": 250, "cognitive_flexibility_pct": 80, "neural_readiness": "Moderate", "sleep_architecture_hr": 6.5, "hrv": 48, "rpe": 8, "stress_level": 4, "fatigue_level": 5, "mood_level": 7 },
    { "player_id": "824010", "pos": "ST", "reaction_time_ms": 242, "cognitive_flexibility_pct": 84, "neural_readiness": "Moderate", "sleep_architecture_hr": 7.2, "hrv": 51, "rpe": 8, "stress_level": 3, "fatigue_level": 5, "mood_level": 7 },
    { "player_id": "824011", "pos": "LW", "reaction_time_ms": 235, "cognitive_flexibility_pct": 86, "neural_readiness": "Moderate", "sleep_architecture_hr": 7.5, "hrv": 56, "rpe": 7, "stress_level": 3, "fatigue_level": 4, "mood_level": 8 },
    { "player_id": "824012", "pos": "CM", "reaction_time_ms": 225, "cognitive_flexibility_pct": 90, "neural_readiness": "Optimal", "sleep_architecture_hr": 7.8, "hrv": 62, "rpe": 6, "stress_level": 2, "fatigue_level": 3, "mood_level": 8 },
    { "player_id": "824013", "pos": "RB", "reaction_time_ms": 220, "cognitive_flexibility_pct": 92, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.0, "hrv": 65, "rpe": 5, "stress_level": 2, "fatigue_level": 2, "mood_level": 9 },
    { "player_id": "824014", "pos": "LW", "reaction_time_ms": 218, "cognitive_flexibility_pct": 94, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.1, "hrv": 67, "rpe": 4, "stress_level": 2, "fatigue_level": 2, "mood_level": 9 },
    { "player_id": "824015", "pos": "GK", "reaction_time_ms": 205, "cognitive_flexibility_pct": 98, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.5, "hrv": 72, "rpe": 0, "stress_level": 1, "fatigue_level": 1, "mood_level": 10 },
    { "player_id": "824016", "pos": "CB", "reaction_time_ms": 208, "cognitive_flexibility_pct": 97, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.3, "hrv": 70, "rpe": 0, "stress_level": 2, "fatigue_level": 2, "mood_level": 9 },
    { "player_id": "824017", "pos": "LB", "reaction_time_ms": 202, "cognitive_flexibility_pct": 99, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.8, "hrv": 74, "rpe": 0, "stress_level": 1, "fatigue_level": 1, "mood_level": 10 },
    { "player_id": "824018", "pos": "CDM", "reaction_time_ms": 212, "cognitive_flexibility_pct": 96, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.0, "hrv": 69, "rpe": 0, "stress_level": 2, "fatigue_level": 2, "mood_level": 9 },
    { "player_id": "824019", "pos": "AM", "reaction_time_ms": 209, "cognitive_flexibility_pct": 97, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.4, "hrv": 71, "rpe": 0, "stress_level": 1, "fatigue_level": 1, "mood_level": 10 },
    { "player_id": "824020", "pos": "ST", "reaction_time_ms": 220, "cognitive_flexibility_pct": 92, "neural_readiness": "Moderate", "sleep_architecture_hr": 7.5, "hrv": 65, "rpe": 0, "stress_level": 3, "fatigue_level": 3, "mood_level": 8 },
    { "player_id": "824021", "pos": "RW", "reaction_time_ms": 200, "cognitive_flexibility_pct": 99, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.9, "hrv": 75, "rpe": 0, "stress_level": 1, "fatigue_level": 1, "mood_level": 10 },
    { "player_id": "824022", "pos": "CB", "reaction_time_ms": 204, "cognitive_flexibility_pct": 98, "neural_readiness": "Optimal", "sleep_architecture_hr": 8.6, "hrv": 73, "rpe": 0, "stress_level": 1, "fatigue_level": 1, "mood_level": 10 }
  ]
}
```

**Placeholders to Fill**

| Placeholder | Source / Description | Example |
| :--- | :--- | :--- |
| `[player_id]` | The 6-digit identification number | `824007` |
| `[react_time]` | CNS reaction speed in milliseconds | `275` |
| `[cog_flex]` | Cognitive flexibility/accuracy score | `71` |
| `[neural_status]` | Qualitative CNS recovery status (Visual flag) | `Red` |
| `[sleep_hr]` | Hours of recorded sleep (architecture) | `5.8` |
| `[hrv_score]` | Heart Rate Variability (RMSSD) | `40` |
| `[rpe_score]` | Perceived exertion from last session | `10` |
| `[stress_val]` | Subjective stress marker (1-10) | `5` |
| `[fatigue_val]` | Subjective fatigue marker (1-10) | `7` |
| `[mood_val]` | Subjective mood/valence marker (1-10) | `5` |
---

## 🏢 Intended Workflow or Task

This prompt captures the "invisible" neural and psychological metrics required to complete the athlete's **360-degree profile**.

* **Trigger:** Completion of morning wellness check-ins and CNS tap tests.
* **Actor:** Sports Psychologist, Performance Consultant, and Medical Staff.
* **Timing:** Post MatchDay 1 (Recovery Phase) and Pre MatchDay 2 (Match Preparation).
* **Next step:** `P05` — Final Digital Twin Dashboard assembly.

```
Wellness/CNS App Sync → [P04 runs] → Neural Readiness Table Created → Combined with P01, P02, P03 → 360° Digital Twin Dashboard
```

---

## ❗ Problem Being Solved

We intend to solve the critical failure of "Invisible Fatigue," where athletes appear physically recovered but are neurally depleted, leading to preventable non-contact injuries and tactical decision-making lapses.

**Pain Points Addressed:**

- Invisible Fatigue: Detecting Central Nervous System (CNS) burnout that physical GPS data (P02) cannot see. A player may be physically fast but cognitively slow.

- Objective Wellness: Converting subjective "mood" and "stress" into a clinical data format that can be correlated with (P02) and (P03).

- Injury Prevention: High RPE and low HRV are leading indicators of impending soft-tissue overstrain.

---

## ⚡ Automation Potential

**Overall Level:** `Medium`

| Dimension | Assessment |
| :--- | :--- |
| **Repetitiveness** | `High` &nbsp; - &nbsp; Required daily for the active squad. |
| **Data availability** | `High` &nbsp; - &nbsp; Pulls from Wellness APIs and Neuro-testing hardware. |
| **Human judgment** | `Low` &nbsp; - &nbsp; Critical for psychologist intervention on "Red" status. |

**Human-in-the-Loop Role:**

The **Lead Sports Psychologist** reviews the `Neural Readiness` status. If a key player is flagged as "Red" despite being physically fit (`P02`), the psychologist conducts a 1-on-1 session before the Tactical briefing.

**Key Insight:** This step prevents "Cognitive Overload" during tactical sessions, ensuring that only players with an "Optimal" or "Amber" neural status are pushed to their cognitive limits.

**Estimated time saving:** ~60% (Automated data collection and flagging vs manual interview-only process).

---

## ⚠️ Risks and Limitations

| Risk | Level | Mitigation |
| :--- | :--- | :--- |
| **Self-Reporting Bias** | `High` | Cross-reference subjective RPE/Mood with objective HRV and CNS Reaction Time deltas. |
| **Data Privacy (GDPR/Sensitive)** | `Medium` | Implement strict role-based access; JSON contains performance scores only, excluding raw clinical notes. |
| **Oversimplification of Mood** | `Low` | Trigger a qualitative 1-on-1 interview with the Lead Psychologist upon "Red" flag detection. |
| **Hardware Latency/Error** | `Low` | Deploy automated data-cleaning scripts to reject extreme outliers before the prompt execution. |

**Overall Risk Rating: MEDIUM** — Requires professional psychological oversight to ensure data supports athlete wellbeing and load management.

--- 

## 🔄 Version History

### v1.0 — Initial Draft ✅ Current
**Date:** March 14 2026

**Prompt:** 

```
Role: You are a Lead Sports Psychologist and Performance Consultant for an elite European football club.

Action: Distribute the "Cognitive and Emotional Pillar" (every input) for Player ID [player_id] in a "Neural & Emotional Readiness" table. Return in JSON format.

Context: We are preparing matchday 2. The data is collected from post-game recovery sessions and morning-of-training wellness checks. This table completes the "Digital Twin" model by layering mental fatigue and emotional state over the physical (P02) and tactical (P03) pillars.

Inputs:
- Reaction Time: [react_time] ms
- Cognitive Flexibility: [cog_flex]%
- Neural Readiness: [neural_status]
- Sleep Architecture: [sleep_hr] hr
- HRV (Heart Rate Variability): [hrv_score]
- RPE (Rate of Perceived Exertion): [rpe_score]
- Stress Level: [stress_val]
- Fatigue Level: [fatigue_val]
- Mood Level: [mood_val]

Constraints:
- Create ONE table per each [player_id].
- Maintain a highly analytical, psychological, and clinical tone.

Cognitive/Emotional Data in JSON format
```

Result: Successfully maps psychological and CNS data to individual player IDs.

**Output:**

```
{
  "neural_emotional_readiness_report": [
    {
      "player_id": "824001",
      "position": "GK",
      "metrics": {
        "reaction_time_ms": 210,
        "cognitive_flexibility_pct": 95,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.2,
        "hrv_score": 68,
        "rpe_score": 4,
        "stress_level": 2,
        "fatigue_level": 3,
        "mood_level": 8
      }
    },
    {
      "player_id": "824002",
      "position": "RB",
      "metrics": {
        "reaction_time_ms": 245,
        "cognitive_flexibility_pct": 82,
        "neural_readiness": "Red",
        "sleep_architecture_hr": 6.1,
        "hrv_score": 52,
        "rpe_score": 8,
        "stress_level": 4,
        "fatigue_level": 5,
        "mood_level": 6
      }
    },
    {
      "player_id": "824003",
      "position": "CB",
      "metrics": {
        "reaction_time_ms": 230,
        "cognitive_flexibility_pct": 88,
        "neural_readiness": "Moderate",
        "sleep_architecture_hr": 7.0,
        "hrv_score": 58,
        "rpe_score": 7,
        "stress_level": 3,
        "fatigue_level": 4,
        "mood_level": 7
      }
    },
    {
      "player_id": "824004",
      "position": "CB",
      "metrics": {
        "reaction_time_ms": 238,
        "cognitive_flexibility_pct": 85,
        "neural_readiness": "Moderate",
        "sleep_architecture_hr": 6.8,
        "hrv_score": 55,
        "rpe_score": 7,
        "stress_level": 3,
        "fatigue_level": 4,
        "mood_level": 7
      }
    },
    {
      "player_id": "824005",
      "position": "LB",
      "metrics": {
        "reaction_time_ms": 255,
        "cognitive_flexibility_pct": 78,
        "neural_readiness": "Red",
        "sleep_architecture_hr": 5.5,
        "hrv_score": 49,
        "rpe_score": 9,
        "stress_level": 5,
        "fatigue_level": 6,
        "mood_level": 5
      }
    },
    {
      "player_id": "824006",
      "position": "CDM",
      "metrics": {
        "reaction_time_ms": 268,
        "cognitive_flexibility_pct": 74,
        "neural_readiness": "Red",
        "sleep_architecture_hr": 6.2,
        "hrv_score": 42,
        "rpe_score": 9,
        "stress_level": 4,
        "fatigue_level": 6,
        "mood_level": 6
      }
    },
    {
      "player_id": "824007",
      "position": "CM",
      "metrics": {
        "reaction_time_ms": 275,
        "cognitive_flexibility_pct": 71,
        "neural_readiness": "Red",
        "sleep_architecture_hr": 5.8,
        "hrv_score": 40,
        "rpe_score": 10,
        "stress_level": 5,
        "fatigue_level": 7,
        "mood_level": 5
      }
    },
    {
      "player_id": "824008",
      "position": "CM",
      "metrics": {
        "reaction_time_ms": 262,
        "cognitive_flexibility_pct": 75,
        "neural_readiness": "Red",
        "sleep_architecture_hr": 6.0,
        "hrv_score": 44,
        "rpe_score": 9,
        "stress_level": 4,
        "fatigue_level": 6,
        "mood_level": 6
      }
    },
    {
      "player_id": "824009",
      "position": "RW",
      "metrics": {
        "reaction_time_ms": 250,
        "cognitive_flexibility_pct": 80,
        "neural_readiness": "Moderate",
        "sleep_architecture_hr": 6.5,
        "hrv_score": 48,
        "rpe_score": 8,
        "stress_level": 4,
        "fatigue_level": 5,
        "mood_level": 7
      }
    },
    {
      "player_id": "824010",
      "position": "ST",
      "metrics": {
        "reaction_time_ms": 242,
        "cognitive_flexibility_pct": 84,
        "neural_readiness": "Moderate",
        "sleep_architecture_hr": 7.2,
        "hrv_score": 51,
        "rpe_score": 8,
        "stress_level": 3,
        "fatigue_level": 5,
        "mood_level": 7
      }
    },
    {
      "player_id": "824011",
      "position": "LW",
      "metrics": {
        "reaction_time_ms": 235,
        "cognitive_flexibility_pct": 86,
        "neural_readiness": "Moderate",
        "sleep_architecture_hr": 7.5,
        "hrv_score": 56,
        "rpe_score": 7,
        "stress_level": 3,
        "fatigue_level": 4,
        "mood_level": 8
      }
    },
    {
      "player_id": "824012",
      "position": "CM",
      "metrics": {
        "reaction_time_ms": 225,
        "cognitive_flexibility_pct": 90,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 7.8,
        "hrv_score": 62,
        "rpe_score": 6,
        "stress_level": 2,
        "fatigue_level": 3,
        "mood_level": 8
      }
    },
    {
      "player_id": "824013",
      "position": "RB",
      "metrics": {
        "reaction_time_ms": 220,
        "cognitive_flexibility_pct": 92,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.0,
        "hrv_score": 65,
        "rpe_score": 5,
        "stress_level": 2,
        "fatigue_level": 2,
        "mood_level": 9
      }
    },
    {
      "player_id": "824014",
      "position": "LW",
      "metrics": {
        "reaction_time_ms": 218,
        "cognitive_flexibility_pct": 94,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.1,
        "hrv_score": 67,
        "rpe_score": 4,
        "stress_level": 2,
        "fatigue_level": 2,
        "mood_level": 9
      }
    },
    {
      "player_id": "824015",
      "position": "GK",
      "metrics": {
        "reaction_time_ms": 205,
        "cognitive_flexibility_pct": 98,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.5,
        "hrv_score": 72,
        "rpe_score": 0,
        "stress_level": 1,
        "fatigue_level": 1,
        "mood_level": 10
      }
    },
    {
      "player_id": "824016",
      "position": "CB",
      "metrics": {
        "reaction_time_ms": 208,
        "cognitive_flexibility_pct": 97,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.3,
        "hrv_score": 70,
        "rpe_score": 0,
        "stress_level": 2,
        "fatigue_level": 2,
        "mood_level": 9
      }
    },
    {
      "player_id": "824017",
      "position": "LB",
      "metrics": {
        "reaction_time_ms": 202,
        "cognitive_flexibility_pct": 99,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.8,
        "hrv_score": 74,
        "rpe_score": 0,
        "stress_level": 1,
        "fatigue_level": 1,
        "mood_level": 10
      }
    },
    {
      "player_id": "824018",
      "position": "CDM",
      "metrics": {
        "reaction_time_ms": 212,
        "cognitive_flexibility_pct": 96,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.0,
        "hrv_score": 69,
        "rpe_score": 0,
        "stress_level": 2,
        "fatigue_level": 2,
        "mood_level": 9
      }
    },
    {
      "player_id": "824019",
      "position": "AM",
      "metrics": {
        "reaction_time_ms": 209,
        "cognitive_flexibility_pct": 97,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.4,
        "hrv_score": 71,
        "rpe_score": 0,
        "stress_level": 1,
        "fatigue_level": 1,
        "mood_level": 10
      }
    },
    {
      "player_id": "824020",
      "position": "ST",
      "metrics": {
        "reaction_time_ms": 220,
        "cognitive_flexibility_pct": 92,
        "neural_readiness": "Moderate",
        "sleep_architecture_hr": 7.5,
        "hrv_score": 65,
        "rpe_score": 0,
        "stress_level": 3,
        "fatigue_level": 3,
        "mood_level": 8
      }
    },
    {
      "player_id": "824021",
      "position": "RW",
      "metrics": {
        "reaction_time_ms": 200,
        "cognitive_flexibility_pct": 99,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.9,
        "hrv_score": 75,
        "rpe_score": 0,
        "stress_level": 1,
        "fatigue_level": 1,
        "mood_level": 10
      }
    },
    {
      "player_id": "824022",
      "position": "CB",
      "metrics": {
        "reaction_time_ms": 204,
        "cognitive_flexibility_pct": 98,
        "neural_readiness": "Optimal",
        "sleep_architecture_hr": 8.6,
        "hrv_score": 73,
        "rpe_score": 0,
        "stress_level": 1,
        "fatigue_level": 1,
        "mood_level": 10
      }
    }
  ]
}
```

---

## 📊 v1.0 Test Results

| Criteria | Score | Status |
| :--- | :---: | :--- |
| **JSON Structure** | `5.0 / 5` | `✅ JSON schema is valid.` |
| **Clinical Tone** | `5.0 / 5` | `✅ Professional psychology tone maintained.` |
| **Pillar Consistency** | `5.0 / 5` | `✅ Digital Twin logic followed.` |
| **Data Plausibility** | `5.0 / 5` | `✅ Neural fluctuations are realistic.` |
| **Constraint Check** | `5.0 / 5` | `✅ All prompt rules met.` |
| **Overall Quality** | **`5.0 / 5`** | `⭐ Ready for operational use.` |

---

## 🔗 Related Prompts

- **Next in chain:** P04 — Cognitive & Emotional Pillars (Injects cognitive and emotional data onto the shell)


