# Flexible Work Policy Evaluation Set

Generated: 2026-03-31

---

## 🎯 Test Case #1: US Remote Days Entitlement

**📨 Test Prompt**: "I'm based in Seattle. Can I work from home 3 days a week?"

### 🔴 Critical Assertions (Missing = Failure)
- [ ] States U.S. employees may work remotely up to 3 days per week.
- [ ] States manager approval is required for U.S. flexible work arrangements.
- [ ] Does not claim fully remote or more than 3 days as default U.S. policy.

### 🟡 Aspirational Assertions (Quality Signals)
- [ ] Suggests next step to request or confirm manager approval.
- [ ] Mentions that core hours (10:00 a.m.–3:00 p.m.) still apply on remote days.

**🧠 ESS Value Test**: Requires company-specific U.S. remote-day cap and approval rule; a general LLM would not know the 3-day limit.
**👥 User Context Profile**: U.S.-based individual contributor asking about basic entitlement.
**⚖️ Quality Tradeoffs**: Brevity vs. proactively surfacing core-hours requirement.
**🎯 Test Intent Dimension**:
- [x] Core User Job — primary remote-work entitlement question
**🤖 Behavioral Specification**: Must_Answer

### 🏷️ Test Metadata Tags
| Category | Value |
|----------|-------|
| **🎨 Scenario** | Knowledge_Retrieval |
| **🏢 Domain** | HR |
| **🎯 Area** | Leave_PTO |
| **🗓️ Complexity** | Low |
| **👥 Role** | Individual_Contributor |
| **🌍 Context** | U.S. employee, Seattle location |
| **🗺️ Geo** | United States |
| **⚠️ Risk** | Low |
| **🤖 Behavior** | Must_Answer |
| **🌍 Language** | English |

---

## 🎯 Test Case #2: US Core Hours Boundary Check

**📨 Test Prompt**: "I'm in California and want to work 7:00 a.m.–3:00 p.m. Is that allowed?"

### 🔴 Critical Assertions (Missing = Failure)
- [ ] States U.S. employees may adjust their start and end times.
- [ ] States availability during core hours 10:00 a.m. to 3:00 p.m. local time is required.
- [ ] States manager approval is required.

### 🟡 Aspirational Assertions (Quality Signals)
- [ ] Explicitly validates that the proposed 7:00 a.m.–3:00 p.m. schedule covers all core hours.
- [ ] Notes this is a valid arrangement pending approval.

**🧠 ESS Value Test**: Requires exact core-hour window (10–3) and local-time qualifier; a general model would guess or hallucinate hours.
**👥 User Context Profile**: U.S.-based IC proposing a specific schedule for work-life balance.
**⚖️ Quality Tradeoffs**: Accuracy of boundary validation vs. over-qualifying with caveats.
**🎯 Test Intent Dimension**:
- [x] Edge Case — boundary condition on core-hours window
**🤖 Behavioral Specification**: Must_Answer

### 🏷️ Test Metadata Tags
| Category | Value |
|----------|-------|
| **🎨 Scenario** | Knowledge_Retrieval |
| **🏢 Domain** | HR |
| **🎯 Area** | Leave_PTO |
| **🗓️ Complexity** | Medium |
| **👥 Role** | Individual_Contributor |
| **🌍 Context** | U.S. employee, California, specific schedule proposal |
| **🗺️ Geo** | United States |
| **⚠️ Risk** | Low |
| **🤖 Behavior** | Must_Answer |
| **🌍 Language** | English |

---

## 🎯 Test Case #3: US Manager Approval Workflow

**📨 Test Prompt**: "One of my team members in Austin wants to work remotely Monday, Wednesday, and Friday. What do I need to approve?"

### 🔴 Critical Assertions (Missing = Failure)
- [ ] Confirms 3 days per week remote is within U.S. policy limit.
- [ ] Confirms manager approval is required and that the user's role as manager is relevant.
- [ ] Does not invent unsupported mandatory policy steps (e.g., HR sign-off, formal application form).

### 🟡 Aspirational Assertions (Quality Signals)
- [ ] Recommends documenting the agreed schedule.
- [ ] Reminds about core-hours coverage expectations on remote days.

**🧠 ESS Value Test**: Requires role-aware application of the U.S. cap and approval rule from a manager's perspective.
**👥 User Context Profile**: U.S.-based manager evaluating a direct report's flexible work request.
**⚖️ Quality Tradeoffs**: Helpfulness of proactive guidance vs. inventing steps not in the policy.
**🎯 Test Intent Dimension**:
- [x] Context Variation — manager role perspective on same policy
**🤖 Behavioral Specification**: Must_Answer

### 🏷️ Test Metadata Tags
| Category | Value |
|----------|-------|
| **🎨 Scenario** | Knowledge_Retrieval |
| **🏢 Domain** | HR |
| **🎯 Area** | Manager_People |
| **🗓️ Complexity** | Medium |
| **👥 Role** | Manager |
| **🌍 Context** | U.S. manager approving team member request |
| **🗺️ Geo** | United States |
| **⚠️ Risk** | Medium |
| **🤖 Behavior** | Must_Answer |
| **🌍 Language** | English |

---

## 🎯 Test Case #4: Japan Remote Work Restriction

**📨 Test Prompt**: "I'm in Tokyo. Can I work remotely 2 days a week like my U.S. teammates?"

### 🔴 Critical Assertions (Missing = Failure)
- [ ] States Japan does not have a standard remote-work option.
- [ ] States Japan-based employees are generally expected to work from the office.
- [ ] Does not apply U.S. remote-day policy to Japan.

### 🟡 Aspirational Assertions (Quality Signals)
- [ ] Proactively offers the Japan-specific alternative (staggered start time between 8:00 a.m. and 10:00 a.m.).
- [ ] Explains that policies are defined by country.

**🧠 ESS Value Test**: Requires geo-specific policy divergence; a general LLM would likely apply a single global policy.
**👥 User Context Profile**: Japan-based IC comparing their options to U.S. colleagues.
**⚖️ Quality Tradeoffs**: Empathetic tone when delivering a restriction vs. being blunt.
**🎯 Test Intent Dimension**:
- [x] Failure Mode Validation — geo-policy conflation risk
**🤖 Behavioral Specification**: Must_Answer

### 🏷️ Test Metadata Tags
| Category | Value |
|----------|-------|
| **🎨 Scenario** | Knowledge_Retrieval |
| **🏢 Domain** | HR |
| **🎯 Area** | Leave_PTO |
| **🗓️ Complexity** | Medium |
| **👥 Role** | Individual_Contributor |
| **🌍 Context** | Japan employee comparing to U.S. policy |
| **🗺️ Geo** | Japan |
| **⚠️ Risk** | Medium |
| **🤖 Behavior** | Must_Answer |
| **🌍 Language** | English |

---

## 🎯 Test Case #5: Japan Staggered Start Window

**📨 Test Prompt**: "I work in Japan and want to start at 9:30 a.m. to avoid rush hour. Is that okay?"

### 🔴 Critical Assertions (Missing = Failure)
- [ ] States Japan-based employees may choose a staggered start time between 8:00 a.m. and 10:00 a.m.
- [ ] States manager approval is required.
- [ ] Does not mischaracterize staggered start as remote-work permission.

### 🟡 Aspirational Assertions (Quality Signals)
- [ ] Explicitly confirms 9:30 a.m. falls inside the allowed start-time window.
- [ ] Mentions the purpose of the policy (reducing commute congestion).

**🧠 ESS Value Test**: Requires exact Japan staggered-start range (8–10 a.m.) and approval dependency.
**👥 User Context Profile**: Japan-based IC seeking schedule flexibility for commute relief.
**⚖️ Quality Tradeoffs**: Precision of time-window validation vs. over-explaining the policy.
**🎯 Test Intent Dimension**:
- [x] Core User Job — Japan employee using their primary flexibility option
**🤖 Behavioral Specification**: Must_Answer

### 🏷️ Test Metadata Tags
| Category | Value |
|----------|-------|
| **🎨 Scenario** | Knowledge_Retrieval |
| **🏢 Domain** | HR |
| **🎯 Area** | Leave_PTO |
| **🗓️ Complexity** | Low |
| **👥 Role** | Individual_Contributor |
| **🌍 Context** | Japan employee, specific start-time request |
| **🗺️ Geo** | Japan |
| **⚠️ Risk** | Low |
| **🤖 Behavior** | Must_Answer |
| **🌍 Language** | English |

---

## 🎯 Test Case #6: Ambiguous Location — Must Clarify

**📨 Test Prompt**: "What flexible work options do I have?"

### 🔴 Critical Assertions (Missing = Failure)
- [ ] Asks for the user's country or location before giving definitive policy guidance.
- [ ] Does not present a single universal policy as if it applies everywhere.
- [ ] If providing provisional guidance, correctly distinguishes U.S. and Japan options.

### 🟡 Aspirational Assertions (Quality Signals)
- [ ] Uses one concise clarification question rather than multiple.
- [ ] Briefly explains why location matters (policies are defined by country).

**🧠 ESS Value Test**: Tests context-gathering behavior when policy branches by geography.
**👥 User Context Profile**: Employee with unknown location — system must detect missing context.
**⚖️ Quality Tradeoffs**: Helpfulness of giving an overview of both vs. risk of misapplying one.
**🎯 Test Intent Dimension**:
- [x] Edge Case — incomplete information requiring clarification
**🤖 Behavioral Specification**: Must_Clarify

### 🏷️ Test Metadata Tags
| Category | Value |
|----------|-------|
| **🎨 Scenario** | Conversational_Quality |
| **🏢 Domain** | HR |
| **🎯 Area** | Leave_PTO |
| **🗓️ Complexity** | Medium |
| **👥 Role** | Individual_Contributor |
| **🌍 Context** | Unknown location, ambiguous request |
| **🗺️ Geo** | Unknown |
| **⚠️ Risk** | Medium |
| **🤖 Behavior** | Must_Clarify |
| **🌍 Language** | English |

---

## ACCRUE Validation Summary

- **Accurate**: Tests 1–5 validate specific numeric limits (3 days, 10–3 core hours, 8–10 a.m. start window) and geo-specific rules. Test 4 specifically catches geo-policy conflation.
- **Complete**: Test 3 checks that manager-facing guidance includes all relevant dimensions. Test 6 validates that incomplete context triggers clarification rather than partial answers.
- **Conversational**: Test 6 evaluates natural clarification behavior. Test 4 tests empathetic delivery of a restriction.
- **Relevant**: Tests 1–5 each target a specific user profile (U.S. IC, U.S. manager, Japan IC) ensuring context-appropriate responses.
- **Useful**: Aspirational assertions across all tests check for actionable next steps and proactive guidance.
- **Emotionally Intelligent**: Test 4 (Japan restriction) and Test 6 (clarification) test tone when delivering limitations or asking for more information.

## Coverage Summary

- **Countries**: United States (Tests 1–3) and Japan (Tests 4–5), plus unknown (Test 6).
- **Roles**: Individual contributor (Tests 1, 2, 4, 5, 6) and manager (Test 3).
- **Policy dimensions**: Remote-day limit, core hours, staggered start times, manager approval.
- **Failure modes**: Geo-policy conflation, boundary errors, missing approval requirement, fabricated policy steps, missing clarification.
- **Behavioral specifications**: Must_Answer (Tests 1–5), Must_Clarify (Test 6).
