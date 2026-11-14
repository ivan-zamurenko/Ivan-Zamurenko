<!doctype html><html lang="en"><head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1"><title>Ivan Zamurenko — GitHub profile preview</title><style>*{box-sizing:border-box}body{margin:0;background:#f6f8fa;color:#1f2328;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif;font-size:16px;line-height:1.5}.preview-note{max-width:960px;margin:20px auto 12px;padding:0 24px;color:#59636e;font-size:12px}.markdown-body{max-width:960px;margin:0 auto 40px;padding:32px;border:1px solid #d1d9e0;border-radius:6px;background:#fff;overflow-wrap:break-word}.markdown-body>:first-child{margin-top:0!important}.markdown-body>:last-child{margin-bottom:0!important}themed-picture,picture{display:block}img{max-width:100%;height:auto;box-sizing:content-box}p{margin:0 0 16px}h2,h3{font-weight:600;line-height:1.25;margin:24px 0 16px}h2{font-size:1.5em;border-bottom:1px solid #d1d9e0b3;padding-bottom:.3em}h3{font-size:1.25em}a{color:#0969da;text-decoration:none}a:hover{text-decoration:underline}a:focus-visible{outline:2px solid #0969da;outline-offset:3px}hr{height:.25em;padding:0;margin:24px 0;background:#d1d9e0;border:0}sub{font-size:75%;line-height:0;position:relative;vertical-align:baseline;bottom:-.25em}@media(max-width:700px){.preview-note{margin:12px 0;padding:0 16px}.markdown-body{padding:16px;border-left:0;border-right:0;border-radius:0;margin-bottom:0}}@media(prefers-color-scheme:dark){body{background:#010409;color:#f0f6fc}.markdown-body{background:#0d1117;border-color:#3d444d}h2{border-color:#3d444db3}hr{background:#3d444d}a{color:#4493f8}.preview-note{color:#9198a1}}summary{cursor:pointer;margin-bottom:16px}details{margin-bottom:16px}summary:focus-visible{outline:2px solid #0969da;outline-offset:3px}</style></head><body><p class="preview-note">LOCAL PREVIEW · GitHub-rendered Markdown with approximate GitHub styling · Unpublished</p><article class="markdown-body"><themed-picture data-catalyst-inline="true"><picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/wordmark-dark.svg">
  <img src="assets/wordmark-light.svg" width="100%" alt="Ivan Zamurenko">
</picture></themed-picture>
<p align="center" dir="auto"><strong>Full-stack development &amp; product engineering</strong></p>
<p align="center" dir="auto">Tralee, Ireland · Open to remote opportunities</p>
<p align="center" dir="auto"><a href="https://www.linkedin.com/in/ivan-zamurenko/" rel="nofollow">LinkedIn</a></p>
<p align="center" dir="auto">
  <a href="#dpd-assistance"><img src="assets/icons/logistics.svg" width="16" height="16" alt="" style="max-width: 100%; height: auto; max-height: 16px;"> DPD Assistance</a>   ·  
  <a href="#handbalancers-studio"><img src="assets/icons/studio.svg" width="16" height="16" alt="" style="max-width: 100%; height: auto; max-height: 16px;"> Handbalancer’s Studio</a>   ·  
  <a href="#food-delivery-analytics"><img src="assets/icons/analytics.svg" width="16" height="16" alt="" style="max-width: 100%; height: auto; max-height: 16px;"> Food Delivery Analytics</a>
</p>
<p dir="auto">I build web applications and tools for work that still involves too many manual steps. My projects cover logistics automation, software for handstand training and operational data analysis. I work across Python, JavaScript, TypeScript and SQL, with an interest in both the interface and the decisions behind it.</p>
<p dir="auto">Below are three projects that show different parts of that work: handling uncertain outcomes, building an application from its foundations, and turning structured data into something useful.</p>
<h3 id="dpd-assistance" dir="auto"><a target="_blank" rel="noopener noreferrer" href="assets/icons/logistics.svg"><img src="assets/icons/logistics.svg" width="20" height="20" alt="" style="max-width: 100%; height: auto; max-height: 20px;"></a> DPD Assistance</h3>
<p dir="auto">
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/javascript.svg"><img src="assets/badges/javascript.svg" alt="JavaScript" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/chrome-manifest-v3.svg"><img src="assets/badges/chrome-manifest-v3.svg" alt="Chrome Manifest V3" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/nodejs.svg"><img src="assets/badges/nodejs.svg" alt="Node.js" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
</p>
<p align="center" dir="auto"><a href="assets/logistics-automation.png"><img src="assets/logistics-automation.png" width="320" alt="Logistics extension popup showing Future Dates, Idle status, Dry Run enabled, and scan controls. No account data is displayed." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>EXTENSION INTERFACE · IDLE STATE · RENDERED LOCALLY</sub></p>
<details open="">
<summary>Recovery &amp; redelivery — navigation report</summary>
<p align="center" dir="auto"><a href="assets/dpd-route-recovery.png"><img src="assets/dpd-route-recovery.png" width="800" alt="Locally rendered parcel-recovery report with synthetic data and two Google Maps navigation links: the recorded delivery point and destination Eircode. Not a live Discord or map capture." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>RECOVERY REPORT · LOCAL PREVIEW · SYNTHETIC DATA</sub></p>
</details>
<p dir="auto">A Chrome extension and supporting tools for parcel-processing workflows. The project brings together barcode scanning, browser interactions and service integrations to reduce repetitive steps in handling shipments.</p>
<p dir="auto">The interesting engineering problem is what happens when an action does not finish cleanly. An interrupted request can leave a write's outcome uncertain; immediately trying again may repeat an action. The repository includes tests for bounded retries, cancellation and uncertain writes. Those cases are a useful window into how the project handles failure.</p>
<p dir="auto">For a parcel left in the wrong place, the bot's <code class="notranslate">/report</code> flow can provide two driving-navigation links: one to the selected delivery event's GPS point, when available, and another to the destination Eircode. Each opens navigation from the driver's current location. The example above uses synthetic data and the project's report formatter; it shows the report output, not a live map or an optimised multi-stop route.</p>
<p dir="auto">The code has evolved beyond its original Gmail-focused name. AI-assisted features remain planned work.</p>
<p dir="auto"><a href="https://github.com/ivan-zamurenko/gmail-ai-assistant">Explore the repository →</a></p>
<hr>
<h3 id="handbalancers-studio" dir="auto"><a target="_blank" rel="noopener noreferrer" href="assets/icons/studio.svg"><img src="assets/icons/studio.svg" width="20" height="20" alt="" style="max-width: 100%; height: auto; max-height: 20px;"></a> Handbalancer’s Studio</h3>
<p dir="auto">
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/python.svg"><img src="assets/badges/python.svg" alt="Python" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/fastapi.svg"><img src="assets/badges/fastapi.svg" alt="FastAPI" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/postgresql.svg"><img src="assets/badges/postgresql.svg" alt="PostgreSQL" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/jinja.svg"><img src="assets/badges/jinja.svg" alt="Jinja" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/javascript.svg"><img src="assets/badges/javascript.svg" alt="JavaScript" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
</p>
<p dir="auto"><a href="assets/studio-home.png"><img src="assets/studio-home.png" width="100%" alt="Handbalancer’s Studio: the current English homepage, with a responsive navigation bar and the headline Move more freely. Feel better." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>HANDBALANCER’S STUDIO · CURRENT BUILD · SOURCE PRIVATE</sub></p>
<details>
<summary>View 2 more screens — mobile sign-in &amp; dark plans</summary>
<p align="center" dir="auto"><a href="assets/studio-login-mobile.png"><img src="assets/studio-login-mobile.png" width="300" alt="Current Studio mobile sign-in screen with empty email and password fields and a Google sign-in button." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>MOBILE SIGN-IN · LOCAL CAPTURE · EMPTY FORM</sub></p>
<p align="center" dir="auto"><a href="assets/studio-plans-dark.png"><img src="assets/studio-plans-dark.png" width="800" alt="Studio dark-theme plans page. Its notice says payments and AI analysis are not available yet; the plans describe intended support." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>DARK THEME · PLANS INTERFACE · PAYMENTS NOT LIVE</sub></p>
</details>
<p dir="auto">A web application I'm building for handstand training. The aim is to bring programmes, practice and coaching into one place. The current work establishes the foundation: public pages, account flows, and a responsive interface in Ukrainian and English, with light and dark themes.</p>
<p dir="auto">The application uses a Python backend, PostgreSQL and server-rendered pages with vanilla JavaScript. That gives me one project in which to work on database changes, backend behaviour and the details someone actually sees: navigation on a small screen, form feedback and loading states.</p>
<p dir="auto">Recent work has focused on mobile navigation and account screens. Training workflows and subscriptions are planned features, and some authentication checks still depend on the external environment. The application is in development; its source code is private. The screenshots show the current homepage, mobile sign-in and dark-theme plans interface, captured locally. The plans describe intended support; payments are not live.</p>
<hr>
<h3 id="food-delivery-analytics" dir="auto"><a target="_blank" rel="noopener noreferrer" href="assets/icons/analytics.svg"><img src="assets/icons/analytics.svg" width="20" height="20" alt="" style="max-width: 100%; height: auto; max-height: 20px;"></a> Food Delivery Analytics</h3>
<p dir="auto">
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/python.svg"><img src="assets/badges/python.svg" alt="Python" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/pandas.svg"><img src="assets/badges/pandas.svg" alt="pandas" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/postgresql.svg"><img src="assets/badges/postgresql.svg" alt="PostgreSQL" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
  <a target="_blank" rel="noopener noreferrer" href="assets/badges/sqlalchemy.svg"><img src="assets/badges/sqlalchemy.svg" alt="SQLAlchemy" height="20" style="max-width: 100%; height: auto; max-height: 20px;"></a>
</p>
<p align="center" dir="auto"><a href="assets/food-delivery-analytics.png"><img src="assets/food-delivery-analytics.png" width="680" alt="An existing analysis chart comparing average delivery time across driver categories in the Brazilian food-delivery dataset." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>FOOD DELIVERY ANALYTICS · EXPORTED ANALYSIS RESULT</sub></p>
<details>
<summary>View 2 more charts — hub comparison &amp; payment trends</summary>
<p align="center" dir="auto"><a href="assets/delivery-hub-comparison.png"><img src="assets/delivery-hub-comparison.png" width="800" alt="Two exported charts comparing the ten leading delivery hubs by store count and revenue in the dataset." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>HUB COMPARISON · EXPORTED DATASET ANALYSIS</sub></p>
<p align="center" dir="auto"><a href="assets/delivery-payment-trends.png"><img src="assets/delivery-payment-trends.png" width="800" alt="Exported line charts showing payment-method shares from January to April 2021 in the food-delivery dataset." style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><sub>PAYMENT-METHOD TRENDS · EXPORTED DATASET ANALYSIS</sub></p>
</details>
<p dir="auto">A Python and PostgreSQL project that brings together delivery, order and payment data from a Brazilian food-delivery dataset. It calculates grouped metrics and produces reports and charts that can be inspected alongside the analysis code.</p>
<p dir="auto">The work covers data cleaning, relational queries and calculations around delivery performance and payments. The repository includes calculation tests and data-quality checks. This complements my application work with examples of transforming data, checking assumptions and making results understandable.</p>
<p dir="auto">The gallery contains existing outputs from the repository: delivery times, hub comparisons and payment-method trends. These are static dataset analyses, not live dashboards or claims of operational improvement.</p>
<p dir="auto"><a href="https://github.com/ivan-zamurenko/Delivery-Food-Center-in-Brazil">Explore the repository →</a></p>
<h2 dir="auto">Let's talk</h2>
<p dir="auto">I'm looking for a remote <strong>Full-stack or Product Engineer</strong> role with a team hiring in Ireland. If these projects are relevant to what you're building, I'd be glad to talk through the code and the decisions behind it.</p>
<p dir="auto"><a href="https://www.linkedin.com/in/ivan-zamurenko/" rel="nofollow">Get in touch on LinkedIn →</a></p></article></body></html>
