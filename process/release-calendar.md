# Release Calendar

## Overview
The FAIR project follows a structured release cadence with three 16-week milestone cycles per year, followed by a 4-week reset period. The purpose of these named milestone releases is to help coordinate the many projects and working groups within FAIR, allowing FAIR's TSC to set major themes or objectives for each milestone, and have each WG and software project under its banner work toward those common goals.

An 8-week cadence for release cycles is shown below as a typical but not mandated schedule. FAIR maintains multiple software projects to meet its objectives, and not all will follow this cadence, with some perhaps doing only one release per milestone, and others potentially more, particularly where smaller changes are deployed. These releases are generally indicated by version numbering, with semantic versioning recommended. Following FAIR's "Version 1.0" milestone, version numbers are not intended to remain synchronized between different software projects. An 8-week cadence for release cycles is intended as a typical but not mandated schedule. FAIR maintains multiple software projects to meet its objectives. Working groups responsible for each software release will adopt an appropriate cadence for the project that includes at lease one release per milestone. For example, AspireCloud follows a release-when-ready model, with small changes released often and larger ones on a planned schedule toward a named release.

## Key Terms
- **M#** = Milestone Cycle (16 weeks each)
- **R#** = Release Cycle (_e.g._, 8 weeks each, 2 per milestone)
- **Weeks** = ISO-8601 week numbers

## Structure
Each Milestone Cycle contains:
- Typically Two 8-week Release Cycles (or other appropriate cadence _within_ the 16-week milestone)
- Typical sprint phases: Development → Alpha → Beta (Feature Freeze) → RC → Release
- Typically, a 6-day buffer after each Tuesday release dates

```mermaid
%%{init: {'theme':'neutral'}}%%

gantt
    title FAIR Milestones & Release Cadence (16 Weeks per Milestone) - 2026
    dateFormat YYYY-MM-DD
    axisFormat %b %d
    
    section M1
    M1 (Jan 5 - Apr 26)     :m1, 2026-01-05, 2026-04-26
    R1 (Jan 5 - Mar 1)      :r1_1, 2026-01-05, 2026-03-01
    R2 (Mar 2 - Apr 26)     :r1_2, 2026-03-02, 2026-04-26
    
    section M2
    M2 (Apr 27 - Aug 16)   :m2, 2026-04-27, 2026-08-16
    R1 (Apr 27 - Jun 21)   :r2_1, 2026-04-27, 2026-06-21
    R2 (Jun 22 - Aug 16)   :r2_2, 2026-06-22, 2026-08-16
    
    section M3
    M3 (Aug 17 - Dec 6)   :m3, 2026-08-17, 2026-12-06
    R1 (Aug 17 - Oct 11)  :r3_1, 2026-08-17, 2026-10-11
    R2 (Oct 12 - Dec 6)   :r3_2, 2026-10-12, 2026-12-06
    
    section Reset Period
    Reset (Dec 7 - Jan 3) :reset, 2026-12-07, 2027-01-03
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
    Beta --> RC[Week 7: RC<br/>Release Checklist]
    
    RC --> Release[Week 8: Tuesday Release<br/>+ 6-Day Buffer]
    Release --> End([Cycle Complete])
    
    style Dev fill:#e1f5ff
    style Test fill:#fff4e1
    style Release fill:#e1ffe1
```

## 2026 Milestone Cycles

### M1: January 5 - Apr 26 (ISO Weeks 2-17)
- **R1**: January 5 - March 1 (Weeks 2-9)
- **R2**: March 2 - Apr 26 (Weeks 10-17)

### M2: Apr 27 - August 16 (ISO Weeks 18-33)
- **R1**: Apr 27 - June 21 (Weeks 18-25)
- **R2**: June 22 - August 16 (Weeks 26-33)

### M3: August 17 - December 6 (ISO Weeks 34-49)
- **R1**: August 17 - October 11 (Weeks 34-41)
- **R2**: October 12 - December 6 (Weeks 42-48)

### Reset Period: December 7 - January 3 (ISO Weeks 49-52)
- 4-week break for planning, infrastructure updates, and team downtime
