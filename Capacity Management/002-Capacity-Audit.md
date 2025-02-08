# Capacity Management – Control Domain (Detailed Explanation)

## Step 1: Identify the Control Owner via Kickoff Meetings
The first step in capacity management control is to identify the **Control Owner (CO)** responsible for overseeing the process. This is done through **Kickoff Meetings**, where key stakeholders are identified and assigned specific responsibilities.

### Purpose of Identifying the Control Owner:
- Ensures **accountability** for monitoring and managing IT resources.
- Helps in **governance and compliance** by assigning ownership.
- Facilitates **audit readiness** by ensuring proper documentation.

---

## Step 2: Inquiry – Understanding the Governance Control Process
This step involves gathering information about how capacity management is governed and controlled. The process includes conducting inquiries with the **Control Owner (CO)** and reviewing the organization's **capacity management procedures**.

### Key Inquiry Questions & Activities:

### 1. Identify the Control Owner (CO) & Capacity Management Procedures
- Gather information about the **Control Owner's Name, Designation, and Timestamp of Inquiry**.
- Review **Capacity Management Procedures** to understand:
  - How capacity is monitored and managed.
  - Whether **documented policies and procedures** exist.

### 2. Identify Capacity Monitoring Tools
- Determine if any **capacity monitoring tools** are in use. Common tools include:
  - **Nagios**
  - **Zabbix**
  - **Other monitoring solutions**
- Verify that all **Production, Live, and Non-Production Servers** are **actively monitored**.
- Cross-check monitored servers with the **Asset Register** to confirm all assets are included.

### 3. Check Alert Mechanisms & Notification Process
- Verify whether the **monitoring tool is generating alerts** when capacity thresholds are breached.
- Ensure that **alerts are communicated to the respective monitoring team** via email or ticketing system.
- Confirm whether **threshold levels are defined in the capacity management procedure**.

### 4. Define Thresholds & Alert Prioritization
- Confirm that **threshold values are properly assigned** based on severity levels.

| **Threshold Level** | **Priority Level** | **Example (Disk Usage)** | **Alert Status** |
|--------------------|------------------|-------------------------|----------------|
| **Below 60% Usage** | Normal | Disk Usage < 60% | OK |
| **65% - 75% Usage** | Low Priority (**P3**) | Disk Usage between 65%-75% | Warning |
| **75% - 85% Usage** | Medium Priority (**P2**) | Disk Usage between 75%-85% | High Alert |
| **85% - 95% Usage** | High Priority (**P1**) | Disk Usage between 85%-95% | Critical Alert |

- **Verify whether alerts are being prioritized based on impact.**
- Ensure **SLA (Service Level Agreements) are defined** for handling alerts.

---

## Step 3: Walkthrough – Testing, Audit, and Evidence Collection
The third step is to conduct a **walkthrough audit** to test, sample, and gather evidence to ensure that the capacity management process is working effectively.

### Key Walkthrough Activities:

### 1. Walkthrough with the Control Owner (CO)
- Conduct a **walkthrough session with the Control Owner** and document:
  - **Control Owner's Name, Designation, and Timestamp of Walkthrough**.
- Request the **Control Owner to show the monitoring dashboard** and verify:
  - Are all assets updated and listed in the system?
  - Are monitoring tools capturing capacity usage accurately?
  - Are alerts being generated in real time?

### 2. Audit Period Review (Feb 2022 – Feb 2023)
- Check whether **alerts were triggered during the audit period**.
- Verify whether **alerts were sent to the respective monitoring team via email**.
- Confirm whether alerts were **properly forwarded to the Distribution List (DL)**.

### 3. Analyze Total Alerts Generated & Their Closure Status
- During the audit period, a total of **654 alerts** were generated.
- Before proceeding with sampling, check if **all alerts have been closed** within their SLA.

### 4. Sample Alerts for Detailed Verification
- Select **a sample of 25 alerts** and verify the following:
  - Were the alerts **notified to the correct DL**?
  - What **priority level** was assigned (P1, P2, P3)?
  - Was the issue **resolved within the defined SLA**?

| **Alert Sample** | **Alert Type** | **Sent to DL? (Yes/No)** | **Priority (P1/P2/P3)** | **Resolved within SLA? (Yes/No)** |
|---------------|------------|-----------------|----------------|----------------|
| Alert #1 | CPU Utilization 85% | Yes | P1 | Yes |
| Alert #2 | Disk Utilization 70% | Yes | P3 | Yes |
| Alert #3 | Network Latency High | Yes | P2 | No |
| Alert #4 | Server Memory 90% | Yes | P1 | Yes |
| Alert #5 | Application Load High | Yes | P2 | Yes |

### 5. Collect Audit Evidence
- Verify whether **screen captures of the monitoring dashboard** are available as evidence.
- Confirm whether **alerts were properly categorized and handled**.
- Ensure there are records showing **alerts were escalated and resolved** within SLA.

---

## Final Checklist for Capacity Management Audit

| **Audit Task** | **Status (Completed/Not Completed)** | **Remarks** |
|--------------|------------------|----------|
| Control Owner Identified | ✅ Completed | Name & Designation Recorded |
| Monitoring Tools Identified | ✅ Completed | Nagios/Zabbix Confirmed |
| Capacity Procedure Documented | ✅ Completed | Available for Review |
| Asset Register Cross-Checked | ✅ Completed | All Monitored Servers Verified |
| Alert Notification Process Verified | ✅ Completed | Alerts Sent to Monitoring Team |
| Threshold Values Defined | ✅ Completed | P1, P2, P3 Levels Assigned |
| SLA for Capacity Issues Verified | ✅ Completed | Defined & Implemented |
| Total Alerts Reviewed (654) | ✅ Completed | Logs Verified |
| Sample Alerts Checked (25) | ✅ Completed | 25 Cases Analyzed |
| Dashboard Screenshots Collected | ✅ Completed | Audit Evidence Preserved |

---

## Summary & Final Recommendations
- **All production/live servers should be continuously monitored.**
- **Monitoring tools must generate alerts based on defined threshold levels.**
- **Alerts must be sent to the respective teams via email or ticketing systems.**
- **The team should ensure that alerts are resolved within SLA.**
- **Audit evidence should include screen captures of monitoring dashboards and alert logs.**

By following these best practices, the organization can ensure **efficient capacity management, proactive issue detection, and compliance with governance controls.** 🚀
