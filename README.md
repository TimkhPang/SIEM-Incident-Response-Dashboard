# SIEM Incident Response Dashboard

This project demonstrates log ingestion, detection, and alerting using Splunk to identify unusual events (e.g. brute force, privilege escalation) from Windows and Apache logs. It builds dashboards, refines detection rules, and reduces false positives—all aligning with real SOC workflows.

---

## 🛠 Tools & Technologies Used

| Tool / System           | Purpose / Security Functionality                                            |
|--------------------------|------------------------------------------------------------------------------|
| Splunk                   | Centralized log collection, correlation, and dashboarding                  |
| Windows Event Logs       | Data source for authentication events, privilege escalation monitoring      |
| Apache Server Logs       | Web server traffic, baseline monitoring, anomaly detection                 |
| Custom Splunk Rules      | Detect failed logins, privilege escalation, brute-force attempts           |
| MITRE ATT&CK Framework    | Mapping detections to technique IDs for structured incident reporting     |
| Log Baseline Analysis     | Establish normal behavior to distinguish anomalies                       |

---

## 🎯 Objectives & Key Outcomes

| Objective                                       | Execution Details                                               | Result / Impact                                              |
|--------------------------------------------------|------------------------------------------------------------------|---------------------------------------------------------------|
| Detect brute-force attacks                       | Created custom rule in Splunk for repeated failed login attempts | Successfully detected simulation with **95% accuracy**         |
| Identify privilege escalation                    | Monitored Windows logs for misuse of elevated permissions       | Flagged escalation events; reduced false positives by **30%**  |
| Establish log baselines                          | Defined normal patterns for Apache and Windows login activity   | Dashboard alerts triggered only when behavior exceeded baseline |
| Improve Alert Tuning                             | Refined correlation logic and rule thresholds                   | Fewer false positives; more meaningful alerts for security team |
