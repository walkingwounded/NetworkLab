# APC NMC Email Alert Setup via Gmail SMTP (AP9544)

Date: 21 April 2025

Engineer: Clyde

Device: APC Smart-UPS NMC (AP9544)

Objective: Configure email alert notifications via Gmail SMTP

## Summary

Configured APC Network Management Card (NMC) to send system alerts via Gmail SMTP server using TLS authentication. This allows proactive alerting for power events and device status monitoring.

## Environment

Device: APC AP9544 (NMC3)

UPS Model: SRV1Ki-e, Single Phase UPS

Firmware Version: N/A

Email Service: Gmail SMTP (smtp.gmail.com)

## Steps Taken

1. Identify NMC IP; configuration performed through web browser.
  
3. Enabled Email Alert under Configuration > Notification > Recipient

Configured the following:

2. SMTP Server: smtp.gmail.com

3. Port: 25

4. Use SSL/TLS: ALWAYS

5. Enable *CA Root Certificate*

6. SMTP Authentication: Enabled

7. Sender Email: your_email@gmail.com

8. Recipient Email: your_alerts@yourcompany.com

9. Generated an *App Password* from Google Account (2FA enabled)

10. Used *App Password* in SMTP authentication

11. Tested email alerts: **successfully received email notifications**

12. Configured notification intervals at Notification > Events

## Test Result

Power failure simulated: alert received within 30 seconds

Status alerts (e.g., battery disconnected): received

Note: Run test using APC *Test Email* prior simulating actual power interruption

## Lessons / Notes

Gmail documentation: https://support.google.com/a/answer/176600?hl=en

APC documentation: https://www.apc.com/us/en/faqs/FA156064/

Gmail limits up to 2000 emails a day.

## Conclusion

Successfully configured email notifications via Gmail for APC UPS alerts. Reliable method for small-to-medium IT setups without an internal mail server.








