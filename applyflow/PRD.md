# ApplyFlow AI — MVP Product Requirements

**Owner:** Serena  
**Status:** Independent portfolio case  
**Data:** Synthetic only

## 1. Problem
Application consultants may manage applicant status across chat, spreadsheets, documents, email, calendars and university portals. This creates coordination risk: missing materials, unclear ownership and deadlines that are discovered too late.

## 2. MVP goal
Help a consultant identify the highest-risk applications and the next operational action in under one minute.

## 3. Primary user
Application consultant / operations coordinator managing multiple active applicants.

## 4. Core jobs to be done
- See which applicants require attention today.
- Understand why a case is risky.
- Ask cross-record questions in natural language.
- Create or trigger a follow-up action.

## 5. MVP scope
1. Student status dashboard.
2. Document completeness model.
3. Deadline-distance calculation.
4. Risk prioritisation rules.
5. AI summary over structured records.
6. Recommended next best action.
7. Manual approval before sending reminders or changing status.

## 6. Out of scope
- Admissions prediction.
- Automated submission to university portals.
- Fabrication or inference of missing applicant facts.
- Autonomous changes to verified academic or identity data.

## 7. Example user story
As an application consultant, I want to see applicants with deadlines in the next 14 days who still have missing required documents, so I can prioritise follow-up before the application becomes at risk.

## 8. Acceptance criteria
- A user can view applicants sorted by risk.
- Each high-risk case shows deadline distance and the missing dependency.
- Ask AI can answer predefined structured-data questions without inventing missing facts.
- Suggested actions require user confirmation.
- The UI labels synthetic/demo data clearly.

## 9. Product events
- `dashboard_viewed`
- `high_risk_case_opened`
- `ask_ai_query_submitted`
- `ai_recommendation_viewed`
- `recommendation_accepted`
- `recommendation_edited`
- `followup_task_created`
- `risk_case_resolved`

## 10. Proposed metrics
- Time to identify first high-risk case.
- Missed-deadline rate.
- High-risk case resolution lead time.
- AI recommendation acceptance/edit rate.
- Repeat weekly use.

## 11. AI boundary
Structured applicant records remain the source of truth. AI may summarise, compare, prioritise and recommend next actions, but it must not invent applicant facts or silently change verified status.