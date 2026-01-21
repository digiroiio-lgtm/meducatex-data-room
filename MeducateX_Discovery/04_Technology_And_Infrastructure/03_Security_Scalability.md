# 03 Security & Scalability Posture

**Purpose:** Outline the security, compliance, and scalability commitments along with clear limitations.

**Last updated:** 2026-01-21

The platform is hosted on a HIPAA-compliant cloud environment with encryption at rest/in transit, role-based access control, audit logging, and multi-factor authentication for administrative access. Scalability is achieved via autoscaling containers and partitioned storage so that each institution retains logical isolation. Monitoring includes uptime alerts, usage dashboards, and periodic tabletop drills.

**Limitations:** No public model weights or training data are distributed; the architecture is tuned for decision-support, not real-time diagnostics. We explicitly document these limitations so VC reviewers understand what MeducateX does not promise.
