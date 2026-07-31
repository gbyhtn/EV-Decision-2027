# Glossary

Version: 0.1 (Draft)

---

# Purpose

This glossary defines the terminology used throughout the EV-Decision-2027 project.

Its purpose is to ensure that documentation, data models, scoring rules and future implementations use a consistent vocabulary.

Whenever a term is defined here, this definition takes precedence over manufacturer-specific terminology.

---

# 1. General Terms

## Electric Vehicle (EV)

A vehicle powered exclusively by electric motors using energy stored in a rechargeable battery.

---

## Vehicle

A uniquely identifiable vehicle variant that can be evaluated.

Example:

* Volkswagen ID.7 Pro S
* Mercedes-Benz CLA 350+
* XPENG G6 AWD

---

## Manufacturer

The company responsible for designing and producing the vehicle.

---

## Model

The commercial product name assigned by the manufacturer.

---

## Variant

A specific configuration of a model, defined by drivetrain, battery, trim level or other distinguishing characteristics.

---

## Model Year

The manufacturer-defined production year of a vehicle.

---

## Platform

The technical vehicle architecture shared between one or more models.

Examples:

* MEB
* PPE
* MMA
* Neue Klasse

---

# 2. Battery

## Battery Capacity (Gross)

The total energy capacity of the battery.

---

## Battery Capacity (Net)

The usable energy available to the driver.

---

## Battery Chemistry

The electrochemical technology used by the battery.

Examples:

* LFP
* NMC
* NCA

---

## State of Charge (SoC)

The current battery charge expressed as a percentage of usable capacity.

---

## Battery Preconditioning

Automatic preparation of the battery to achieve optimal charging performance.

---

# 3. Charging

## AC Charging

Charging using alternating current.

---

## DC Charging

Charging using direct current.

---

## Charging Curve

The relationship between charging power and battery state of charge.

---

## Charging Planner

Software that plans charging stops during navigation.

---

## Vehicle-to-Load (V2L)

The ability to supply external electrical devices directly from the vehicle battery without requiring a bidirectional charging station.

---

## Vehicle-to-Home (V2H)

The ability to supply electrical energy to a building.

---

## Vehicle-to-Grid (V2G)

The ability to exchange electrical energy with the public electricity grid.

---

# 4. Driver Assistance

## ADAS

Advanced Driver Assistance Systems.

Collective term for electronic systems supporting the driver.

---

## Adaptive Cruise Control (ACC)

Automatically maintains a selected speed and following distance.

---

## Lane Centering

Continuously keeps the vehicle centred within the lane.

---

## Traffic Sign Recognition

Detection and interpretation of traffic signs.

---

## Speed Adaptation

Automatic adjustment of the target speed based on recognised speed limits or navigation data.

---

# 5. Software

## Over-the-Air Update (OTA)

Software update delivered remotely without requiring a workshop visit.

---

## Software Version

The documented software state of the evaluated vehicle.

---

## Digital Key

A system allowing authorised access and vehicle operation using a smartphone or compatible device.

---

## Infotainment System

The integrated user interface providing navigation, media, connectivity and vehicle settings.

---

# 6. Vehicle Features

## Feature

A function or equipment item that is available for a vehicle.

A feature describes **whether** a capability exists, not **how well** it performs.

Examples:

* Heat Pump
* Matrix LED
* Head-Up Display
* Digital Key
* V2L
* Frunk

---

## Equipment Package

A predefined group of optional or standard features offered together by the manufacturer.

---

## Standard Equipment

A feature included in the base specification of a vehicle variant.

---

## Optional Equipment

A feature requiring an additional package or individual option.

---

# 7. Evaluation

## Criterion

A measurable aspect used during vehicle evaluation.

---

## Category

A logical grouping of related criteria.

Examples:

* Charging
* Software
* Interior
* Driver Assistance

---

## Profile

A configurable set of priorities representing a specific user type.

Examples:

* Long Distance & Resilience
* Family
* Business
* Budget

---

## Weight

The importance assigned to a criterion within a profile.

---

## KO Criterion

A mandatory requirement.

Failure to meet a KO criterion excludes a vehicle from recommendation for the corresponding profile, regardless of its overall score.

---

## Rating

The numerical evaluation assigned to a criterion.

---

## Technical Score

Aggregated score based on objective technical characteristics.

---

## Functional Score

Aggregated score describing the quality of implemented vehicle functions.

---

## Profile Score

Aggregated score describing how well a vehicle matches a specific user profile.

---

## Confidence Score

A measure of how reliable the current evaluation is.

It represents confidence in the assessment, not vehicle quality.

---

## Value Score

A measure of value relative to purchase price and ownership costs.

This score is intentionally independent from the Technical Score.

---

## Recommendation

The final result of the evaluation process for a given user profile.

---

# 8. Data Model

## Technical Specification

Objective vehicle characteristics that can be verified independently.

---

## Behaviour

Observable behaviour of a feature under defined conditions.

Examples:

* Speed adaptation timing
* Lane centering quality
* Navigation reliability

---

## Experience

Subjective long-term impressions resulting from vehicle use.

Examples:

* Seat comfort
* Cabin ergonomics
* Perceived software usability

---

## Source

Documented evidence supporting an evaluation.

---

## Observation

A documented factual observation made during testing or vehicle use.

Observations may contribute to one or more ratings but are not ratings themselves.

---

## Region

A market or geographical area where specifications, software or available equipment may differ.

Examples:

* Europe
* North America
* China

---

# 9. Source Types

## Manufacturer

Information published by the vehicle manufacturer.

---

## Independent Test

Professional evaluation conducted by an independent organisation.

---

## Long-Term Test

Evaluation based on extended real-world vehicle usage.

---

## Owner Experience

Documented experience reported by vehicle owners.

---

## Own Evaluation

Assessment performed directly within the EV-Decision-2027 project.

---

# Document Ownership

Changes to glossary definitions should be made carefully, as they may affect the interpretation of scoring rules, data models and historical evaluations.

Whenever possible, new terms should be added rather than redefining existing ones.
