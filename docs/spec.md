# NIST SP 800-115 — Information Security Testing — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates it in
CI. The prose headings are hand-owned — everything between `tl:*` markers is injected from
the YAML items, so the published spec can never drift from the graph.

This source expresses **NIST SP 800-115, "Technical Guide to Information Security Testing and
Assessment"**: each technique category and process phase is a `user_requirement`, and each
technique or activity is a `system_requirement` that `implements` it. The SP 800-115 section
lives in `attrs.source_ref` (e.g. `NIST SP 800-115 §5.2`). The throughline UIDs are this
source's own and immutable — a consumer cites an item as `nist800115:SR-0012`, never by a
section number.

NIST SP 800-115 is a U.S. government publication in the public domain; see `NOTICE`.

Contains
<!-- tl:count type == 'user_requirement' -->
6
<!-- tl:end --> categories/phases and
<!-- tl:count type == 'system_requirement' -->
25
<!-- tl:end --> techniques/activities.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — Information security can be assessed with repeatable technical methods** — `intent`, status `proposed`

> NIST SP 800-115 exists so that an organisation can plan and perform technical information security testing and assessment in a repeatable, methodical way — using recognised review, identification and validation techniques within a disciplined planning, execution and post-testing process — rather than ad-hoc security checks.

**source_ref**: NIST SP 800-115
<!-- tl:end -->

## 3. Review techniques

<!-- tl:item UR-0001 -->
**UR-0001 — Review techniques** — `user_requirement`, status `proposed`

> Passive, examination-based techniques that assess systems, applications, networks, policies and procedures without actively exercising the target.

*Derives from:* INT-0001

**source_ref**: NIST SP 800-115 §3
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref').startswith('NIST SP 800-115 §3') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | proposed | Documentation review |
| SR-0002 | system_requirement | proposed | Log review |
| SR-0003 | system_requirement | proposed | Ruleset review |
| SR-0004 | system_requirement | proposed | System configuration review |
| SR-0005 | system_requirement | proposed | Network sniffing |
| SR-0006 | system_requirement | proposed | File integrity checking |
<!-- tl:end -->

## 4. Target identification and analysis techniques

<!-- tl:item UR-0002 -->
**UR-0002 — Target identification and analysis techniques** — `user_requirement`, status `proposed`

> Techniques that identify systems, ports, services and potential vulnerabilities, generally active but not intended to exploit them.

*Derives from:* INT-0001

**source_ref**: NIST SP 800-115 §4
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref').startswith('NIST SP 800-115 §4') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0007 | system_requirement | proposed | Network discovery |
| SR-0008 | system_requirement | proposed | Network port and service identification |
| SR-0009 | system_requirement | proposed | Vulnerability scanning |
| SR-0010 | system_requirement | proposed | Wireless scanning |
<!-- tl:end -->

## 5. Target vulnerability validation techniques

<!-- tl:item UR-0003 -->
**UR-0003 — Target vulnerability validation techniques** — `user_requirement`, status `proposed`

> Techniques that actively confirm the existence of vulnerabilities by attempting to exploit them, corroborating findings from earlier phases.

*Derives from:* INT-0001

**source_ref**: NIST SP 800-115 §5
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref').startswith('NIST SP 800-115 §5') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0011 | system_requirement | proposed | Password cracking |
| SR-0012 | system_requirement | proposed | Penetration testing |
| SR-0013 | system_requirement | proposed | Social engineering |
<!-- tl:end -->

## 6. Security assessment planning

<!-- tl:item UR-0004 -->
**UR-0004 — Security assessment planning** — `user_requirement`, status `proposed`

> Establishing the policy, priorities, approach, rules of engagement and legal basis for an assessment before any testing begins.

*Derives from:* INT-0001

**source_ref**: NIST SP 800-115 §6
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref').startswith('NIST SP 800-115 §6') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0014 | system_requirement | proposed | Establish an information security assessment policy |
| SR-0015 | system_requirement | proposed | Prioritize and schedule assessments by risk |
| SR-0016 | system_requirement | proposed | Select the assessment approach and objectives |
| SR-0017 | system_requirement | proposed | Establish rules of engagement |
| SR-0018 | system_requirement | proposed | Address legal considerations and authorization |
<!-- tl:end -->

## 7. Security assessment execution

<!-- tl:item UR-0005 -->
**UR-0005 — Security assessment execution** — `user_requirement`, status `proposed`

> Coordinating and carrying out the assessment, analysing results to identify vulnerabilities, and handling assessment data securely.

*Derives from:* INT-0001

**source_ref**: NIST SP 800-115 §7
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref').startswith('NIST SP 800-115 §7') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0019 | system_requirement | proposed | Coordinate the assessment with stakeholders |
| SR-0020 | system_requirement | proposed | Execute the selected assessment techniques |
| SR-0021 | system_requirement | proposed | Analyze results to identify vulnerabilities |
| SR-0022 | system_requirement | proposed | Handle assessment data securely |
<!-- tl:end -->

## 8. Post-testing activities

<!-- tl:item UR-0006 -->
**UR-0006 — Post-testing activities** — `user_requirement`, status `proposed`

> Turning findings into action: root-cause analysis, reporting, and mitigation of the identified weaknesses.

*Derives from:* INT-0001

**source_ref**: NIST SP 800-115 §8
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref').startswith('NIST SP 800-115 §8') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0023 | system_requirement | proposed | Conduct root-cause analysis of findings |
| SR-0024 | system_requirement | proposed | Report findings with risk-based recommendations |
| SR-0025 | system_requirement | proposed | Remediate and track mitigation |
<!-- tl:end -->
