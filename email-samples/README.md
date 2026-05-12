# Phishing Email Samples Analyzed

## Email Sample #1: CNN SUSPICIOUS (Server Not Found)

**FROM:** CNN Alerts <alerts@custom-cnn.net>
**TO:** victim@email.com
**SUBJECT:** CNN Alerts: My Custom Alert

Dear CNN Member,

You have requested to receive custom alerts from CNN.

Your Custom Alert Summary:
- Stock market update: Dow Jones rises 200 points
- Weather alert: Thunderstorms expected in your area
- Breaking news: Developing story in Washington

VIEW YOUR CUSTOM ALERT: http://cnn-alerts-security-check.com/verify

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

**URL Analyzed:** http://cnn-alerts-security-check.com/verify

**Result in DevTools:** Server Not Found (DNS resolution failed)

**Red Flags:**
- Fake domain: cnn-alerts-security-check.com (real CNN uses cnn.com)
- Missing HTTPS: http:// instead of https://
- Domain not resolving (likely reported/shutdown)

---

## Email Sample #2: CNN Phishing (Fake News)

**FROM:** CNN.com Daily Top 10 <newsletter@cnn-mail.com>
**TO:** victim@email.com
**SUBJECT:** CNN.com Daily Top 10

Top 10 News Stories Today

1. Breaking: Presidential candidates debate economy
2. Storm chasers track Hurricane Bertha
3. Oil prices drop to $118 per barrel
4. Olympics opening ceremony preview

CLICK HERE FOR FULL STORY: http://fake-news-updates.com/click.php?id=3847

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

**URL Analyzed:** http://fake-news-updates.com/click.php?id=3847

**Result in DevTools:** 500 error, CSP violations

**Red Flags:**
- Fake domain: fake-news-updates.com
- Suspicious path: /click.php?id= (tracking parameter)
- 500 server error

---

## Email Sample #3: Safe Email (LinkedIn - For Comparison)

**FROM:** LinkedIn <messages-noreply@linkedin.com>
**TO:** user@gmail.com
**SUBJECT:** Sarah Miller wants to connect with you

Hi [Name],

Sarah Miller (Software Engineer at Google) wants to connect with you on LinkedIn.

View Invitation: https://www.linkedin.com/in/sarahmiller

This invitation will expire in 30 days.

- The LinkedIn Team

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

**URL Analyzed:** https://www.linkedin.com

**Why It's Safe:**
- Legitimate domain: linkedin.com
- HTTPS present
- Security headers visible (x-li-pop, x-li-uuid)
- Valid cookies (JSESSIONID, bscookie)
