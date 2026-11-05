# Credential Compromise Response – SOC Level 1

## 1. Incident Scenario

A fictional employee reports that they clicked a suspicious link in a phishing email and entered their Microsoft 365 password.

**Incident type:** Suspected credential compromise  
**Affected account:** employee@fintrust.example  
**Severity:** High – preliminary assessment  
**Status:** Requires immediate investigation and escalation

## 2. Initial Assessment

The employee may have disclosed their login credentials to an unauthorised third party.

This creates a risk of account takeover, unauthorised access to company information and further phishing activity.

Credential compromise has not yet been independently confirmed.

## 3. Immediate SOC Response

As a SOC Level 1 Analyst:

1. Record the employee's report and preserve the original phishing email.
2. Escalate the incident immediately to the appropriate security team.
3. Follow the organisation's approved account containment procedure.
4. Request an authorised password reset.
5. Arrange revocation of active sessions where appropriate.
6. Confirm that MFA is enabled and investigate any suspicious MFA activity.

## 4. Investigation Activities

Review available Microsoft 365 and identity logs for:

- Unusual sign-in locations or IP addresses.
- Repeated failed or successful login attempts.
- Sign-ins from unfamiliar devices.
- Unexpected MFA requests or changes.
- Unauthorised inbox forwarding rules.
- Suspicious email activity.
- Unfamiliar application permissions or OAuth grants.

## 5. Recommended Actions

- Secure the affected account.
- Investigate whether other accounts were targeted.
- Review potentially accessed information.
- Block confirmed malicious indicators through approved security controls.
- Document the investigation and preserve relevant evidence.
- Escalate any additional suspicious findings.

## 6. Escalation Criteria

Escalate immediately if there is evidence of:

- Unauthorised account access.
- Suspicious successful sign-ins.
- MFA manipulation.
- Unauthorised changes to mailbox settings.
- Access to sensitive organisational information.

## 7. Conclusion

The incident should be treated as a potential credential compromise requiring urgent investigation.

The SOC Level 1 Analyst should preserve evidence, initiate escalation and support authorised containment activities.

**Final assessment:** Potential Microsoft 365 credential compromise – investigation and containment required.

**Disclaimer:** This is a simulated incident response exercise using fictional information.
