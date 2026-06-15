# FUTURE_CS_02

Phishing Email Analysis

**Internship:** Future Interns Cyber Security Internship 2026 — Task 2  
**Prepared by:** Shivakumar S  
# Tools Used

Google Admin Toolbox Message Header Analyser — SPF, DKIM, DMARC results, routing, and delivery timing for all 10 samples
Cisco Talos Intelligence — Sending IP reputation and network owner lookup for real received samples (E-01, E-02, E-03)
Gmail "Show Original" — Raw header extraction for real received emails
Public GitHub phishing datasets — Source for samples E-04 through E-10

# Analysis Approach

Header extraction — Raw headers pasted into Google Admin Toolbox; SPF, DKIM, DMARC results recorded
Sender domain check — Display name compared against actual sending domain in angle brackets
Body review — Urgency language, reward lures, and greeting personalisation assessed
Link inspection — Destination URLs examined via raw HTML source without activation
IP reputation lookup — Sending IPs verified on Cisco Talos for real-world samples
Classification — Each email scored against a four-indicator framework; 2+ confirmed = Phishing, 1 = Suspicious, 0 = Safe

Methodology
Fully passive and read-only. No links clicked, no attachments opened, no credentials entered, no phishing infrastructure interacted with at any point.
Repository Structure

images/ — Screenshots used as evidence during analysis

samples/ — The 10 email samples analysed
