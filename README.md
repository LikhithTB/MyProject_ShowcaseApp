# MyProject_ShowcaseApp

**Individual Project – Problem Statement #04: Student Project Portfolio & Showcase App**

A web/mobile app for a student project expo: teams publish showcase profiles with verified GitHub links, panel judges score projects with a weighted digital rubric, the public votes once per project after OTP verification, and a real-time leaderboard combines both. Suspicious voting or scoring patterns are flagged for organiser review.

**Actors:** Student Team, Panel Judge, Public Voter

## Repository Structure

| Folder | Contents | Status |
|---|---|---|
| `1_RE` | FR & NFR requirements table, RTM table, use-case diagram, UC-05 flow specification | Done |
| `2_Architecture` | UML component diagram (Microservices) + one-page architecture justification | Done |
| `3_Project_Creation_Screenshots` | GitHub and Jira project creation screenshots | Add screenshots |
| `4_SRS_and_WBS` | Software Requirements Specification and Work Breakdown Structure | Done |
| `5_Copilot_Code` | GitHub Copilot generated code screenshots / repository link | To be added later |
| `6_Software_Testing` | Testing-tool practice, bug fix and retest repository link | To be added later |

## Key Requirements
- FR-001 – Showcase profiles with verified GitHub URL
- FR-002 – Weighted digital rubric judging
- FR-003 – One vote per project, OTP-verified identity
- FR-004 – Leaderboard from normalised scores + votes
- FR-005 – Automatic organiser review queue
- NFR-001 – API latency under 300 ms
- NFR-002 – 3,000 concurrent users, failure rate at most 0.5%

## Architecture
Microservices behind an API Gateway (Profile, OTP Verification, Voting, Judging, Leaderboard, Review Monitor) connected by an Event Bus. See `2_Architecture/Component_Diagram.png`.
