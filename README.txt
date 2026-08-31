# Dominators FC Website Update

Files:
- index.html — public website
- script.js — Firestore-powered public content loader
- style.css — public website styles
- admin.html — professional admin control center
- admin.js — admin editor + Firestore saving
- admin.css — admin UI
- firestore.rules — simple rules required by this password-in-Firestore implementation

Default admin password: 12345678

Firestore:
- siteContent/main = all editable website content
- adminSettings/main = { password: "12345678", updatedAt: ... }

Important:
This requested password-in-Firestore design requires unauthenticated read/write access to these two documents, so it is not appropriate for a public production system. For stronger security, migrate the admin login to Firebase Authentication and protect Firestore with authenticated role rules.

Keep your existing images/ folder beside these files.
