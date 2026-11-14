<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/wordmark-dark.svg">
  <img src="assets/wordmark-light.svg" width="100%" alt="Ivan Zamurenko">
</picture>

<p align="center"><strong>Full-stack development &amp; product engineering</strong></p>
<p align="center">Tralee, Ireland · Open to remote opportunities</p>
<p align="center"><a href="https://www.linkedin.com/in/ivan-zamurenko/">LinkedIn</a></p>
<p align="center">
  <a href="#dpd-assistance"><img src="assets/icons/logistics.svg" width="16" height="16" alt=""> DPD Assistance</a> &nbsp; · &nbsp;
  <a href="#handbalancers-studio"><img src="assets/icons/studio.svg" width="16" height="16" alt=""> Handbalancer’s Studio</a> &nbsp; · &nbsp;
  <a href="#food-delivery-analytics"><img src="assets/icons/analytics.svg" width="16" height="16" alt=""> Food Delivery Analytics</a>
</p>

I build web applications and tools for work that still involves too many manual steps. My projects cover logistics automation, software for handstand training and operational data analysis. I work across Python, JavaScript, TypeScript and SQL, with an interest in both the interface and the decisions behind it.

Below are three projects that show different parts of that work: handling uncertain outcomes, building an application from its foundations, and turning structured data into something useful.

### <img src="assets/icons/logistics.svg" width="20" height="20" alt=""> DPD Assistance

<p>
  <img src="assets/badges/javascript.svg" alt="JavaScript" height="20">
  <img src="assets/badges/chrome-manifest-v3.svg" alt="Chrome Manifest V3" height="20">
  <img src="assets/badges/nodejs.svg" alt="Node.js" height="20">
</p>

<p align="center"><a href="assets/logistics-automation.png"><img src="assets/logistics-automation.png" width="320" alt="Logistics extension popup showing Future Dates, Idle status, Dry Run enabled, and scan controls. No account data is displayed."></a></p>
<p align="center"><sub>EXTENSION INTERFACE · IDLE STATE · RENDERED LOCALLY</sub></p>

<details open>
<summary>Recovery &amp; redelivery — navigation report</summary>

<p align="center"><a href="assets/dpd-route-recovery.png"><img src="assets/dpd-route-recovery.png" width="800" alt="Locally rendered parcel-recovery report with synthetic data and two Google Maps navigation links: the recorded delivery point and destination Eircode. Not a live Discord or map capture."></a></p>
<p align="center"><sub>RECOVERY REPORT · LOCAL PREVIEW · SYNTHETIC DATA</sub></p>

</details>

A Chrome extension and supporting tools for parcel-processing workflows. The project brings together barcode scanning, browser interactions and service integrations to reduce repetitive steps in handling shipments.

The interesting engineering problem is what happens when an action does not finish cleanly. An interrupted request can leave a write's outcome uncertain; immediately trying again may repeat an action. The repository includes tests for bounded retries, cancellation and uncertain writes. Those cases are a useful window into how the project handles failure.

For a parcel left in the wrong place, the bot's `/report` flow can provide two driving-navigation links: one to the selected delivery event's GPS point, when available, and another to the destination Eircode. Each opens navigation from the driver's current location. The example above uses synthetic data and the project's report formatter; it shows the report output, not a live map or an optimised multi-stop route.

The code has evolved beyond its original Gmail-focused name. AI-assisted features remain planned work.

[Explore the repository →](https://github.com/ivan-zamurenko/gmail-ai-assistant)

---

### <img src="assets/icons/studio.svg" width="20" height="20" alt=""> Handbalancer’s Studio

<p>
  <img src="assets/badges/python.svg" alt="Python" height="20">
  <img src="assets/badges/fastapi.svg" alt="FastAPI" height="20">
  <img src="assets/badges/postgresql.svg" alt="PostgreSQL" height="20">
  <img src="assets/badges/jinja.svg" alt="Jinja" height="20">
  <img src="assets/badges/javascript.svg" alt="JavaScript" height="20">
</p>

<a href="assets/studio-home.png"><img src="assets/studio-home.png" width="100%" alt="Handbalancer’s Studio: the current English homepage, with a responsive navigation bar and the headline Move more freely. Feel better."></a>
<p align="center"><sub>HANDBALANCER’S STUDIO · CURRENT BUILD · SOURCE PRIVATE</sub></p>

<details>
<summary>View 2 more screens — mobile sign-in &amp; dark plans</summary>

<p align="center"><a href="assets/studio-login-mobile.png"><img src="assets/studio-login-mobile.png" width="300" alt="Current Studio mobile sign-in screen with empty email and password fields and a Google sign-in button."></a></p>
<p align="center"><sub>MOBILE SIGN-IN · LOCAL CAPTURE · EMPTY FORM</sub></p>

<p align="center"><a href="assets/studio-plans-dark.png"><img src="assets/studio-plans-dark.png" width="800" alt="Studio dark-theme plans page. Its notice says payments and AI analysis are not available yet; the plans describe intended support."></a></p>
<p align="center"><sub>DARK THEME · PLANS INTERFACE · PAYMENTS NOT LIVE</sub></p>

</details>

A web application I'm building for handstand training. The aim is to bring programmes, practice and coaching into one place. The current work establishes the foundation: public pages, account flows, and a responsive interface in Ukrainian and English, with light and dark themes.

The application uses a Python backend, PostgreSQL and server-rendered pages with vanilla JavaScript. That gives me one project in which to work on database changes, backend behaviour and the details someone actually sees: navigation on a small screen, form feedback and loading states.

Recent work has focused on mobile navigation and account screens. Training workflows and subscriptions are planned features, and some authentication checks still depend on the external environment. The application is in development; its source code is private. The screenshots show the current homepage, mobile sign-in and dark-theme plans interface, captured locally. The plans describe intended support; payments are not live.

---

### <img src="assets/icons/analytics.svg" width="20" height="20" alt=""> Food Delivery Analytics

<p>
  <img src="assets/badges/python.svg" alt="Python" height="20">
  <img src="assets/badges/pandas.svg" alt="pandas" height="20">
  <img src="assets/badges/postgresql.svg" alt="PostgreSQL" height="20">
  <img src="assets/badges/sqlalchemy.svg" alt="SQLAlchemy" height="20">
</p>

<p align="center"><a href="assets/food-delivery-analytics.png"><img src="assets/food-delivery-analytics.png" width="680" alt="An existing analysis chart comparing average delivery time across driver categories in the Brazilian food-delivery dataset."></a></p>
<p align="center"><sub>FOOD DELIVERY ANALYTICS · EXPORTED ANALYSIS RESULT</sub></p>

<details>
<summary>View 2 more charts — hub comparison &amp; payment trends</summary>

<p align="center"><a href="assets/delivery-hub-comparison.png"><img src="assets/delivery-hub-comparison.png" width="800" alt="Two exported charts comparing the ten leading delivery hubs by store count and revenue in the dataset."></a></p>
<p align="center"><sub>HUB COMPARISON · EXPORTED DATASET ANALYSIS</sub></p>

<p align="center"><a href="assets/delivery-payment-trends.png"><img src="assets/delivery-payment-trends.png" width="800" alt="Exported line charts showing payment-method shares from January to April 2021 in the food-delivery dataset."></a></p>
<p align="center"><sub>PAYMENT-METHOD TRENDS · EXPORTED DATASET ANALYSIS</sub></p>

</details>

A Python and PostgreSQL project that brings together delivery, order and payment data from a Brazilian food-delivery dataset. It calculates grouped metrics and produces reports and charts that can be inspected alongside the analysis code.

The work covers data cleaning, relational queries and calculations around delivery performance and payments. The repository includes calculation tests and data-quality checks. This complements my application work with examples of transforming data, checking assumptions and making results understandable.

The gallery contains existing outputs from the repository: delivery times, hub comparisons and payment-method trends. These are static dataset analyses, not live dashboards or claims of operational improvement.

[Explore the repository →](https://github.com/ivan-zamurenko/Delivery-Food-Center-in-Brazil)

## Let's talk

I'm looking for a remote **Full-stack or Product Engineer** role with a team hiring in Ireland. If these projects are relevant to what you're building, I'd be glad to talk through the code and the decisions behind it.

[Get in touch on LinkedIn →](https://www.linkedin.com/in/ivan-zamurenko/)
