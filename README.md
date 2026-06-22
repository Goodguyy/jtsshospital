
<!-- ═══════════════════════════════════════════════════════════
     EMAILJS SETUP GUIDE — DELETE THIS BLOCK ONCE CONFIGURED
     ═══════════════════════════════════════════════════════════ -->
<div id="setupGuide" style="background:#fef3c7;border-top:3px solid #f59e0b;padding:2.5rem;font-family:monospace;font-size:.88rem;line-height:1.8;color:#1e2a26">
  <strong style="font-size:1rem;font-family:sans-serif">⚙️ EmailJS Setup Guide (remove this section once done)</strong><br><br>

  <strong>STEP 1 — Create a free EmailJS account</strong><br>
  → Go to <a href="https://www.emailjs.com" target="_blank">https://www.emailjs.com</a> and sign up free<br>
  → Free plan: 200 emails/month (more than enough for appointments)<br><br>

  <strong>STEP 2 — Add your Email Service</strong><br>
  → Dashboard → Email Services → Add New Service → choose <em>Gmail</em><br>
  → Connect <strong>johntheresahosp@gmail.com</strong> (allow permissions)<br>
  → Copy your <strong>Service ID</strong> (looks like: <code>service_abc1234</code>)<br>
  → Paste it into <code>EMAILJS_SERVICE_ID</code> in the script above<br><br>

  <strong>STEP 3 — Create an Email Template</strong><br>
  → Dashboard → Email Templates → Create New Template<br>
  → Set <strong>To Email</strong>: <code>johntheresahosp@gmail.com</code><br>
  → Set <strong>Subject</strong>: <code>New Appointment Request — {{department}}</code><br>
  → Set <strong>Body</strong> (copy this exactly):<br>
  <pre style="background:#fff;padding:1rem;border-radius:8px;margin:.5rem 0;white-space:pre-wrap">New appointment request received:

Patient Name:  {{from_name}}
Phone:         {{phone}}
Email:         {{reply_to}}
Department:    {{department}}
Preferred Date: {{appt_date}}
Notes:         {{message}}

Please call the patient within 24 hours to confirm.</pre>
  → Save and copy your <strong>Template ID</strong> (looks like: <code>template_xyz7890</code>)<br>
  → Paste it into <code>EMAILJS_TEMPLATE_ID</code> in the script above<br><br>

  <strong>STEP 4 — Get your Public Key</strong><br>
  → Dashboard → Account → API Keys → copy <strong>Public Key</strong><br>
  → Paste it into <code>EMAILJS_PUBLIC_KEY</code> in the script above<br><br>

  <strong>STEP 5 — Test it</strong><br>
  → Fill the appointment form and submit<br>
  → Check <strong>johntheresahosp@gmail.com</strong> inbox (also check Spam folder first time)<br><br>

  <strong>STEP 6 — Clean up</strong><br>
  → Delete this entire yellow setup guide section from the HTML file<br>
  → Push to GitHub — done! ✅
</div>
</body>
</html>
