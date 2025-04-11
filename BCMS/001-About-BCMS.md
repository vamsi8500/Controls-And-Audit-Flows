# Business Continuity and Management System (BCMS) Overview

## 1. What is BCMS?
A **Business Continuity and Management System (BCMS)** ensures that an organization can continue operating in case of disruptions such as cyberattacks, natural disasters, or technical failures. It includes policies, procedures, and recovery strategies to minimize downtime and data loss.

BCMS covers two major aspects:
- **Business Continuity (BC):** How a business will continue operating during a disaster.
- **Disaster Recovery (DR):** How a business will recover lost data and restore operations after a disaster.

## 2. Key Components of BCMS
### A. Business Continuity in Case of Disaster
- Ensures operations can continue despite disruptions.
- Involves backup plans, alternative locations, and redundant systems.
- Managed by applications, cloud infrastructure, and network teams.

### B. Disaster Recovery in Case of Data Loss
- Focuses on restoring lost data and bringing systems back online.
- Requires backup solutions, replication strategies, and failover mechanisms.

## 3. Key BCMS Metrics
To measure and ensure an effective Business Continuity Plan (BCP) and Disaster Recovery Plan (DRP), several key metrics are used:

| **Metric** | **Definition** | **Purpose** |
|------------|--------------|--------------|
| **Recovery Point Objective (RPO)** | Maximum acceptable data loss, measured in time. | Defines how much data can be lost before it impacts the business. |
| **Recovery Time Objective (RTO)** | Maximum acceptable time to restore critical systems. | Determines how quickly systems must be back online. |
| **Work Recovery Time (WRT)** | Time required to verify data integrity after restoration. | Ensures data correctness before business resumes. |
| **Maximum Tolerable Downtime (MTD)** | Maximum time an organization can survive without critical systems. | Includes RTO + WRT, ensuring continuity limits are met. |

## 4. Example Calculation
Let's say a company defines the following:

- **RPO:** 30 minutes (Maximum 30 minutes of data loss is acceptable)
- **RTO:** 1 hour (Systems must be restored within 1 hour)
- **WRT:** 1 hour (Data integrity must be tested within 1 hour)
- **MTD = RTO + WRT**

### MTD Calculation:
```
MTD = RTO + WRT = 1hr + 1hr = 2hrs
```

If a cloud security service like **CrowdStrike** is used:
- **RPO = 30 min**
- **RTO = 30 min**
- **WRT = 1 hr**
- **MTD = 2 hrs**

Each service must ensure that its recovery metrics **do not breach the agreed Service Level Agreements (SLAs).**

## 5. Service Level Agreements (SLA) and BCMS
An **SLA** defines the level of service and guarantees provided by a vendor. If RTO, RPO, or WRT is breached, the SLA is violated.

### Example SLA values:

| **Metric** | **SLA Commitment** |
|------------|------------------|
| **RPO** | 12 hours |
| **RTO** | 12 hours |
| **WRT** | 6 hours |

# RTO (Recovery Time Objective) and RPO (Recovery Point Objective)

**RTO** and **RPO** are two key concepts in disaster recovery and business continuity planning. Let’s break them down with simple definitions and examples:

---

## 1. RTO – Recovery Time Objective

**Definition:**  
The maximum acceptable amount of time it should take to restore a system or application after a failure or disaster.

**Example:**  
Let’s say your e-commerce site goes down due to a server crash. If your **RTO is 2 hours**, it means your IT team should bring the system back online within 2 hours to avoid serious business impact.

---

## 2. RPO – Recovery Point Objective

**Definition:**  
The maximum acceptable amount of data loss measured in time. It defines the point in time to which data must be restored.

**Example:**  
If your **RPO is 15 minutes**, and the system crashes at 2:00 PM, then you should be able to recover data up to 1:45 PM. This means you can afford to lose only 15 minutes worth of data.

---

## Combined Example

Imagine you’re running an online banking system:

- **RTO = 4 hours** → You must bring the system back up within 4 hours.
- **RPO = 10 minutes** → You can afford to lose at most 10 minutes of data (e.g., transactions, logs).

### So, your disaster recovery plan should ensure that:
- Backups are taken every 10 minutes.
- Systems are capable of being restored and operational in less than 4 hours.


If breached, an investigation is required with **evidence** such as:
- Policies & procedures documentation
- Business Risk Analysis (BRA) and DR plans
- Plan approvals by Cybersecurity Director or CEO
- Mock drill test results
- SLA monitoring reports

## 6. Testing and Compliance
Organizations conduct **mock disaster recovery drills** to verify their BCMS is effective. These tests ensure that:
- **Production environments can failover to disaster recovery (DR) sites.**
- **Key metrics like RTO and RPO are met.**
- **Data recovery works correctly.**

### Testing methods:
#### 1. Random Data Integrity Check:
- Select a random database table.
- Compare row count in DR and production.

#### 2. Mock Disaster Drills:
- Shutdown production servers.
- Verify DR site takes over with all data intact.

## 7. Failure Handling and Evidence Collection
If SLA, RPO, or RTO values are breached, a post-mortem review is conducted. Required evidence includes:
- **Test reports (RTO, RPO, WRT, MTD).**
- **Approval logs from senior management.**
- **Mock drill schedules and results.**
- **Compliance audit records.**

If a critical failure is detected, teams must:
- Escalate the issue to cybersecurity and cloud teams.
- Update BCMS plans and improve disaster recovery mechanisms.

## 8. Conclusion
A **strong BCMS ensures business continuity and quick disaster recovery** by setting recovery objectives, testing regularly, and maintaining compliance. Organizations must regularly assess their **RPO, RTO, WRT, and MTD values** to avoid SLA breaches and minimize operational risks.
