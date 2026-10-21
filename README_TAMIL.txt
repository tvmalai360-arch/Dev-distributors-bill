DEV DISTRIBUTORS BILLING APP — QUICK START
==========================================

இந்த package-ல் உள்ளவை:
• உங்கள் DEV OG 4.html-இன் billing fields, GST calculation, dealer tools, invoice history, print/PDF options ஆகியவை அடிப்படையாக வைத்துள்ள mobile-friendly UI.
• Business logo upload; logo invoice-ல் தெரியும்.
• Install செய்யக்கூடிய PWA அமைப்பு (HTTPS அல்லது localhost-ல் serve செய்யும்போது).
• SQLite database backend + invoice/dealer API.
• Offline-ல் local browser storage மூலம் draft/invoice save ஆகும்.

முக்கியமான வேறுபாடு:
இப்போது HTML-ல் draft/dealer records device/browser-இல் சேமிக்கப்படும். Invoice save செய்யும்போது backend கிடைத்தால் SQLite database-க்கும் mirror செய்யும். பல mobile/device-களில் ஒரே shared data வேண்டும் என்றால் hosting, authentication, மற்றும் முழுமையான cloud-sync அமைப்பை deploy செய்வது அவசியம். இந்த starter-ல் login/role security இன்னும் அமைக்கப்படவில்லை; இணையத்தில் public-ஆக deploy செய்வதற்கு முன் authentication சேர்க்கவும்.

RUN ON COMPUTER
1. Node.js 20+ install செய்யவும்.
2. இந்த folder-ல் terminal திறக்கவும்.
3. npm install
4. npm start
5. Browser-ல் http://localhost:3000 திறக்கவும்.

MOBILE APP போல install செய்ய:
• App-ஐ HTTPS domain-ல் host செய்யவும்.
• Android Chrome-ல் website திறந்து menu → Install app / Add to Home screen தேர்வு செய்யவும்.

HTML மட்டும் திறந்தால்:
public/index.html-ஐ நேரடியாக browser-ல் திறக்கலாம். Logo, draft, dealer details, history ஆகியவை அந்த browser/device storage-ல் மட்டுமே இருக்கும்; server database sync இயங்காது.

DATA BACKUP
SQLite file: dev-billing.sqlite (server இயங்கிய பின் உருவாகும்). Regular backup எடுக்கவும்.

TAX NOTE
GST கணக்கீடு source HTML-ல் உள்ள logic-ஐ அடிப்படையாகக் கொண்டது. Production tax compliance-க்கு accountant/qualified professional மூலம் சரிபார்க்கவும்.
