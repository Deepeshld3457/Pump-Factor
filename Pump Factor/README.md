# The Pump Factor: A Gym Workout Analysis 💪

## Overview
A Power BI project analyzing workout data from 20 gym-goers across 
480 logged sessions to identify which exercises, equipment types, 
and conditions (time of day, cardio timing, protein intake) produce 
the highest muscle "pump."

## Data Model
Star schema with 3 tables:
- **Person_Dim** — 20 people (demographics, experience level, gym)
- **Exercise_Dim** — 52 exercises across 7 muscle groups
- **Workout_Log** — 480 workout entries (fact table)

Relationships: `Person_ID` and `Exercise_ID` connect the fact table to 
both dimension tables.

## Key Insights
- Evening workouts consistently show higher pump ratings than morning sessions, across almost every muscle group
- Barbell and Dumbbell exercises outperform Machine exercises for pump
- **Legs** — highest pump in the evening with no cardio
- **Chest** — pumps hardest with cardio done before the evening session
- **Biceps** — Concentration Curls and Hammer Curls deliver the strongest pump
- **Shoulders** — light up most in the evening, especially with cardio skipped
- Protein timing (within 30 min vs later) shows only a mild effect on pump rating

## Report Pages
1. **Overview** — KPIs and high-level comparisons across Muscle Group, Equipment Type, Time of Day, Cardio Timing, and Protein Timing
2. **Deep Dive** — Interactive matrix filterable by Muscle Group, Cardio Timing, and Time of Day, with conditional formatting highlighting top-performing exercises
3. **Key Insights** — Summary findings and final recommendation

## Tools Used
Power BI Desktop, DAX, Excel


