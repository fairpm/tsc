# Release Calendar

## Overview
The FAIR project follows a structured release cadence with three 16-week milestone cycles per year, followed by a 4-week reset period.

## Key Terms
- **MC** = Milestone Cycle (16 weeks each)
- **RC** = Release Cycle (8 weeks each, 2 per milestone)
- **Weeks** = ISO-8601 week numbers

## Structure
Each Milestone Cycle contains:
- Two 8-week Release Cycles
- Sprint phases: Development → Alpha → Beta (Feature Freeze) → RC → Release
- 6-day buffer after Tuesday releases

```mermaid
%%{init: {'theme':'neutral'}}%%

gantt
    title FAIR Milestones & Release Cadence (16 Weeks per Milestone) - 2026
    dateFormat YYYY-MM-DD
    axisFormat %b %d
    
    section MC1
    MC1 (Jan 5 - May 3)     :mc1, 2026-01-05, 2026-05-03
    RC1 (Jan 5 - Mar 1)      :rc1_1, 2026-01-05, 2026-03-01
    RC2 (Mar 2 - May 3)    :rc1_2, 2026-03-02, 2026-05-03
    
    section MC2
    MC2 (May 4 - Aug 23)   :mc2, 2026-05-04, 2026-08-23
    RC1 (May 4 - Jun 28)   :rc2_1, 2026-05-04, 2026-06-28
    RC2 (Jun 29 - Aug 23)  :rc2_2, 2026-06-29, 2026-08-23
    
    section MC3
    MC3 (Aug 24 - Nov 29)  :mc3, 2026-08-24, 2026-11-29
    RC1 (Aug 24 - Oct 18)  :rc3_1, 2026-08-24, 2026-10-18
    RC2 (Oct 19 - Nov 29)  :rc3_2, 2026-10-19, 2026-11-29
    
    section Reset Period
    Reset (Nov 30 - Dec 27) :reset, 2026-11-30, 2026-12-27
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

### MC1: January 5 - May 3 (ISO Weeks 2-18)
- **RC1**: January 5 - March 1 (Weeks 2-9)
- **RC2**: March 2 - May 3 (Weeks 10-18)

### MC2: May 4 - August 23 (ISO Weeks 19-34)
- **RC1**: May 4 - June 28 (Weeks 19-26)
- **RC2**: June 29 - August 23 (Weeks 27-34)

### MC3: August 24 - November 29 (ISO Weeks 35-48)
- **RC1**: August 24 - October 18 (Weeks 35-42)
- **RC2**: October 19 - November 29 (Weeks 43-48)

### Reset Period: November 30 - December 27 (ISO Weeks 49-52)
- 4-week break for planning, infrastructure updates, and team downtime
