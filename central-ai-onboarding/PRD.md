# Central AI Onboarding Redesign — Mini PRD

**Owner:** Serena  
**Type:** Independent targeted portfolio case  
**Affiliation:** None. This is not employer work and is not endorsed by Wing / Central AI.

## 1. Problem hypothesis
A broad AI platform can create onboarding friction when a new SMB user is asked to understand multiple modules and integrations before experiencing useful AI output.

This hypothesis should be validated using real funnel data, support tickets, onboarding observation and user interviews.

## 2. Goal
Reduce time from signup to the first successful AI-assisted action.

## 3. Proposed user journey
1. Ask the user what outcome they want first.
2. Reveal only the integration needed for that outcome.
3. Ask for bounded AI permissions.
4. Generate the first useful output.
5. Ask the user to approve or edit the first AI action.
6. Recommend the next relevant capability only after activation.

## 4. Example user story
As a small-business owner, I want Central to guide me through the shortest setup path for the job I care about, so I can experience value without first learning every product module.

## 5. Acceptance criteria
- The user can select a primary desired outcome.
- Only required setup steps are shown before first value.
- The user can see what permissions AI is requesting.
- The onboarding flow ends in a useful AI output, not merely a success screen.
- The first material action requires user approval in the prototype concept.
- Secondary modules are progressively disclosed after activation.

## 6. Proposed events
- `onboarding_goal_selected`
- `integration_started`
- `integration_connected`
- `permission_configured`
- `first_ai_output_generated`
- `first_ai_action_approved`
- `first_ai_action_edited`
- `next_module_opened`

## 7. Primary metrics
- First-successful-AI-action rate within 24 hours.
- Time to First Value.
- Step-level onboarding drop-off.
- D1 / D7 return among activated users.
- Edit/approval rate on the first AI action.

## 8. Validation plan
- Compare outcome-first onboarding vs current/default flow in a controlled experiment.
- Review session recordings for hesitation and abandoned integrations.
- Interview newly activated and non-activated users.
- Track which outcomes lead to fastest first value and strongest D7 return.

## 9. Portfolio caveat
No production user data, conversion numbers or internal Central AI metrics are claimed in this case.