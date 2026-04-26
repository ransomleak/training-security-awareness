# Free Interactive Security Training Library

**100+ free hands-on SCORM exercises** covering security awareness, GDPR, AI security, and more. Built for people who want to retain what they learn and share with others.

![demo](/Assets/demo.gif)

🔗 **[Browse the full library →](https://ransomleak.com/learning)** &nbsp;|&nbsp; 🎮 **[Try a live demo →](https://ransomleak.com/exercises/phishing/)**

---

## Why this exists

Most security awareness training is forgettable: boring slide decks, soulless videos, and lately, AI-generated materials that turn people off. The problem isn't the content itself — it's the format, because passive learning doesn't build habits. People sit through a 10-minute video, click "Complete," and remember nothing when it matters.

**This library takes a different approach.**

Every exercise drops you into an interactive 3D office environment where you face realistic incidents in first-person. You interact with real objects — a phone, a PC running a live OS (browser, terminal, Zoom), a flipchart — and make decisions under pressure, just like you would at your desk.

Scenarios include things like:

- Spotting phishing indicators in a suspicious email
- Handling a scam phone call (vishing) in real time
- Downloading a malicious file and watching the consequences unfold

The goal is to build muscle memory so that when something bad is about to happen at work, people remember having faced it before — and respond accordingly. Every exercise ends with a quiz at a 100% pass threshold to confirm the knowledge is stuck.

---

## Format

Every exercise is a **SCORM .zip file** — ready to import into any LMS, embed into your existing training pipeline, or test on [SCORM Cloud](https://cloud.scorm.com/) before rollout.

The repo root contains full course packages. The `Individual Exercises` folder contains standalone exercises if you want to build a custom curriculum.

**The content is fully white-labeled** — no logos, no backlinks, no strings attached. Use it however you like, more on this below.

---

## Usage & License

You're free to use, embed, and teach with this content — personally, professionally, or commercially in workshops. Redistributing or reselling the content as a standalone product is prohibited.

[![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This library is licensed under [CC BY-NC 4.0][cc-by-nc]. Free to use and share with attribution. Commercial resale of the content is prohibited.

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg

---

## Table of Contents

### OWASP Top 10 for Agentic Applications

1. [**AI Agent Goal Hijacking**](https://ransomleak.com/exercises/agentic-goal-hijack/) — Stop an autonomous AI agent from being redirected by a poisoned email containing hidden instructions by detecting hidden instructions embedded in incoming data that redirect agent objectives, tracing how a goal-hijacked agent pivots from legitimate tasks to data exfiltration, and applying input validation strategies that prevent agents from treating data as instructions.

2. [**AI Agent Tool Exploitation**](https://ransomleak.com/exercises/agentic-tool-misuse/) — Prevent an AI agent from being manipulated into using its legitimate tools to delete files and send unauthorized messages by identifying how ambiguous prompts cause agents to misuse legitimate tool access, tracing destructive tool calls triggered by manipulated input parameters, and applying least-privilege tool access policies to contain agent tool exploitation.

3. [**Agent Identity and Privilege Abuse**](https://ransomleak.com/exercises/agentic-identity-privilege-abuse/) — Prevent an AI agent from reusing inherited high-privilege credentials to access systems beyond its authorized scope by tracing how agents inherit and propagate user credentials across different system contexts, identifying confused deputy vulnerabilities where agent privilege exceeds intended scope, and applying scoped credential delegation to prevent cross-context privilege escalation.

4. [**Agentic AI Supply Chain Attack**](https://ransomleak.com/exercises/agentic-supply-chain/) — Investigate a backdoored third-party AI plugin that silently modifies agent behavior and exfiltrates sensitive data by detecting behavioral anomalies indicating a compromised third-party AI component, tracing data exfiltration pathways through backdoored plugins and MCP servers, and applying supply chain verification practices before integrating external AI tools.

5. [**AI Agent Code Injection**](https://ransomleak.com/exercises/agentic-code-execution/) — Catch an AI coding assistant before it executes a shell script containing injected commands that compromise your system by detecting injected commands hidden within AI-generated code and shell scripts, tracing how user input flows through code generation into unsandboxed execution, and applying code review and sandboxing practices to AI-generated scripts before execution.

6. [**AI Agent Memory Poisoning**](https://ransomleak.com/exercises/agentic-memory-poisoning/) — Detect adversarial content injected into an AI agent's persistent memory that corrupts all future decisions by identifying poisoned entries in an agent's persistent memory and retrieval context, tracing how corrupted memory influences downstream agent decisions across sessions, and applying memory integrity verification to detect and remove adversarial content.

7. [**Agent-to-Agent Communication Spoofing**](https://ransomleak.com/exercises/agentic-insecure-communication/) — Intercept and identify spoofed messages between AI agents in a multi-agent workflow before fabricated instructions cause damage by detecting spoofed agent identities and fabricated messages in multi-agent communication channels, tracing how unauthenticated inter-agent messages enable man-in-the-middle attacks, and applying message authentication and agent identity verification to secure multi-agent systems.

8. [**Multi-Agent Cascading Failure**](https://ransomleak.com/exercises/agentic-cascading-failures/) — Contain a minor AI hallucination before it cascades through downstream agents into a catastrophic system-wide failure by tracing error propagation from a single agent hallucination through multiple downstream systems, identifying amplification points where small errors compound into catastrophic outcomes, and applying circuit breaker patterns and human checkpoints to interrupt cascading agent failures.

9. [**Over-Trusting AI Agent Recommendations**](https://ransomleak.com/exercises/agentic-trust-exploitation/) — Catch a series of compromised AI agent recommendations that exploit your trust to approve a fraudulent transfer and a backdoored code change by recognizing automation bias patterns where consistent AI accuracy creates false confidence, identifying subtle anomalies in AI recommendations that indicate manipulation or compromise, and applying structured verification workflows that resist social engineering through AI interfaces.

10. [**Detecting a Rogue AI Agent**](https://ransomleak.com/exercises/agentic-rogue-agent/) — Investigate a compromised AI agent that appears functional while silently performing unauthorized actions and evading monitoring by detecting covert unauthorized actions performed by an agent that appears to be operating normally, tracing persistence mechanisms that allow rogue agents to survive restarts and monitoring sweeps, and applying behavioral analysis and anomaly detection to distinguish rogue agents from legitimate ones.



### OWASP Top 10 for LLM Applications


1. [**OpenClaw Prompt Injection**](https://ransomleak.com/exercises/clawdbot-prompt-injection/) — Stop an AI assistant from leaking data via hidden prompts by identifying hidden instructions in documents, preventing data exfiltration through AI tools, and recognizing prompt injection patterns.

2. [**Sensitive Data Exposure Through AI**](https://ransomleak.com/exercises/llm-sensitive-data-disclosure/) — See what happens when confidential data enters a consumer AI tool by recognizing sensitive data categories that should never enter AI prompts, tracing how pasted content persists in AI training data and logs, and applying data classification policies before using AI tools.

3. [**AI Supply Chain Compromise**](https://ransomleak.com/exercises/llm-supply-chain-attack/) — Deploy an AI plugin that hides a backdoor in plain sight by identifying supply chain risks in third-party AI models and plugins, detecting behavioral anomalies in AI components from external sources, and applying vetting procedures before deploying marketplace AI tools.

4. [**AI Training Data Poisoning**](https://ransomleak.com/exercises/llm-data-poisoning/) — Watch poisoned documents corrupt your AI's answers in real time by tracing how manipulated documents alter AI-generated outputs, identifying signs of data poisoning in AI responses, and applying content integrity controls to knowledge base inputs.

5. [**Unsafe AI Output Handling**](https://ransomleak.com/exercises/llm-improper-output-handling/) — Exploit an AI whose outputs flow unchecked into live systems by identifying injection risks when AI outputs feed into downstream systems, tracing how unsanitized AI output enables code execution, and applying output validation controls between AI and connected systems.

6. [**Over-Permissioned AI Agent**](https://ransomleak.com/exercises/llm-excessive-agency/) — Manipulate an AI assistant into misusing its own permissions by identifying excessive permissions granted to AI agents, tracing unauthorized actions performed by manipulated AI tools, and applying least-privilege principles to AI agent configurations.

7. [**AI System Prompt Extraction**](https://ransomleak.com/exercises/llm-system-prompt-leakage/) — Extract hidden instructions from a customer-facing AI chatbot by executing prompt extraction techniques against a live AI chatbot, identifying sensitive information exposed through leaked system prompts, and applying prompt hardening techniques to prevent system instruction disclosure.

8. [**RAG Pipeline Exploitation**](https://ransomleak.com/exercises/llm-vector-embedding-attack/) — Exploit a RAG pipeline to access documents beyond your clearance by identifying access control failures in vector database retrieval, tracing how adversarial embeddings corrupt search results, and applying authorization checks at the retrieval layer of RAG systems.

9. [**AI Hallucination and Misinformation**](https://ransomleak.com/exercises/llm-ai-misinformation/) — Catch fabricated statistics and fake citations in an AI report by detecting hallucinated facts and fabricated sources in AI outputs, verifying AI-generated claims against authoritative references, and applying fact-checking workflows to AI-assisted business content.

10. [**AI Denial-of-Service Attack**](https://ransomleak.com/exercises/llm-unbounded-consumption/) — Launch a denial-of-wallet attack against an unprotected AI API by identifying resource exhaustion vectors in AI API endpoints, tracing how crafted prompts escalate compute costs exponentially, and applying rate limiting and budget controls to AI service deployments.


---

### Web & Browser Safety



1. [**HTTPS & Website Security**](https://ransomleak.com/exercises/https-and-website-security/) — Learn why the padlock icon is not proof of safety by evaluating real-world certificate warnings, expired certs, and mismatched TLS certificates across simulated websites.

2. [**Safe Browsing & Downloads**](https://ransomleak.com/exercises/safe-browsing-and-downloads/) — Spot malicious downloads before they run by navigating fake vendor sites, deceptive update prompts, and drive-by download traps that disguise malware as legitimate software.

3. [**Typosquatting Awareness**](https://ransomleak.com/exercises/typosquatting-awareness/) — Catch the domain tricks attackers use against you by identifying lookalike URLs, character-swap domains, and homograph attacks that are nearly pixel-perfect in your browser's address bar.

4. [**Browser Autofill Risks**](https://ransomleak.com/exercises/browser-autofill-risks/) — Hidden form fields silently steal your autofilled data, as demonstrated through a realistic scenario where a colleague unknowingly submits credit card and home address details to an attacker-controlled page.

5. [**Browser Extension Safety**](https://ransomleak.com/exercises/browser-extension-safety/) — That helpful extension might be stealing everything, as shown by tracing a forensic timeline of how a highly-rated productivity extension exfiltrated data from an unsuspecting user's device.

6. [**Browser Notification Abuse**](https://ransomleak.com/exercises/browser-notification-abuse/) — Recognize fake CAPTCHA prompts designed to hijack notification permissions and learn to revoke malicious push notification access before attackers escalate to credential phishing.

---

### Passwords & Account Security



1. [**Password Manager Habits**](https://ransomleak.com/exercises/password-manager-habits/) — Build strong habits with your password manager by migrating weak and reused passwords into a vault, generating unique replacements, and using autofill as a phishing detection tool.

2. [**Least Privilege Awareness**](https://ransomleak.com/exercises/least-privilege-awareness/) — Keep access to the minimum your job requires by auditing realistic permission assignments, revoking stale admin rights, and flagging shared service accounts and expired contractor credentials.

3. [**Joiner-Mover-Leaver Awareness**](https://ransomleak.com/exercises/joiner-mover-leaver-awareness/) — Manage access rights through role transitions by working through onboarding, lateral moves, and offboarding scenarios that include manager exceptions, forwarded files, and emergency access requests.

4. [**MFA Setup & Best Practices**](https://ransomleak.com/exercises/mfa-setup-best-practices/) — Set up multi-factor authentication the right way by comparing SMS, authenticator apps, and hardware keys, and learning to recognize and resist MFA fatigue push notification attacks.

5. [**Credential Stuffing Awareness**](https://ransomleak.com/exercises/credential-stuffing-awareness/) — See how breached passwords fuel automated attacks by tracing a live credential stuffing incident, identifying compromised accounts, and breaking the password reuse cycle.

6. [**Account Recovery Security**](https://ransomleak.com/exercises/account-recovery-security/) — Defend account recovery from social engineering by practicing identity verification procedures under pressure from a convincing caller impersonating a locked-out employee.

7. [**Privileged Access Basics**](https://ransomleak.com/exercises/privileged-access-basics/) — Learn why admin accounts need special handling by contrasting a just-in-time access workflow with an incident where everyday use of a privileged account gave an attacker immediate infrastructure access.

---

### Device Security



1. [**Ransomware**](https://ransomleak.com/exercises/ransomware/) — Survive a ransomware attack in real time by making rapid containment decisions as files encrypt, programs fail, and the malware spreads across shared drives and mapped network resources.

2. [**USB Drop Attack**](https://ransomleak.com/exercises/usb-drop-attack/) — Think twice before plugging in that USB drive by experiencing a simulated autorun attack, including Rubber Ducky payloads that compromise a system in under 10 seconds.

3. [**Backup Best Practices**](https://ransomleak.com/exercises/backup-best-practices/) — Build a backup plan that survives ransomware by learning the 3-2-1 rule, understanding the difference between sync and true backup, and discovering the real consequences of common backup failures.

4. [**Encryption & Lock Discipline**](https://ransomleak.com/exercises/encryption-and-lock-discipline/) — Practice the habits that protect unattended devices by seeing what an attacker can accomplish in 90 seconds on an unlocked laptop, then configuring auto-lock and verifying full disk encryption.

5. [**OS Updates & Patching Basics**](https://ransomleak.com/exercises/os-updates-and-patching-basics/) — See why skipping updates opens real attack paths by tracing what a deferred security patch was fixing and how quickly attackers weaponize newly published CVEs.

6. [**Endpoint Patching & EDR Alerts**](https://ransomleak.com/exercises/endpoint-patching-and-edr-alerts/) — Know what your EDR alert means and what to do next by triaging live process anomalies, registry changes, and unusual network connections to decide whether to ignore, investigate, or escalate.

7. [**Safe Bluetooth Practices**](https://ransomleak.com/exercises/safe-bluetooth-practices/) — Your headphones are broadcasting more than music — audit paired devices, configure non-discoverable mode, and understand the BlueBorne, KNOB, and BLUFFS vulnerability families that exploit discoverable Bluetooth connections.

8. [**File Extension Awareness**](https://ransomleak.com/exercises/file-extension-awareness/) — It looks like a PDF but runs like malware — learn to spot double-extension tricks, reveal true file types, and identify dangerous extensions like .scr, .cmd, .vbs, and .ps1.

---

### Protecting Sensitive Information



1. [**Data Leakage**](https://ransomleak.com/exercises/data-leakage/) — Stop sensitive data from leaving your organization by walking through misdirected emails, hidden document metadata, unsecured file shares, and less obvious leakage channels like AI tools and screen sharing.

2. [**Data Classification Basics**](https://ransomleak.com/exercises/data-classification-basics/) — Label data correctly by sensitivity level by sorting real-world documents into Public, Internal, Confidential, and Restricted categories and applying the correct storage, sharing, and disposal rules for each.

3. [**Identity Theft Prevention**](https://ransomleak.com/exercises/identity-theft-prevention/) — Spot identity theft tactics targeting employees by recognizing convincing HR impersonation emails, unattended personnel files, and phone callers armed with enough personal detail to sound legitimate.

4. [**Secure Sharing Practices**](https://ransomleak.com/exercises/secure-sharing-practices/) — Share files safely without creating security gaps by evaluating common sharing scenarios and learning why a password-protected expiring link differs from an unencrypted email attachment.

--- 

### Incident Reporting



1. [**General Incident Reporting**](https://ransomleak.com/exercises/general-incident-reporting/) — Know when and how to report a security incident. Recognize what qualifies as an incident, complete a security report correctly, understand reporting timelines and thresholds.

2. [**Reporting Culture**](https://ransomleak.com/exercises/reporting-culture/) — Build a team that reports without fear. Practice blameless incident reporting, understand psychological safety principles,apply the aviation CRM framework

---

### Phishing & Impersonation Attacks



1. [**Vishing**](https://ransomleak.com/exercises/vishing/) — Handle a realistic voice phishing call by detecting caller ID spoofing, practicing callback verification through official numbers, and resisting urgency and authority pressure from a convincing impersonator.

2. [**Phishing**](https://ransomleak.com/exercises/phishing/) — Spot a phishing email before you click by examining spoofed sender addresses, hovering over mismatched URLs, and identifying the emotional pressure tactics that drive credential theft.

3. [**Double Barrel Phishing**](https://ransomleak.com/exercises/double-barrel-phishing/) — Recognize the two-email trust trap by identifying the harmless setup message and the malicious follow-up that exploits the trust established in the first exchange.

4. [**Whaling With A Deepfake**](https://ransomleak.com/exercises/whaling-with-a-deepfake/) — Spot an AI-generated executive on a video call by detecting deepfake indicators during a live meeting and verifying identity before authorizing an irreversible financial transfer.

5. [**Social Engineering**](https://ransomleak.com/exercises/social-engineering/) — Recognize manipulation before you comply by holding your ground against a caller using authority, reciprocity, and artificial urgency, then redirecting verification through official channels.

6. [**Business Email Compromise**](https://ransomleak.com/exercises/business-email-compromise/) — Stop a CEO impersonation wire fraud by detecting executive impersonation emails, verifying payment requests out-of-band, and understanding why BEC causes billions in annual losses.

7. [**Smishing**](https://ransomleak.com/exercises/smishing/) — Detect fraud hiding in your text messages by slowing down on urgent delivery alerts and banking notifications, verifying through official channels, and never tapping shortened URLs.

8. [**Callback Phishing**](https://ransomleak.com/exercises/callback-phishing/) — Handle a fake invoice designed to make you call by identifying TOAD attack patterns, spotting fake invoices with callback numbers, and responding without clicking any links.

9. [**Spear Phishing**](https://ransomleak.com/exercises/spear-phishing/) — Your public LinkedIn profile is an attacker's playbook — trace how a single social media post enables a fully personalized phishing email complete with credential-harvesting collaboration portal.

10. [**QR Code Phishing (Quishing)**](https://ransomleak.com/exercises/qr-code-phishing/) — That QR code skips every email filter you have — walk through a realistic quishing attack chain and learn to preview QR code destinations before scanning on your mobile device.

11. [**Tech Support Scams**](https://ransomleak.com/exercises/tech-support-scams/) — That virus warning is the actual attack — recognize fake browser-based system alerts, refuse remote access requests from unsolicited callers, and learn why Ctrl+Alt+Delete is the correct first response.

12. [**WhatsApp Social Engineering**](https://ransomleak.com/exercises/whatsapp-social-engineering/) — Your "boss" on WhatsApp isn't your boss — experience a real-time impersonation conversation that escalates into a gift card scam and learn why messaging apps are a preferred attack channel.

13. [**SEO Poisoning Awareness**](https://ransomleak.com/exercises/seo-poisoning/) — Top search results aren't always trustworthy — detect a poisoned software download page, verify authenticity through publisher signatures and file hashes, and navigate directly to official vendor sites.

---

### GDPR Compliance



1. [**Marketing Consent Management**](https://ransomleak.com/exercises/gdpr-marketing-consent-management/) — Build compliant opt-in flows that regulators accept by designing consent flows that meet GDPR Article 7 standards, building a consent record system, and handling live withdrawal requests.

2. [**Fraudulent DSAR Detection**](https://ransomleak.com/exercises/gdpr-fraudulent-dsar-detection/) — Spot fake data access requests used for social engineering by evaluating incoming DSARs for identity inconsistencies, urgency language, and mismatched contact details before responding.

3. [**Data Breach Response**](https://ransomleak.com/exercises/gdpr-data-breach-response/) — Triage a breach and meet the 72-hour notification clock by assessing incident severity, drafting a supervisory authority notification, and making judgment calls about what qualifies as notifiable under Article 33.

4. [**Third-Party Data Processor Vetting**](https://ransomleak.com/exercises/gdpr-third-party-data-processor-vetting/) — Evaluate a vendor's data processing controls before signing by reviewing security certifications, sub-processor arrangements, breach notification procedures, and DPA clauses that fall short of Article 28.

5. [**Security Incident Response**](https://ransomleak.com/exercises/gdpr-security-incident-response/) — Coordinate security and privacy teams during a live breach by running parallel workstreams that balance containment priorities with personal data assessment and Article 33 notification deadlines.

6. [**Privacy by Design Review**](https://ransomleak.com/exercises/gdpr-privacy-by-design-review/) — Evaluate a product feature through a privacy-first lens by applying Article 25 data minimization checks and navigating real tradeoffs between functionality and privacy in behavioral tracking requests.

7. [**Legitimate DSAR Processing**](https://ransomleak.com/exercises/gdpr-legitimate-dsar-processing/) — Process a data subject access request end to end by verifying requester identity, searching across CRM, email archives, analytics, and backups, then compiling and redacting the response within 30 days.

8. [**Cross-Border Data Transfers**](https://ransomleak.com/exercises/gdpr-cross-border-data-transfers/) — Navigate transfer mechanisms for data leaving the EEA by assessing adequacy decisions, selecting Standard Contractual Clauses, and conducting a Transfer Impact Assessment following the Schrems II ruling.

9. [**PII Document Redaction**](https://ransomleak.com/exercises/gdpr-pii-document-redaction/) — Redact personal data from documents before disclosure by learning why black-box overlays and unstripped metadata can expose what you thought you removed.

10. [**Data Protection Impact Assessment**](https://ransomleak.com/exercises/gdpr-data-protection-impact-assessment/) — Run a DPIA for a high-risk data processing activity by working through Article 35 triggers, risk mapping, proportionality assessment, and producing documentation that meets statutory content requirements.

11. [**Data Mapping and Records of Processing**](https://ransomleak.com/exercises/gdpr-data-mapping-and-records-of-processing/) — Build an Article 30 processing register from scratch by conducting data flow interviews across departments and connecting fragmented data practices into a coherent, compliant RoPA.

---

### Safe Communication & Sharing



1. [**Social Media Oversharing**](https://ransomleak.com/exercises/social-media-oversharing/) — See how attackers exploit your public profiles by discovering how a vacation photo, birthday post, and conference check-in can be combined into a profile enabling highly personalized attacks.

2. [**Cloud Sharing Controls**](https://ransomleak.com/exercises/cloud-sharing-controls/) — Audit who can see your shared files right now by reviewing a tangled permissions history, tightening access to minimum required levels, and setting expiration dates under time pressure.

3. [**Guest Access Management**](https://ransomleak.com/exercises/guest-access-management/) — Control what external users can reach and for how long by auditing dormant guest accounts, revoking access from vendors whose projects have ended, and creating a structured offboarding checklist.

4. [**Secure Messaging Practices**](https://ransomleak.com/exercises/secure-messaging-practices/) — Stop sensitive data from leaking through chat apps by recognizing when passwords, customer PII, or whiteboard photos have been shared carelessly and learning the correct channels for sensitive information.

5. [**Social Media Policy**](https://ransomleak.com/exercises/social-media-policy/) — Learn what not to post on corporate accounts by evaluating real scenarios where LinkedIn posts and office photos inadvertently leaked deal details, client data, and internal system information.

6. [**Third-Party App OAuth Risks**](https://ransomleak.com/exercises/third-party-app-oauth-risks/) — Check what you gave permission to access by evaluating whether a new app's requested permissions match its actual function and auditing OAuth-connected apps for excessive or unnecessary access.

---

### Workplace Security



1. [**Insider Threat (Intentional)**](https://ransomleak.com/exercises/insider-threat-intentional/) — Recognize the warning signs of a malicious insider by spotting the pattern of after-hours file access and large USB transfers before the damage reaches a point of no return.

2. [**Shadow IT Awareness**](https://ransomleak.com/exercises/shadow-it-awareness/) — Find out what happens when teams use unapproved apps by tracing what occurred behind the scenes when a confidential spreadsheet was uploaded to a free online converter with no data agreement.

3. [**Image-Based Attacks (Stegosploit)**](https://ransomleak.com/exercises/image-based-attacks-stegosploit/) — That image file might be carrying more than pixels — investigate a contractor's portfolio that hides a JavaScript payload inside a JPEG and learn three steganographic attack methods and their detection approaches.

4. [**Insider Threat (Accidental)**](https://ransomleak.com/exercises/insider-threat-accidental/) — One wrong attachment and forty-seven salaries are exposed — experience a misdirected email incident from the DLP flag through the full incident reporting workflow.

5. [**Collaboration Tool Hygiene**](https://ransomleak.com/exercises/collaboration-tool-hygiene/) — One shortcut in Slack and credentials are everywhere — audit channel integrations and ex-employee access after discovering that pasted database credentials were exfiltrated through a stale webhook.

---

### Remote & Home Office Security



1. [**VPN Usage & Safety**](https://ransomleak.com/exercises/vpn-usage-and-safety/) — Configure and use your VPN without leaving gaps by experiencing the real consequences of a mid-session disconnect on public Wi-Fi, including exposed credentials and unencrypted file transfers.

2. [**Home Router Security**](https://ransomleak.com/exercises/home-router-security/) — Find out who else is on your home network by identifying unauthorized connected devices, changing default admin credentials, disabling WPS, enabling WPA3, and recognizing signs of DNS hijacking.

---

### Real-World Incidents



1. [**MGM Resorts Breach**](https://ransomleak.com/exercises/mgm-resorts-security-breach/) — Relive the 10-minute helpdesk call that cost $100M by tracing the Scattered Spider attack chain from LinkedIn reconnaissance through a vishing call to ALPHV/BlackCat ransomware deployment.

2. [**OneNote Email Attack**](https://ransomleak.com/exercises/onenote-email-attack/) — Trace a real BEC scam built on weeks of inbox surveillance by receiving a lookalike-domain invoice redirect that uses real project details and the exact right amount to defeat scrutiny.

---

### Security Policies & Your Role



1. [**Audit Mindset Basics**](https://ransomleak.com/exercises/audit-mindset-basics/) — Think like an auditor to find compliance gaps before external reviewers do by checking whether password policies match real behavior, verifying access reviews, and identifying gaps between written procedures and daily operations.

2. [**Audit Portal Training**](https://ransomleak.com/exercises/audit-portal-training/) — Navigate GRC portals and submit audit evidence. Upload and tag compliance evidence correctly, track remediation tasks to closure, avoid common portal submission errors

3. [**Employee Security Responsibilities**](https://ransomleak.com/exercises/employee-security-responsibilities/) — Know your personal security duties at work. Recognize tailgating and credential sharing risks, report incidents through the right channels, protect physical and digital access points

4. [**ISMS Policy Awareness**](https://ransomleak.com/exercises/isms-policy-awareness/) — Connect ISO 27001 policies to your daily work. Match ISMS policies to real work situations, understand the ISO 27001 policy structure, spot gaps between policy and daily practice.

5. [**Internet & Email Acceptable Use**](https://ransomleak.com/exercises/internet-email-acceptable-use/) — Stay within corporate internet and email policies. Recognize risky email forwarding behaviors, understand personal device boundaries at work, avoid common acceptable use violations
