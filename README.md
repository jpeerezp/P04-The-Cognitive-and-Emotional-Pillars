# P04 · The Cognitive and Emonional Pillars

**Section:** 01 — The Digital Twin Foundation

**Workflow step:** Step 4 of 4

**Current version:** 

**Status:** ✅ Tested and approved

**Last updated:** March 2026

---

## 📌 Prompt Text (v1.0 — current)

```
Role: You are an Assistant Coach, Lead Sports Scientist and S&C Consultant for an elite European football club.

Action: Distribute the "Technical and Tactical Pillar" (every input) for Player ID [player_id] in a  "Technical/Tactical Readiness" table that shows all the data for each [player_id] . Return in JSON format

Context: We are preparing matchday 2. The data is collected from matchday 1 and post-game week 1. The table must include all the analyzed data to be shown next to a "Digital twin" model of each [player_id].

Inputs:
 
- Progressive passes
- Expected Threat (xT)
- Pass completion under pressure
- Successful Dribbles
- Box entries
- Heatmaps & Average Position
- Packing rate
- Defensive compactness
- Pressing triggers
- Inter-line movements

Constraints:
- Create ONE table per each [player_id], not per player position.
- Clinical and professional tone.

Technical and Tactical Data in JSON format:
{
  "la_liga_technical_tactical_week_1": [
    { "player_id": "824001", "pos": "GK", "prog_passes": 8, "xt": 0.04, "pass_completion_under_pressure_pct": 88, "successful_dribbles": 0, "box_entries": 0, "avg_position": "Box", "packing_rate": 12, "defensive_compactness_pct": 95, "pressing_triggers": 1, "inter_line_movements": 0 },
    { "player_id": "824002", "pos": "RB", "prog_passes": 14, "xt": 0.18, "pass_completion_under_pressure_pct": 78, "successful_dribbles": 3, "box_entries": 4, "avg_position": "High-Wide", "packing_rate": 48, "defensive_compactness_pct": 82, "pressing_triggers": 14, "inter_line_movements": 8 },
    { "player_id": "824003", "pos": "CB", "prog_passes": 11, "xt": 0.08, "pass_completion_under_pressure_pct": 91, "successful_dribbles": 0, "box_entries": 0, "avg_position": "Mid-Deep", "packing_rate": 32, "defensive_compactness_pct": 94, "pressing_triggers": 6, "inter_line_movements": 2 },
    { "player_id": "824004", "pos": "CB", "prog_passes": 9, "xt": 0.05, "pass_completion_under_pressure_pct": 93, "successful_dribbles": 0, "box_entries": 1, "avg_position": "Mid-Deep", "packing_rate": 28, "defensive_compactness_pct": 96, "pressing_triggers": 5, "inter_line_movements": 1 },
    { "player_id": "824005", "pos": "LB", "prog_passes": 12, "xt": 0.22, "pass_completion_under_pressure_pct": 76, "successful_dribbles": 4, "box_entries": 5, "avg_position": "High-Wide", "packing_rate": 41, "defensive_compactness_pct": 80, "pressing_triggers": 12, "inter_line_movements": 9 },
    { "player_id": "824006", "pos": "CDM", "prog_passes": 18, "xt": 0.15, "pass_completion_under_pressure_pct": 86, "successful_dribbles": 1, "box_entries": 2, "avg_position": "Center-Mid", "packing_rate": 65, "defensive_compactness_pct": 91, "pressing_triggers": 22, "inter_line_movements": 12 },
    { "player_id": "824007", "pos": "CM", "prog_passes": 22, "xt": 0.29, "pass_completion_under_pressure_pct": 84, "successful_dribbles": 2, "box_entries": 6, "avg_position": "Box-to-Box", "packing_rate": 78, "defensive_compactness_pct": 88, "pressing_triggers": 19, "inter_line_movements": 15 },
    { "player_id": "824008", "pos": "CM", "prog_passes": 25, "xt": 0.31, "pass_completion_under_pressure_pct": 81, "successful_dribbles": 3, "box_entries": 5, "avg_position": "Box-to-Box", "packing_rate": 82, "defensive_compactness_pct": 85, "pressing_triggers": 17, "inter_line_movements": 14 },
    { "player_id": "824009", "pos": "RW", "prog_passes": 7, "xt": 0.35, "pass_completion_under_pressure_pct": 72, "successful_dribbles": 6, "box_entries": 8, "avg_position": "Final-Third", "packing_rate": 39, "defensive_compactness_pct": 75, "pressing_triggers": 15, "inter_line_movements": 11 },
    { "player_id": "824010", "pos": "ST", "prog_passes": 4, "xt": 0.12, "pass_completion_under_pressure_pct": 68, "successful_dribbles": 2, "box_entries": 9, "avg_position": "High-Central", "packing_rate": 18, "defensive_compactness_pct": 70, "pressing_triggers": 11, "inter_line_movements": 6 },
    { "player_id": "824011", "pos": "LW", "prog_passes": 10, "xt": 0.28, "pass_completion_under_pressure_pct": 75, "successful_dribbles": 5, "box_entries": 7, "avg_position": "Final-Third", "packing_rate": 34, "defensive_compactness_pct": 78, "pressing_triggers": 13, "inter_line_movements": 10 },
    { "player_id": "824012", "pos": "CM", "prog_passes": 6, "xt": 0.09, "pass_completion_under_pressure_pct": 85, "successful_dribbles": 1, "box_entries": 2, "avg_position": "Center-Mid", "packing_rate": 11, "defensive_compactness_pct": 88, "pressing_triggers": 6, "inter_line_movements": 4 },
    { "player_id": "824013", "pos": "RB", "prog_passes": 3, "xt": 0.04, "pass_completion_under_pressure_pct": 80, "successful_dribbles": 1, "box_entries": 1, "avg_position": "Mid-Wide", "packing_rate": 7, "defensive_compactness_pct": 90, "pressing_triggers": 4, "inter_line_movements": 2 },
    { "player_id": "824014", "pos": "LW", "prog_passes": 2, "xt": 0.02, "pass_completion_under_pressure_pct": 82, "successful_dribbles": 1, "box_entries": 1, "avg_position": "High-Wide", "packing_rate": 3, "defensive_compactness_pct": 92, "pressing_triggers": 2, "inter_line_movements": 1 },
    { "player_id": "824015", "pos": "GK", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 },
    { "player_id": "824016", "pos": "CB", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 },
    { "player_id": "824017", "pos": "LB", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 },
    { "player_id": "824018", "pos": "CDM", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 },
    { "player_id": "824019", "pos": "AM", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 },
    { "player_id": "824020", "pos": "ST", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 },
    { "player_id": "824021", "pos": "RW", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 },
    { "player_id": "824022", "pos": "CB", "prog_passes": 0, "xt": 0, "pass_completion_under_pressure_pct": 0, "successful_dribbles": 0, "box_entries": 0, "avg_position": "N/A", "packing_rate": 0, "defensive_compactness_pct": 0, "pressing_triggers": 0, "inter_line_movements": 0 }
  ]
}
```

**Placeholders to fill**

| Placeholder | Source / Description | Example |
| :--- | :--- | :--- |
| `[player_id]` | The 6-digit identification number | `824007` |
| `[prog_pass]` | Progressive passes made | `22` |
| `[xt]` | Expected Threat (xT) value | `0.29` |
| `[pass_pressure_pct]` | Pass completion % under pressure | `84` |
| `[drib_succ]` | Number of successful dribbles | `2` |
| `[box_entries]` | Successful entries into the penalty box | `6` |
| `[avg_pos]` | Heatmap / Average Position label | `Box-to-Box` |
| `[packing_rate]` | Total opponents bypassed | `78` |
| `[compact_pct]` | Defensive compactness % maintained | `88` |
| `[press_triggers]` | Defensive pressing triggers activated | `19` |
| `[inter_line_mvmt]` | Effective movements between lines | `15` |

---

## 🏢 Intended Workflow or Task

This prompt generates the individualized technical and tactical data cards required for the "Digital Twin" dashboard.

* **Trigger:** Availability of Matchday 1 Tactical and Technical data.
* **Actor:** Coaching Staff (Asistant Coach, Tactical Analyst, Individual Development Coach, Video/Data Analysts) and Technical Analysis Department.
* **Timing:** Post MatchDay 1; pre MatchDay 2 analysis.
* **Next step:** P04 (Cognitive and Emotional Pillars) introduction.

```
MD+1 Event Data → [P03 runs] → Individual Technical and Tactical Profile Created → Layered onto P01 Shell
→ P04 Introduction
```

---

## ❗ Problem Being Solved

Coaching staffs often struggle to bridge the gap between pure athletic output (`P02`) and tactical efficiency.

**Pain Points Addressed:**

- Isolated Metric Analysis: Standard reports often list passes without context. `P03` forces the AI to look at `Passes under Pressure` and `Inter-line Movements`, which define elite decision-making.

- Cognitive Overload for Coaches: Instead of reviewing 50+ individual stats, the Head Coach receives a clinical "Digital Twin" table that summarizes the player's tactical impact in MatchDay 1.

- Role-Specific Context: By providing `avg_position` and `packing_rate`, the prompt allows for a direct comparison between the player's assigned tactical role and their actual on-pitch execution.

---

### ⚡ Automation Potential

**Overall Level:** `High`

| Dimension | Assessment |
| :--- | :--- |
| **Repetitiveness** | `Very High` &nbsp; - &nbsp; Required for the full squad weekly. |
| **Data availability** | `High` &nbsp; - &nbsp; Maps 1:1 with modern football event-data APIs (Opta/StatsBomb). |
| **Human judgment** | `Medium` &nbsp; - &nbsp; AI synthesizes the "what"; Tactical Analyst reviews; Coach interprets the "why." |
| **Integration** | `High` &nbsp; - &nbsp; Can be automated via JSON pipeline directly to the dashboard. |

**Estimated time saving:** ~85% (Reduction in manual video-tagging vs data correlation time).
**Human-in-the-Loop Role:** Tactical Analyst must act as a gatekeeper. While the AI processes 100% of the raw event data into the "Digital Twin" table, the Analyst reviews data to ensure they align with the specific tactical instructions given before the match.

---

## ⚠️ Risks and Limitations

| Risk | Level | Mitigation |
| :--- | :--- | :--- |
| Hallucination of Data | `Medium` | Validate all fields in JSON before prompt runs; reject null values. |
| Contextual Nuances | `Medium` | Coach review required to account for mid-game anomalies. |
| Threshold Rigidity | `Low` | Clinical tone ensures objective reporting; analyst oversight for interpretation. |

**Overall Risk Rating: MEDIUM** - Suitable for tactical planning assistance with professional analyst oversight.

--- 

### v1.0 — Initial Draft (Runned Twice)
**Date:** March 12 2026

**Prompt:** 

```
Role: You are an Assistant Coach, Lead Sports Scientist and S&C Consultant for an elite European football club.

Action: Distribute the "Techical and Tacticall Pillar" (every input) for Player ID [player_id] in a  "Technical/Tactical Readiness" table that shows all the data for each [player_id] . 

Context: We are preparing matchday 2. The data is collected from matchday 1 and post-game week 1. The table must include all the analyzed data to be shown next to a "Digital twin" model of each [player_id].

Inputs: 

Progressive passes

xT

Pass completion under pressure

Successful Dribles

Box entries

Heatmaps & Average Position

Packing rate

Defensive com pactness

Pressing triggers

inter-line movements

Constraints:
- Create ONE table per each [player_id], not per player position.
- Clinical and professional tone.

Data in JSON
```

**Result:** After running the prompt twice, model introduced modular, individual tactical tables that map directly to the "Digital Twin".

**Observed effect:** Successfully distinguishes between "Starting" players and "Sub" players (IDs with 0 values).

**Lesson learned:** Forcing a 1:1 ID-to-Table ratio is the only way to ensure the data is "Digital Twin" ready for frontend injection.

---

## 📊 v1.0 Test Results

| Criteria | Score | Status |
| :--- | :---: | :--- |
| Instruction Adherence | `5.0 / 5` | ✅ Perfect |
| Completeness | `5.0 / 5` | ✅ All tactical pillars covered |
| Data Structuring Accuracy | `4.9 / 5` | ✅ Ready for JSON/UI integration |
| Readability | `4.9 / 5` | ✅ Optimized for High-Performance Staff |
| Tone Appropriateness | `4.8 / 5` | ✅ Professional & Clinical |
| Send-ready without edit| `4.7 / 5` | ✅ Minimal manual oversight needed |
| **Overall** | `4.9 / 5`| ⭐ Gold Standard |

---

## 🔗 Related Prompts

- **Next in chain:** P04 — Cognitive & Emotional Pillars (Injects cognitive and emotional data onto the shell)


