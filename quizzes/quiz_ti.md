# TI (IT / Technology) -- Knowledge Assessment
## Lakeshore Homes Professional Development Program

*This assessment helps us understand expertise across our team and identify areas for professional growth. Your responses will help us improve our technology systems and support every department more effectively.*

---

### Section A: Core Knowledge (Multiple Choice)

**Q1.** How many business processes are currently configured in the Const App (Hatchbox)?
- A) 8
- B) 12
- C) 16
- D) 20

**Q2.** What database engine does the Const App (Hatchbox) currently use?
- A) PostgreSQL
- B) MySQL
- C) SQLite
- D) MongoDB

**Q3.** How many executable services are in the Const App service catalog?
- A) 66
- B) 100
- C) 156
- D) 200

**Q4.** What is the primary communication tool used for subcontractor coordination (90%+ of communication)?
- A) Email
- B) Slack
- C) WhatsApp
- D) BuilderTrend messaging

**Q5.** What tool does the IT department use for automating access to county permit portals?
- A) Selenium
- B) Puppeteer
- C) Playwright
- D) Beautiful Soup

**Q6.** How many total users are currently in the Const App system?
- A) 15
- B) 25
- C) 35
- D) 50

**Q7.** What hosting platform runs the Const App?
- A) AWS EC2
- B) Heroku
- C) Hatchbox
- D) Render

**Q8.** Where are Power BI credentials stored?
- A) In the IT ticketing system
- B) In a board on Canva in the Slack channel #qps-tqm-private
- C) In the AWS Secrets Manager
- D) In the Const App admin panel

**Q9.** What is the critical hardware problem affecting the Takeoff and Design teams?
- A) Monitors are too small
- B) Company CPUs cannot adequately run AutoCAD, SketchUp, Enscape, and BlueBeam
- C) Network switches are failing
- D) Printers are not connected

**Q10.** The BuilderTrend-to-QuickBooks integration for "classes" (project classification) is:
- A) Fully automated
- B) Partially automated but manual for classes, consuming hours daily
- C) Not integrated at all
- D) Handled by a third-party middleware

---

### Section B: Process & Decision-Making (Open Response)

**Q11.** Walk us through what happens when a new employee starts and needs system access. List every system they might need access to, who requests the access, how long each provisioning step takes, and what the most common delays are.

**Q12.** Describe the real pain points of the BuilderTrend-to-Const App migration from the technical side. What data needs to be migrated, what cannot be migrated, and what will the transition period look like for users who need to work in both systems simultaneously?

**Q13.** When a department reports that "BuilderTrend is slow," what do you actually do to troubleshoot? Is it always a BT issue, or are there local factors? Walk us through your diagnostic process and the most common root causes.

**Q14.** Describe the actual process for programming a Playwright scraper for a new county portal. What information do you need from the Permits team, how long does it take, what breaks most often, and how do you handle portal redesigns?

**Q15.** Explain how you manage the SQLite database for the Const App. With 130 tables and growing, what is your backup strategy, what happens if the database corrupts, and at what scale does SQLite become a problem that requires migration to PostgreSQL?

**Q16.** Walk us through how the Power BI Gateway on the EC2 Windows instance works. What data flows through it, who maintains it, what happens when it goes down, and how do you monitor its health?

**Q17.** Describe the IT task queue system (IT_TASK_REQUEST). How do tasks actually get prioritized when you have 5 pending requests from different departments? What is your real decision process, not just the stated SLA levels?

**Q18.** When someone creates a Google Sheet as a personal tracking tool (which most departments do), how do you decide whether to let it continue, integrate it into a proper system, or replace it entirely? Give examples of sheets that should stay versus ones that need to be replaced.

**Q19.** Describe the challenges of supporting field workers who have poor internet connectivity. What tools work offline or with intermittent connection, and what workarounds have you developed for when BT or Slack cannot connect in the field?

**Q20.** Walk us through the actual process for deploying a new release of the Const App. What testing happens before deployment, who needs to be notified, what is the rollback plan if something goes wrong, and how do you handle it if the update breaks a workflow that a department depends on?

---

### Section C: Advanced Scenarios & Edge Cases (Open Response)

**Q21.** The Const App database is currently 2,880 KB with 130 tables. If Lakeshore scales to 500 simultaneous homes (from the current ~30-50), estimate the data growth. At what point does SQLite become untenable, what are the specific failure modes you would expect, and describe your migration plan to PostgreSQL including data integrity verification.

**Q22.** Three departments report issues simultaneously: (1) QuickBooks cannot import bills from BT, (2) the Power BI dashboard is showing stale data from yesterday, (3) a field supervisor cannot log into the Const App from their phone. How do you triage these, and what is your actual process for parallel debugging when you are the primary support person?

**Q23.** The Nathan AI quotation automation project achieved 90% accuracy in testing. Describe what the remaining 10% of failures look like, how you handle edge cases in PDF parsing, and what the feedback loop looks like when the AI generates an incorrect quotation that gets sent to a vendor.

**Q24.** A county portal that Lakeshore uses for permit scheduling (let's say Marion County) completely redesigns their website overnight, breaking the Playwright scraper. The permits team has 5 inspections to schedule today. Describe your immediate response, your workaround for today, and your process for rebuilding the scraper.

**Q25.** Candida and Gabriela (Takeoff/Design) are using their personal computers because company hardware cannot run their software. Describe the real security, data management, and compliance risks this creates. What would your ideal hardware solution look like, and how would you make the business case to get budget approval?

**Q26.** You discover that 15 of the 25 admin accounts in the Const App have the same default password (Lakeshore2026!). Some of these accounts access sensitive financial data. Describe your complete security remediation plan, including how you implement it without disrupting daily operations.

**Q27.** The Lakeshore team communicates across 6+ different tools (WhatsApp, Slack, BT, email, Google Sheets, verbal). Important decisions often happen in WhatsApp chats that are never recorded in any system. Describe your realistic strategy for improving this situation, acknowledging that you cannot force people to change overnight. What is the one change that would have the biggest impact?

**Q28.** Evandro is the Product Owner and primary developer of the Const App. What happens if Evandro is unavailable for an extended period? Describe the bus factor risk for the entire technology stack, which systems are most vulnerable, and what documentation or cross-training would you prioritize.

**Q29.** Describe the data flows between all Lakeshore systems -- BT, Const App, QuickBooks, Power BI, Google Sheets, Slack, WhatsApp, Zorro. Where does data get created, where does it get duplicated, where are the gaps, and where are the conflicts (same data with different values in different systems)? Which single integration, if built, would save the most person-hours per week?

**Q30.** If you were designing the Lakeshore IT infrastructure from scratch today (not migrating from existing systems), what would your architecture look like? Consider: 500 homes, multiple counties, concessionaire model requiring transferable systems, field workers with poor connectivity, bilingual team, zero cloud API cost requirement. What would you keep from the current stack and what would you replace?
