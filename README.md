# annonymous-suggestion-box
Beautiful, anonymous suggestion form powered by emailJS

**Setup Instructions (takes 5 minutes):**
1. Create EmailJS Account (Free)

Go to emailjs.com and sign up
It's completely free for up to 200 emails/month

2. Configure EmailJS Service

Add an Email Service (choose Gmail)
Connect it to any Gmail account (can be a dummy one)

3. Create Email Template

Create a new template with this content:

Template Settings:
```
Template Name: Anonymous Suggestion Template
Subject: New Anonymous Suggestion
From Name: Suggestion Box
From Email: {{from_email}} (leave as is)
To Email: imsinu9@gmail.com ← Put your email here
```

Template Content (HTML Body):
```
html<h3>New Anonymous Suggestion</h3>
<p><strong>Suggestion:</strong></p>
<p>{{suggestion}}</p>
<p><strong>Submitted:</strong> {{timestamp}}</p>
<p><strong>Session ID:</strong> {{session_id}}</p>
<hr>
<p><em>This suggestion was submitted anonymously through your Slack suggestion box.</em></p>

Click "Save" - you'll get a Template ID (like template_xyz123)

```

Set the To Email to: <Your Email>

4. Update the HTML File
Replace these placeholders in the code:

```
YOUR_PUBLIC_KEY → Your EmailJS public key
YOUR_SERVICE_ID → Your service ID
YOUR_TEMPLATE_ID → Your template ID
```

Key Features for Anonymous Comfort:
✅ Zero Tracking - No IP addresses, no cookies, no analytics
✅ Encouraging Language - Specifically mentions complaints are welcome
✅ Safe Space Messaging - Reassures users it's judgment-free
✅ Anonymous Session ID - Only for your tracking, not linked to users
✅ Direct Email Delivery - You'll get suggestions in your inbox instantly
How Users Will Feel Comfortable:

Welcoming Tone: "Your candid input helps me grow"
Explicit Permission: "complaints included!"
Safety Assurance: "100% Anonymous & Safe"
Encouraging Placeholder: Mentions all types of feedback are valuable

The form will send you an email like this:
```
Subject: New Anonymous Suggestion
From: your-emailjs-service@gmail.com
To: <Your Email>

New Anonymous Suggestion

Suggestion: [Their feedback here]
Submitted: 12/29/2021, 3:45:23 PM
Session: ANON_k7x9m2p4q
```
