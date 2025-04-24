# Types of Risks in Information Security

## 1. Operational Risk
Risk arising from failed internal processes, people, or systems (e.g., human error, system failure).
- **Example**: Backup failure, misconfigured firewall.

## 2. Compliance Risk
Risk of non-compliance with laws, regulations, or internal policies.
- **Example**: Failing a SOX 404 or ISO 27001 audit due to inadequate documentation.

## 3. Strategic Risk
Risk that affects an organization’s long-term goals or strategy.
- **Example**: Adopting a vendor with poor security posture impacting your reputation.

## 4. Reputational Risk
Risk of negative public opinion or stakeholder trust.
- **Example**: A data breach making headlines due to a third-party vulnerability.

## 5. Cybersecurity Risk (or IT Risk)
Risk of unauthorized access, attacks, or data breaches.
- **Example**: Ransomware attacks, phishing incidents, DDoS attacks.

## 6. Third-Party/Vendor Risk
Risk associated with external vendors or service providers.
- **Example**: Vendor does not meet required security controls or has weak access management.

## 7. Financial Risk
Direct or indirect financial losses due to a security event.
- **Example**: Fines due to GDPR non-compliance, or cost of incident response.

## 8. Privacy Risk
Risk associated with exposure or misuse of personally identifiable information (PII).
- **Example**: Improper handling of customer data, violating data retention laws.

## 9. Technology Risk
Risk related to outdated or unpatched systems and software.
- **Example**: Unsupported operating systems with known vulnerabilities.

## 10. Physical Security Risk
Risk related to unauthorized physical access or environmental hazards.
- **Example**: Lack of CCTV, access badge misuse, or server room overheating.

- # Quantitative vs Qualitative Risk Models

| Feature | Qualitative Risk Model | Quantitative Risk Model |
|--------|-----------------------------|------------------------------|
| 🔍 **Definition** | Assesses risk using descriptive categories (e.g., High, Medium, Low) | Assesses risk using numerical values (e.g., monetary loss, probabilities) |
| 📏 **Measurement** | Subjective, based on expert judgment | Objective, based on data and calculations |
| 🛠️ **Tools** | Risk matrices, heat maps, interviews | Monte Carlo simulations, ALE, probability distributions |
| 📈 **Output** | Risk rankings or priority lists | Exact financial impact and probability values |
| 🧠 **Used When** | Data is scarce or for initial risk assessments | Data is available and precise risk measurement is needed |
| 💼 **Common In** | Small/medium businesses, early ISMS phases | Financial services, insurance, high-risk industries |

---

## 🔹 Qualitative Risk Model – Example

You identify a threat of phishing to your organization.

- **Likelihood** = High  
- **Impact** = Medium  
- **Risk Level** = High (based on matrix)

✅ Easy to understand, fast to implement  
❌ Subjective, inconsistent between people

---

## 🔸 Quantitative Risk Model – Example

You estimate:

- **Annual Rate of Occurrence (ARO)** = 0.5  
- **Single Loss Expectancy (SLE)** = $50,000  
- **Annual Loss Expectancy (ALE)** = ARO × SLE = **$25,000**

✅ Precise and data-driven  
❌ Time-consuming, needs reliable historical data

---

## 📚 When to Use What?

| Situation | Use Model |
|----------|------------|
| You're starting ISMS and lack detailed data | Qualitative |
| You need executive buy-in and a quick heat map | Qualitative |
| You're justifying cybersecurity investment | Quantitative |
| You're managing regulatory or financial risk | Quantitative |

