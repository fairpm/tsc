# Release Calendar

## Overview
The FAIR project follows a structured release cadence with three 16-week milestone cycles per year, followed by a 4-week reset period.

## Key Terms
- **MC** = Milestone Cycle (16 weeks each)
- **Cycle** = Release Cycle (8 weeks each, 2 per milestone)
- **Weeks** = ISO-8601 week numbers

## Structure
Each Milestone Cycle contains:
- Two 8-week Release Cycles
- Sprint phases: Development → Alpha → Beta (Feature Freeze) → Cycle → Release
- 6-day buffer after Tuesday releases

```mermaid
%%{init: {'theme':'neutral'}}%%

gantt
    title FAIR Milestones & Release Cadence (16 Weeks per Milestone) - 2026
    dateFormat YYYY-MM-DD
    axisFormat %b %d
    
section MC1
    MC1 (Jan 5 - Apr 26)     :mc1, 2026-01-05, 2026-04-26
    Cycle1 (Jan 5 - Mar 1)      :Cycle1_1, 2026-01-05, 2026-03-01
    Cycle2 (Mar 2 - Apr 26)     :Cycle1_2, 2026-03-02, 2026-04-26
    
    section MC2
    MC2 (Apr 27 - Aug 16)    :mc2, 2026-04-27, 2026-08-16
    Cycle1 (Apr 27 - Jun 21)    :Cycle2_1, 2026-04-27, 2026-06-21
    Cycle2 (Jun 22 - Aug 16)    :Cycle2_2, 2026-06-22, 2026-08-16
    
    section MC3
    MC3 (Aug 17 - Dec 6)     :mc3, 2026-08-17, 2026-12-06
    Cycle1 (Aug 17 - Oct 11)    :Cycle3_1, 2026-08-17, 2026-10-11
    Cycle2 (Oct 12 - Dec 6)     :Cycle3_2, 2026-10-12, 2026-12-06
    
    section Reset Period
    Reset (Dec 7 - Jan 3)   :reset, 2026-12-07, 2027-01-03
```
## FAIR Release Cycle - Sprint & Phase Structure (8 Weeks)

```mermaid
%%{init: {'theme':'neutral'}}%%
flowchart LR
    Start([8-Week Release Cycle]) --> Dev{Development Phase<br/>Weeks 1-4}
    
    Dev -->|Option A| S1[Sprint 1<br/>Weeks 1-2<br/>Release Plan]
    S1 --> S2[Sprint 2<br/>Weeks 3-4]
    
    Dev -->|Option B| Alt[3-Week Dev Cycle<br/>Weeks 1-3<br/>2 Sprints to Beta]
    
    S2 --> Test[Testing Phase<br/>Weeks 5-7]
    Alt --> Test
    
    Test --> Alpha[Week 5: Alpha<br/>Testing]
    Alpha --> Beta[Week 6: Beta<br/>Feature Freeze]
    Beta --> Cycle[Week 7: Cycle<br/>Release Checklist]
    
    Cycle --> Release[Week 8: Tuesday Release<br/>+ 6-Day Buffer]
    Release --> End([Cycle Complete])
    
    style Dev fill:#e1f5ff
    style Test fill:#fff4e1
    style Release fill:#e1ffe1
```

## 2026 Milestone Cycles

### MC1: January 5 - April 26 (ISO Weeks 2-17)
- **Cycle1**: January 5 - March 1 (Weeks 2-9)
- **Cycle2**: March 2 - April 26 (Weeks 10-17)

### MC2: April 27 - August 16 (ISO Weeks 18-33)
- **Cycle1**: April 27 - June 21 (Weeks 18-25)
- **Cycle2**: June 22 - August 16 (Weeks 26-33)

### MC3: August 17 - December 6 (ISO Weeks 34-49)
- **Cycle1**: August 17 - October 11 (Weeks 34-41)
- **Cycle2**: October 12 - December 6 (Weeks 42-49)

### Reset Period: December 7 - January 3, 2027 (ISO Weeks 50-53)
- 4-week break for planning, infrastructure updates, and team downtime

