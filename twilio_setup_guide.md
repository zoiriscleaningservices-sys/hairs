# Twilio Automatic SMS Setup Guide - Styles by Cece

This guide explains how to connect **Twilio** to your booking form on [Formspree](https://formspree.io) so clients automatically receive a text message (SMS) on their mobile phones as soon as they submit an appointment request.

---

## 1. Get Your Free Twilio Credentials

1. Sign up or log into [Twilio Console](https://console.twilio.com/).
2. On your Twilio Dashboard, click **Get a Trial Number** (or purchase a dedicated local number for ~$1.15/mo).
3. Copy the following 3 credentials:
   - **Account SID**: `ACxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`
   - **Auth Token**: `your_auth_token_here`
   - **Twilio Phone Number**: `+1251xxxxxxx`

---

## 2. Connect Twilio in Formspree

1. Log into [formspree.io](https://formspree.io) and open your form **`xgvnwajw`**.
2. Click on **Plugins** / **Integrations** in the left menu.
3. Choose **Twilio** (or **Zapier** / **Make**).
4. Enter your Twilio credentials:
   - **Account SID**: `AC...`
   - **Auth Token**: `[Your Token]`
   - **From Number**: `[Your Twilio Number]`
   - **To Field**: `phone`
5. Enter the automated SMS template:
   ```text
   Hi {{name}}! Your booking request for {{service}} on {{date}} with Styles by Cece is RECEIVED! 💇‍♀️ A $10 deposit is required to secure your spot. Location: Downtown Mobile, AL. Stylist Tel: (251) 545-8911.
   ```
6. Click **Save & Enable**.

---

## 3. Test The Integration

1. Go to [www.stylesbycece.com](https://www.stylesbycece.com#booking).
2. Submit a test booking with your own mobile phone number.
3. Check your cell phone — you will receive the automatic SMS text message directly from your Twilio number!
