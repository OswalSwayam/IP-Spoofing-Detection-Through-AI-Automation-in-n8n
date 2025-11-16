# 🤖IP-Spoofing-Detection-Through-AI-Automation-in-n8n

# 🧠n8n  Workflow
Email spoofing investigation, Security monitoring for incoming mail, SOC/investigation automation, Automated IP intelligence enrichment, Logging and reporting for suspicious email activity, SPF, DKIM, and DMARC validation and classification, Automatic logging to Google Sheets for history, audits, and analysis.

# 🚀Setup Instructions
1. Import Workflow:
Download the JSON file from this repository.
In n8n, go to Menu → Import Workflow
Upload the JSON!..

2. 🧩Configure Credentials:
You will need: Gmail (OAuth2 credentials for read-only header access)
& also needed IP_API (IPQualityScore: API key for IP reputation queries)

3. 📡Enable the Workflow.

4. 🔄Turn on the workflow.
   
5. 🗂️Incoming emails will now be scanned and appended to your sheet.

6.Output Format (Each processed email produces structured data):
a.initialIP
b.spf
c.dkim
d.dmarc
e.organization
f.country
g.city
h.recentSpamActivity
i.ipSenderReputation
j.These values help you visually identify suspicious senders or spoofing attempts.

# 📈Workflow Summary
A.Gmail Trigger receives an email.
B.Headers are cleaned, extracted, and parsed.
C.Originating IP is isolated.
D.SPF/DKIM/DMARC values are determined.
E.IP reputation & geo data are fetched.
F.Data is formatted into a single structured output.
G.Entry is automatically saved to Google Sheets.
H.Optional AI agent processes or explains results.

# 🔧Future Enhancements
1. Automated alerts (Slack, Telegram, Discord, Email).
2. Auto-blocking IPs with high fraud score.
3. Integration with Firewalls / SIEM tools.
4. Visualization dashboards.
5. Attachment malware scanning.
