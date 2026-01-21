# RISQON Scoring Logic

**Status:** Locked – Data Room Version  
**Purpose:** Risk-awareness signaling and decision-support metadata only  
**Last updated:** 2026-01-21

RISQON is a standalone risk-awareness scoring system currently ~15% complete; the scoring engine structure is being refined to satisfy legal and compliance shoring requirements across U.S. healthcare systems. The document below reflects the authoritative operating design.

## 1. Relationship Between RISQON and MeducateX
- RISQON is an independent decision-support layer that may optionally integrate with MeducateX workflows; neither system is required for the other to operate.
- RISQON does not act on behalf of MeducateX, does not inherit clinical responsibilities, and does not represent MeducateX medical, legal, or institutional decisions.
- Any integration is technical/contextual only—it does not delegate organizational or enforcement authorities.

## 2. Scope of RISQON Scoring
- RISQON surfaces risk-awareness signals for human review and governance prioritization only.
- Scores do not represent medical advice, legal advice, approvals, denials, or validation of activities.
- RISQON does not replace institutional review, IRB processes, or compliance oversight—every outcome requires explicit human interpretation and action.

## 3. Three-Layer AI Filtering Architecture (Risk-Awareness Only)
RISQON employs AI layers to boost signal reliability and reduce false positives. No layer autonomously triggers enforcement.

**Layer 1 – Structural & Metadata Validation**  
- Validates required field presence, role/participation tagging consistency, governance tag completeness, and timestamp provenance.

**Layer 2 – Contextual Risk Pattern Detection**  
- Flags mismatches between procedure categories and governance tags, participation ambiguities, consent gaps, and atypical metadata requiring review.

**Layer 3 – Cross-Layer Consistency & Signal Confirmation**  
- Independently re-evaluates signals from Layers 1 and 2 to confirm persistence, downgrade noise, and concentrate rationale into a unified score.

## 4. Inputs Used for Scoring (Non-Clinical)
- Procedure/content category classifications  
- Participation and role attributions  
- Governance/compliance tags (IRB status, consent presence, retention indicators)  
- Content provenance and traceability references  
- Documentation completeness and structural integrity markers  
- Patient outcomes, clinical performance, and decision quality are excluded from RISQON analysis.

## 5. Output Definition
- RISQON issues a human-readable risk-awareness score with rationale describing what triggered the signal, which metadata elements are misaligned, and what category of review may be required.
- Scores are advisory only and carry no enforcement authority; they explicitly avoid any clinical decision-making posture.

## 6. Decision Boundary and Liability Position
- RISQON is a transparency and visibility tool, not an automated decision engine.
- Final accountability for interpretation/action rests with the institution, compliance/governance authority, and human reviewers assigned to the content.
- RISQON disclaims any automated decision-making authority in all disclosures.

**Lock note:** This document is final, non-marketing, and audit-oriented. Public or marketing statements about RISQON must defer to this description if inconsistencies arise.
