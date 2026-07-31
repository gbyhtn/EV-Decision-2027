# Architecture

## Overview

```
                Data Sources
                     │
                     ▼
              Normalized Database
                     │
                     ▼
             Scoring Engine
                     │
        ┌────────────┴────────────┐
        ▼                         ▼
   Excel Export             Future Web UI
```

---

## Components

### Data

Objective vehicle information

### Ratings

Subjective assessments

### Sources

Evidence for every rating

### Profiles

Different user priorities

### Reports

Automatically generated summaries

---

## Design Goals

- Modular
- Explainable
- Version controlled
- Extensible
- Platform independent