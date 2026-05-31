# Incident Detection and Verification

## Key Concepts

* **Detection** is the prompt identification of security events and suspicious activities.
* **Analysis** involves investigating and validating alerts to determine if a real incident exists.
* Detection is performed using tools such as:

  * Intrusion Detection Systems (IDS)
  * Security Information and Event Management (SIEM) platforms
  * Threat intelligence platforms
  * Threat hunting techniques
* **Indicators of Compromise (IoCs)** are pieces of evidence suggesting a security incident may have occurred.
* **Indicators of Attack (IoAs)** represent attacker behaviors that indicate an attack is actively occurring.
* **Threat Hunting** is the proactive search for hidden threats that evade automated detection tools.
* **Threat Intelligence** provides context about existing and emerging threats using information from various sources.
* The **Pyramid of Pain** ranks IoCs based on how difficult it is for attackers to change them:

  1. Hash Values
  2. IP Addresses
  3. Domain Names
  4. Network Artifacts
  5. Host Artifacts
  6. Tools
  7. Tactics, Techniques, and Procedures (TTPs)

## Alert Triage Process

1. **Receive and Assess**

   * Validate the alert.
   * Identify false positives.
   * Determine severity and scope.

2. **Assign Priority**

   * Evaluate functional impact.
   * Assess information impact.
   * Consider recoverability.

3. **Collect and Analyze**

   * Gather evidence.
   * Research related threats.
   * Document findings.
   * Escalate if necessary.

---

# Create and Use Documentation

## Importance of Documentation

Documentation supports:

* Investigations
* Incident response activities
* Communication
* Compliance requirements
* Knowledge transfer

## Benefits of Documentation

### Transparency

* Creates accountability.
* Supports audits and legal processes.
* Maintains evidence tracking through chain of custody.

### Standardization

* Ensures consistent incident handling.
* Supports repeatable processes.
* Facilitates onboarding and training.

### Clarity

* Provides understandable information.
* Explains decisions and actions taken.
* Improves communication among teams.

## Common Security Documentation

* Incident Response Plans
* Playbooks
* Business Continuity Plans (BCP)
* Chain of Custody Records
* Investigation Notes
* Lessons Learned Reports
* Final Incident Reports

## Documentation Best Practices

* Know your audience.
* Keep information concise and relevant.
* Review and update documents regularly.
* Maintain accuracy and consistency.
* Document actions as they occur.

---

# Response and Recovery

## Containment

* Limits the spread and impact of an incident.
* Prevents additional damage.
* Examples:

  * Isolating infected systems
  * Blocking malicious IP addresses
  * Disabling compromised accounts

## Eradication

* Removes all traces of the threat.
* Eliminates malware and attacker access.
* Addresses root causes and vulnerabilities.

## Recovery

* Restores systems and services to normal operation.
* Verifies systems are functioning correctly.
* Continues monitoring for signs of reinfection.

## Business Continuity Planning (BCP)

* Ensures critical business operations continue during disruptions.
* Defines recovery procedures and responsibilities.
* Minimizes operational downtime.

## Site Resilience Recovery Options

### Hot Site

* Fully operational duplicate environment.
* Immediate failover capability.

### Warm Site

* Partially prepared backup environment.
* Requires minimal setup before use.

### Cold Site

* Basic infrastructure only.
* Requires significant setup before operation.

## Recovery Goals

* Restore business operations.
* Protect critical assets.
* Minimize downtime.
* Reduce financial and reputational impact.

---

# Post-Incident Actions

## Post-Incident Activity

* Final phase of the incident response lifecycle.
* Reviews the incident and response efforts.
* Identifies opportunities for improvement.

## Lessons Learned Meeting (Post-Mortem)

### Purpose

* Evaluate incident handling.
* Identify strengths and weaknesses.
* Improve future response processes.

### Common Discussion Questions

* What happened?
* When did it occur?
* How was it detected?
* How was it contained?
* What recovery actions were taken?
* What improvements are needed?

### Meeting Roles

* Moderator: Leads discussions.
* Scribe: Records notes and action items.

## Recommendations

* Update incident response playbooks.
* Improve detection capabilities.
* Enhance security controls.
* Refine communication procedures.
* Implement new security technologies.

## Final Report Components

### Executive Summary

* High-level overview of the incident.
* Key findings and impact.

### Timeline

* Chronological sequence of events.

### Investigation Details

* Analysis performed.
* Evidence collected.
* Findings and conclusions.

### Recommendations

* Actions to prevent similar incidents.

## Key Objectives of Post-Incident Activities

* Learn from incidents.
* Improve response processes.
* Strengthen organizational security posture.
* Reduce future risk.
