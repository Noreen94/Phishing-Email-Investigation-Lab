# Phishing Email Investigation Report

## 1. Incident Overview

**Incident type:** Suspected phishing email  
**Target organisation:** FinTrust Solutions (fictional)  
**Date received:** 5 November 2026  
**Reported time:** 09:42 AM  
**Severity:** Medium – preliminary assessment  
**Investigation status:** Initial analysis completed

## 2. Email Details

- **Sender:** security-alert@micr0soft-account.example
- **Recipient:** employee@fintrust.example
- **Subject:** URGENT: Your Microsoft 365 Account Will Be Suspended
- **Suspicious URL:** hxxps://micr0soft-security.example/verify

## 3. Indicators of Phishing

The following suspicious characteristics were identified:

1. **Impersonation:** The sender uses `micr0soft` with a zero instead of the letter O.
2. **Generic greeting:** The email addresses the recipient as "Dear User".
3. **Urgency:** The subject line creates pressure to act immediately.
4. **Threatening language:** The message threatens account suspension within 24 hours.
5. **Credential harvesting risk:** The recipient is asked to verify account details through a link.
6. **Suspicious domain:** The verification link uses an unfamiliar domain rather than an established Microsoft domain.

## 4. Indicators of Compromise (IOCs)

| Indicator | Observed value |
|---|---|
| Sender address | security-alert@micr0soft-account.example |
| Suspicious domain | micr0soft-security.example |
| URL path | /verify |
| Subject | URGENT: Your Microsoft 365 Account Will Be Suspended |

These are indicators extracted from the simulated email. Their malicious reputation has not been independently verified.

## 5. Risk Assessment

The email presents a potential credential theft risk. If an employee followed the link and entered their login details, an attacker could potentially gain unauthorised access to the account.

The urgency and impersonation techniques increase the likelihood of a recipient being persuaded to act.

## 6. Recommended SOC Response

- Do not click the suspicious link or reply to the email.
- Report and escalate the email to the security team.
- Check whether other employees received the same message.
- Review available email security and identity logs.
- Check for suspicious sign-ins or unusual account activity.
- If credential compromise is confirmed, follow the organisation's account containment and password reset procedures.
- Consider blocking the sender and domain through approved security controls.

## 7. Investigation Limitations

This investigation is based on a fictional email sample. No live URL was visited, and no real email headers, attachments, or authentication logs were available.

The sender's identity, domain reputation, and whether credentials were compromised cannot be confirmed from the supplied email content alone.

## 8. Conclusion

The simulated email contains multiple characteristics consistent with a phishing attempt, including brand impersonation, urgency, threatening language, and a suspicious verification link.

The appropriate SOC response is to treat the email as suspicious, preserve the evidence, and escalate for further investigation.

**Final assessment:** Suspected phishing – further verification required.

## 9. Email Authentication Analysis

The simulated email headers showed the following authentication results:

- SPF: FAIL
- DKIM: NONE
- DMARC: FAIL

These results indicate that the email failed SPF and DMARC authentication checks and had no DKIM signature.

Combined with the suspicious sender address, urgency, brand impersonation and unfamiliar verification link, these findings increase the likelihood that the message is a phishing attempt.

Note: These are simulated header results created for this lab, not results obtained from a live email investigation.
