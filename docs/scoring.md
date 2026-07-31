# Scoring Model

Version: 0.1 (Draft)

---

# Purpose

The scoring model defines how electric vehicles are evaluated within the EV-Decision-2027 project.

The primary goals are:

- transparency
- reproducibility
- explainability
- adaptability

Every score must be traceable back to documented evidence.

---

# Design Principles

The scoring model follows six fundamental principles.

## 1. Explainability

Every score must be understandable.

No "black box" calculations are allowed.

---

## 2. Separation of Facts and Ratings

Objective technical data

Examples

- battery capacity
- charging power
- dimensions

must never be mixed with

subjective ratings

Examples

- seat comfort
- software quality
- assistance behaviour

---

## 3. Evidence First

Marketing material never generates a score.

Scores are derived from

- measurements
- documentation
- independent testing
- real-world experience

---

## 4. User Profiles

The project does not define one universal "best vehicle".

Instead, different user profiles apply different weightings.

Example profiles

- Long Distance & Resilience
- Family
- Technology
- Budget
- Company Car

---

## 5. Confidence

Every subjective score includes a confidence level.

Confidence expresses

not

whether a vehicle is good,

but

how reliable the current assessment is.

---

## 6. OTA Awareness

Software updates may improve or reduce ratings.

Scores therefore always refer to a documented software version.

---

# Evaluation Layers

Vehicle evaluation consists of three independent layers.

## Layer 1

Objective Technical Data

Examples

Battery

Charging

Dimensions

Weight

Power

---

## Layer 2

Functional Evaluation

Examples

Assistance

Charging Experience

Navigation

App

Lighting

Interior

---

## Layer 3

Profile Evaluation

Different users

Different priorities

Different weights

---

# Score Types

Every vehicle receives five independent scores.
Die Kriterien werden künftig in vier Ebenen eingeteilt:

Ebene	    Beispiel
Fact	    Akku 84 kWh
Feature	    V2L vorhanden
Behaviour	Tempolimit wird direkt am Schild übernommen
Experience	Sitzkomfort auf Langstrecke

## Technical Score - Technische Daten

Measures

objective technical capabilities.

Examples

Battery

Charging

Efficiency

Packaging

---

## Functional Score - Umsetzung der Funktionen

Measures

quality of implementation.

Examples

Driver assistance

OTA

Navigation

App

Seats

Interior

---

## Profile Score - Übereinstimmung zum Nutzerprofil

Measures

how well the vehicle matches a specific user profile.

This score is profile dependent.

---

## Confidence Score - Aussagekraft der Bewertung

Measures

how reliable the current evaluation is.

Confidence is NOT a quality score.

---

## Value Score - Preis-Leistungs-Verhältnis

price-performance ratio

---

# KO Criteria

KO criteria are mandatory requirements.

Vehicles failing one or more KO criteria cannot receive a recommendation for the corresponding user profile.

Example

Required

V2L

Vehicle

No V2L

Result

Not recommended for "Long Distance & Resilience"

even if the overall score is very high.

---

# Weighting

Weights are never hard coded.

Weights belong to

profiles.

Every profile defines

- mandatory requirements
- weighting
- optional bonus criteria

---

# Rating Scale

Objective data are not rated directly.

Only functional characteristics receive points.

| Score | Meaning |
|-------:|---------|
| 10 | Reference class |
| 9 | Excellent |
| 8 | Very good |
| 7 | Good |
| 6 | Above average |
| 5 | Average |
| 4 | Below average |
| 3 | Weak |
| 2 | Poor |
| 1 | Very poor |
| 0 | Not available / unusable |

---

# Source Quality

Every rating references one or more sources.

Examples

Manufacturer

Independent test

Long-term review

Owner experience

Own testing

---

# Review Date

Every rating includes

- review date

- software version

- evaluator

- source

This enables long-term tracking of OTA improvements.

---

# Future Extensions

The scoring model is intentionally designed to support

- additional user profiles

- new vehicle technologies

- future charging standards

- new assistance systems

without requiring architectural changes.

---

# Summary

The EV-Decision-2027 scoring model is based on

- objective facts

- documented evidence

- transparent weighting

- explainable calculations

rather than subjective overall impressions.