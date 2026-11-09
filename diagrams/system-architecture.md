# High-level architecture (Mermaid)

```mermaid
flowchart LR
    T[Teacher / Authorized User] --> UI[Web Application]
    UI --> API[FastAPI Application]
    API --> OBJ[Cloud Object Storage]
    API --> Q[Background Task Queue]
    Q --> W[Recognition Worker]
    W --> CV[Face Detection & Embedding Pipeline]
    CV --> MATCH[Class-Scoped Identity Matching]
    MATCH --> DB[(PostgreSQL + Vector Extension)]
    W --> CACHE[(Redis)]
    CACHE --> API
    API --> REVIEW[Attendance Review & Correction]
    REVIEW --> DB
    DB --> REPORTS[Attendance Records & Reports]
    REPORTS --> UI
```

This diagram is intentionally high-level. Do not add internal routes, network boundaries, credentials, exact data schemas, recognition thresholds, security controls or private infrastructure details to the public version.
