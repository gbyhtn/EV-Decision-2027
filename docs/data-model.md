# Data Model

Version: 0.1 (Draft)

---

# Purpose

The data model defines the logical structure of all information managed within the EV-Decision-2027 project.

Its purpose is to ensure that vehicle evaluations remain transparent, reproducible and extensible over time.

This document describes the conceptual model and is intentionally independent of any specific implementation (SQLite, CSV, JSON, etc.).

---

# Design Goals

The data model shall be:

* Modular
* Explainable
* Extensible
* Versionable
* Technology independent

The same conceptual model shall support:

* SQLite database
* CSV import/export
* Excel reporting
* Python evaluation engine
* Future web applications

---

# Core Principles

## Separation of Concerns

Objective facts and subjective evaluations are stored separately.

Technical specifications must never be mixed with ratings or opinions.

---

## Traceability

Every subjective assessment must reference one or more documented sources.

Each rating shall include:

* evaluator
* review date
* software version (if applicable)
* confidence level

---

## OTA Awareness

Vehicle capabilities may change over time through software updates.

The data model therefore supports versioned software information.

---

# Domain Model

The project is organised around the following core entities.

## Vehicle

Represents a specific vehicle configuration.

Examples:

* Volkswagen ID.7 Pro S
* BMW iX3 Neue Klasse
* Mercedes CLA EV
* XPENG G6

Attributes include:

* Manufacturer
* Model
* Variant
* Model Year
* Platform
* Drive Type
* Battery
* Powertrain

---

## Technical Specification

Contains objective technical information.

Examples:

* Battery capacity
* Battery chemistry
* Charging power
* Vehicle dimensions
* Weight
* Drag coefficient
* Drive system
* Suspension

Technical specifications are factual and do not receive scores.

---

## Feature

Represents the presence or absence of a function.

Examples:

* V2L
* Matrix LED
* Head-Up Display
* Heat Pump
* Frunk
* Digital Key

A feature may also contain additional metadata such as regional availability or optional equipment.

---

## Behaviour

Describes how a feature performs in real-world use.

Examples:

* Speed adaptation at traffic signs
* Lane centering quality
* Charging planner reliability
* Navigation rerouting
* One-pedal driving behaviour

Behaviour is evaluated using documented observations.

---

## Experience

Represents long-term user impressions.

Examples:

* Seat comfort
* Material quality
* Cabin noise
* Software usability
* Ergonomics
* Ride comfort

Experience is subjective and therefore always linked to evidence and confidence.

---

## Criterion

Represents a single evaluation criterion.

Each criterion belongs to one functional category.

Examples:

* V2L
* DC charging
* Driver assistance
* OTA updates
* Matrix LED

Criteria define what can be evaluated.

---

## Category

Groups related criteria.

Examples:

* Battery
* Charging
* Assistance
* Software
* Interior
* Lighting
* Comfort
* Safety

Categories simplify reporting and weighting.

---

## Profile

Represents a user-specific evaluation profile.

Examples:

* Long Distance & Resilience
* Family
* Business
* Technology Enthusiast
* Budget

Profiles define:

* mandatory criteria
* weighting
* bonus criteria

---

## Rating

Represents an evaluation result for one criterion.

Attributes:

* Score
* Confidence
* Comment
* Evaluator
* Review Date
* Software Version
* Source Reference

---

## Source

Represents evidence supporting a rating.

Possible source types:

* Manufacturer
* Independent Test
* Long-term Test
* Owner Experience
* Scientific Publication
* Own Evaluation

Every source includes:

* publication date
* URL or reference
* source quality
* language

---

## Software Version

Represents the software state of a vehicle.

Examples:

* Infotainment Version
* ADAS Version
* Navigation Version

Ratings may depend on a specific software version.

---

# Relationships

The conceptual relationships are:

Vehicle

→ Technical Specification

→ Features

→ Software Versions

→ Ratings

Ratings

→ Criterion

→ Source

→ Evaluator

Profiles

→ Criteria

→ Weightings

Categories

→ Criteria

---

# Evaluation Flow

Vehicle

↓

Technical Data

↓

Features

↓

Behaviour

↓

Experience

↓

Ratings

↓

Profile Weighting

↓

Recommendation

---

# Versioning

Vehicle information evolves over time.

Changes may result from:

* OTA updates
* Facelifts
* Hardware revisions
* New measurements
* Additional testing

Historical evaluations should remain reproducible.

---

# Future Extensions

The data model is intentionally designed to support:

* new battery technologies
* bidirectional charging
* autonomous driving
* additional user profiles
* commercial vehicles
* future EV standards

without requiring structural redesign.

---

# Summary

The EV-Decision-2027 data model separates facts, functionality, behaviour, experience and evaluation into clearly defined entities.

This separation ensures that every recommendation remains transparent, evidence-based and reproducible while allowing the project to evolve alongside future vehicle technologies.
