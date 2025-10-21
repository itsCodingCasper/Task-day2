# Phishing Email Indicators Report

## Sample Email

**Subject:** Important: Confirm Your Account Suspension Notice

**From:** "PayPal Support" <support@paypalsecure-alerts.com>

**To:** you@example.com

> Dear Customer,
>
> We noticed unusual activity on your PayPal account and have temporarily limited access to protect your security. Please confirm your identity to restore full account functionality.
>
> Click the button below to verify your account:
>
> **[Verify My Account Now]:**
>
> Failure to verify within 24 hours will result in permanent account suspension.
>
> Thank you for choosing PayPal.
>
> — The PayPal Security Team


## Indicators

1. **Fake Sender Domain**
   - "support@paypalsecure-alerts.com" is not a legitimate PayPal domain; official PayPal emails use "@paypal.com".
   - *Screenshot: sender-address.png*

2. **Generic Recipient**
   - Addressed to "you@example.com" and uses "Dear Customer" rather than your full name.
   - *Screenshot: generic-greeting.png*

3. **Urgent Language and Threats**
   - The email warns of “permanent account suspension” if actions are not taken within 24 hours.
   - *Screenshot: urgency-threat.png*

4. **Suspicious Verification Link**
   - The button says “Verify My Account Now,” which is not a standard PayPal process; hovering over the link reveals a non-PayPal URL.
   - *Screenshot: suspicious-link.png*
   - *link_scan_result.png*: (Include screenshot or result of a free phishing link scan)

5. **Unprofessional Format**
   - Noticeable formatting issues such as odd line breaks or excessive spaces that differ from legitimate PayPal communication.
   - *Screenshot: formatting-issues.png*

6. **Generic Signature**
   - Signed as "The PayPal Security Team" rather than listing actual support contacts.
   - *Screenshot: signature.png*

## Email Header Analysis

- [email_header.txt]: Full raw header pasted for reference.
- Noted lack of SPF/DKIM/DMARC authentication or mismatched reply-to fields, showing evidence of spoofing.

## Conclusion

Based on these factors, the email shows multiple signs typical of phishing attempts and should NOT be trusted.
