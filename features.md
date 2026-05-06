# Engineering Firm Project Management — Feature & Functionality Survey

> Candidate #326 · Researched: 2026-05-03

## Solutions Analysed

| Tool | Type | Licence / Model | URL |
|------|------|-----------------|-----|
| Deltek Vantagepoint | Enterprise ERP/PM | Commercial — Quote only | https://www.deltek.com/en/erp/vantagepoint |
| BQE CORE | Cloud SaaS PSA | Commercial — Quote only | https://www.bqe.com/ |
| Unanet ERP AE | Cloud SaaS ERP | Commercial — Quote only | https://unanet.com/erp-for-a-e/erp-for-a-e-overview |
| Monograph | Cloud SaaS PM | Commercial — $30–$55/user/month | https://monograph.com/ |
| BigTime | Cloud SaaS PSA | Commercial — From $20/user/month | https://www.bigtime.net/ |
| Productive | Cloud SaaS PM/PSA | Commercial — From $10/user/month | https://productive.io/ |
| Birdview PSA | Cloud SaaS PM/PSA | Commercial — Tiered | https://birdviewpsa.com/ |
| Factor AE | Cloud SaaS PM | Commercial — Tiered | https://factorapp.com/ |

---

## Feature Analysis by Solution

### Deltek Vantagepoint

**Core features**
- Integrated CRM, business development, and project pursuit tracking
- Phase-based project accounting with multi-stage billing (T&M, fixed-fee, milestone)
- Earned Value Management (EVM) with BCWS, BCWP, ACWP calculations
- DCAA-compliant indirect cost rate structure and audit trail
- Resource planning with colour-coded capacity dashboards and utilisation reporting
- General ledger, accounts payable/receivable, and financial statements
- Real-time project health dashboards with profitability and margin tracking
- Multi-company and multi-currency support for global engineering firms
- Document management with version control
- Mobile time and expense entry

**Differentiating features**
- Industry standard for large A&E government contractors; built-in DCAA compliance
- Deepest integration of project accounting with EVM in the mid-to-enterprise market
- Built-in AI agent ("Vantagepoint AI") for natural language data queries
- Broad ecosystem of certified implementation partners and add-on modules

**UX patterns**
- Role-based dashboards for project managers, finance, and principals
- Highly configurable hub-based data model; steep learning curve for non-accountants
- Desktop-first with progressively added cloud and mobile layers

**Integration points**
- REST API covering configuration, hubs, and transactions (vantagepointapi.deltek.com)
- Native integrations with Microsoft 365, Teams, and SharePoint
- Deltek ecosystem: Cobra (EVM), Acumen, and Costpoint for government contracting

**Known gaps**
- UI is complex and not intuitive for non-finance users; described as "built for accountants"
- Reporting is cumbersome and less flexible than users expect
- Features from predecessor Deltek Vision (e.g. pinning phases, custom layouts) were removed and not yet fully restored
- Embedded AI agent receives poor reviews — inconsistent responses and long reply times
- Requires significant implementation investment; not suited to small firms
- Timesheets require horizontal scrolling; mobile experience is limited

**Licence / IP notes**
- Proprietary commercial software; source code not disclosed
- Pricing requires direct sales engagement; typically $50,000+ annual for mid-size firms

---

### BQE CORE

**Core features**
- Integrated time and expense tracking with mobile support
- Flexible billing engine: T&M, fixed-fee, milestone, retainer, and percentage-complete
- Project budgeting by phase, task, and fee type
- Integrated payroll and HR functionality
- Accounts receivable, accounts payable, and general ledger
- Batch invoicing with customisable invoice templates
- Business intelligence dashboards and KPI reporting
- Sub-consultant management and expense pass-through billing
- Client portal for invoice review and payment

**Differentiating features**
- All-in-one: combines accounting, payroll, billing, and project management in one product
- Strong automation for repetitive billing workflows
- Embedded payroll reduces need for third-party payroll software

**UX patterns**
- Wizard-driven billing workflow reduces errors before invoicing
- Highly configurable invoice templates
- Progressive disclosure: detailed accounting functions behind simpler PM-facing views

**Integration points**
- REST API with OAuth 2.0; developer portal at api-developer.bqecore.com
- Native QuickBooks Online and Desktop sync
- Integrations with Stripe, ADP, and accounting platforms
- Sample SDKs in ASP.NET MVC, Java, PHP, Angular, and iOS

**Known gaps**
- Initial configuration is complex; onboarding takes significant time
- Not optimised for DCAA government contracting at enterprise scale
- Reporting depth is strong but custom report building is not self-service
- Mobile experience trails desktop capabilities

**Licence / IP notes**
- Proprietary commercial SaaS; no open-source components
- Pricing is quote-based at mid-market tier

---

### Unanet ERP AE

**Core features**
- Centralised project management hub (Project Central) with budget, team, contract, and client data
- DCAA-compliant timekeeping with labour distribution and audit trails
- Earned Value Management integrated with project accounting
- Resource scheduling and capacity forecasting
- CRM with pipeline and pursuit tracking
- Invoice designer with AIA-aligned billing templates
- Customisable analytics dashboards with real-time data
- Financial reporting: GL, balance sheet, P&L, and indirect rate calculations
- AI assistant ("Champ for ERP", powered by Wyatt) for natural language ERP queries

**Differentiating features**
- Purpose-built for A/E firms from the ground up, not adapted from generic ERP
- Strong DCAA compliance posture comparable to Deltek, at a more modern UX
- Agentic AI assistant with access to live ERP data for conversational reporting

**UX patterns**
- Role-based access with simplified views for project managers vs. finance staff
- Modern cloud-native interface with lower implementation burden than Deltek
- Mobile-ready with multi-device timesheet support

**Integration points**
- REST API documented at dev.portal.unanet.io; API key + subdomain authentication
- Native Mosaic integration for resource planning visualisation
- Integrations with QuickBooks, Microsoft Dynamics, and accounting platforms

**Known gaps**
- Smaller ecosystem and partner network than Deltek
- Less mature mobile app than desktop experience
- Third-party BIM/CAD integrations are limited compared to Autodesk-native tools

**Licence / IP notes**
- Proprietary commercial SaaS; pricing on application

---

### Monograph

**Core features**
- Phase-based project budgeting and live fee tracking
- MoneyGantt™: Gantt chart with live fee meter that changes colour as hours are logged
- Built-in time tracking with billable vs. non-billable hour separation
- Capacity forecasting and staffing planning across the project portfolio
- Invoicing with AIA-style billing and batch invoice generation
- Smart Inbox for invoice reminders and payment link embedding
- Margin and cash flow monitoring in real time
- QuickBooks Online integration for accounting sync
- BIM/CAD file linking to tasks and revisions

**Differentiating features**
- MoneyGantt™ is a unique visual innovation — combines schedule and financial health in one view
- Exclusively designed for architects and engineers; not a generic PM tool
- Extremely high user satisfaction (90%+) due to clean, focused UX

**UX patterns**
- Visual-first interface with colour-coded financial health indicators
- Minimal onboarding friction; designed for principals and project managers, not accountants
- Progressive disclosure hides accounting complexity behind project-centric views

**Integration points**
- QuickBooks Online (two-way sync, limited)
- API documented via API Tracker; limited public developer documentation
- No broad native integration ecosystem

**Known gaps**
- Custom reporting is limited; users want more flexible report builder
- Two-way sync with QuickBooks Online is incomplete (payments not reflected in Monograph)
- No granular task management; not suited for complex sub-task hierarchies
- Overhead and PTO tracking is basic
- Guest/contractor pricing model is inflexible — same per-seat price for 1099 staff
- No DCAA compliance features; not suitable for government contractors
- Limited integrations outside QuickBooks

**Licence / IP notes**
- Proprietary commercial SaaS
- MoneyGantt™ appears to be a proprietary branded feature; no patent found in public records

---

### BigTime

**Core features**
- Time tracking with timer and mobile entry
- All major billing models: T&M, fixed-fee, milestone, retainer in one system
- Project budgeting with variance tracking
- Resource scheduling with skills-based and capacity-based assignment
- Predictive project lifecycle management from proposal through billing
- Expense tracking with receipt capture
- Invoicing with deep QuickBooks/Sage Intacct integration
- Customisable dashboards and KPI reporting
- Embedded AI for scheduling recommendations and operational insights

**Differentiating features**
- All integrations (QuickBooks, Sage Intacct, Microsoft Dynamics, NetSuite) developed and maintained in-house
- Strong billing model flexibility within a single product
- BigTime Enterprise PSA adds portfolio-level management for larger firms

**UX patterns**
- Workflow-driven billing review and approval process
- Postman API collection published for developer self-service
- Contextual dashboards by project manager, finance, and executive roles

**Integration points**
- REST API at iq.bigtime.net/BigtimeData/api/v2; session-token authentication
- Native integrations: QuickBooks (Desktop and Online), Sage Intacct, Microsoft Dynamics GP/365, Business Central, NetSuite
- Jira integration for task-to-time-entry linking
- Rate limit: 30 API calls/minute per session token

**Known gaps**
- Not purpose-built for large multi-office engineering firms
- DCAA compliance is not a core product feature
- Reporting customisation requires configuration effort
- Mobile app trails desktop experience

**Licence / IP notes**
- Proprietary commercial SaaS; all integrations are proprietary
- Pricing from approximately $20/user/month; enterprise tier on application

---

### Productive

**Core features**
- Project budgeting supporting hourly, fixed, and mixed billing models
- Resource planning with capacity and availability forecasting
- Real-time profitability tracking including salaries and overheads (not just revenue)
- Time and expense tracking integrated with invoicing
- Financial reporting: revenue recognition, project margins, and company P&L
- Sales CRM for pipeline tracking
- Customisable task boards and project timelines
- Open API with webhooks for automation

**Differentiating features**
- Unique overhead absorption model — tracks true project profitability accounting for staff cost and company overhead
- Advanced financial forecasting with utilisation-to-revenue projections
- Clean, modern UX positioned as an agency and consultancy tool

**UX patterns**
- Unified view of resource availability, project financials, and sales pipeline
- Dashboard-first design with drill-down into individual project or person
- Designed for principals and operations managers, not dedicated finance staff

**Integration points**
- REST API following JSON:API specification at developer.productive.io
- X-Auth-Token + X-Organization-Id header authentication
- Webhooks and Open API integration listed
- Integrations with QuickBooks, Xero, Slack, and Zapier

**Known gaps**
- Not suited for DCAA/government contracting compliance
- Earned Value Management not available
- Sub-consultant and subcontract management is basic
- Limited engineering-specific features (no BIM integration, no AIA billing templates)
- Smaller customer base in A/E vs. digital agencies and IT consultancies

**Licence / IP notes**
- Proprietary commercial SaaS
- Open API JSON:API schema is documented publicly

---

### Birdview PSA

**Core features**
- End-to-end project lifecycle from sales opportunity through delivery and invoicing
- AI-powered resource allocation with skills matching and workload balancing
- Advanced project planning with tasks, milestones, dependencies (waterfall and agile)
- Financial tracking with project margin and revenue reporting
- Business intelligence with customisable dashboards
- 5,000+ integrations via Zapier and native connectors
- Time tracking linked to Jira tickets
- Template library for standardising project setup

**Differentiating features**
- Broadest integration library in the category (5,000+ via Zapier)
- Supports both waterfall and agile delivery methodologies in a single tool
- Full sales-to-delivery lifecycle without separate CRM

**UX patterns**
- Visual workload views with over/under-allocation highlighting
- Configurable templates for rapid project standup
- Role-based views from principal to project manager to resource

**Integration points**
- 1,000+ native integrations; 5,000+ via Zapier
- Jira integration for bidirectional time tracking
- REST API available; specific documentation via vendor portal

**Known gaps**
- Not engineering-specific; lacks AIA billing templates and phase-based fee management
- No DCAA compliance
- Earned Value Management not available
- BIM/CAD integration not available

**Licence / IP notes**
- Proprietary commercial SaaS

---

### Factor AE

**Core features**
- Project and phase breakdowns with task creation
- Resource scheduling and capacity planning
- Sub-consultant management and invoice pass-through
- Time and expense tracking
- Guided invoicing workflow: time entries → review → approve → send
- AIA-aligned invoice templates with firm branding customisation
- Payment link embedding for ACH/credit card collection
- Invoice reminder automation
- QuickBooks Online integration
- Industry-specific KPI tracking

**Differentiating features**
- Fully guided invoicing process unique to smaller A/E firm workflows
- Fully-assisted onboarding with no additional fee for ongoing support
- AIA invoice alignment with built-in subconsultant billing pass-through

**UX patterns**
- Wizard-style billing workflow prevents common billing errors
- Clean, navigation-friendly UI praised by small firm users
- Simple per-phase, per-task budget structure without complex accounting overhead

**Integration points**
- Native QuickBooks Online integration
- REST API availability not prominently documented; limited public developer resources

**Known gaps**
- Very small ecosystem; limited integrations beyond QuickBooks
- Not suitable for large multi-office or government-contracting firms
- No resource forecasting across portfolio
- No DCAA compliance; no earned value management
- Reporting customisation is limited

**Licence / IP notes**
- Proprietary commercial SaaS; no additional support fees
- Very small review base (10 reviews); claims 100% satisfaction

---

## Cross-Cutting Feature Themes

### Table-Stakes Features
- Time and expense tracking with mobile entry
- Phase-based project budgeting
- Flexible billing models (T&M, fixed-fee, milestone)
- Invoice generation with approval workflow
- QuickBooks or accounting system integration
- Basic resource scheduling and utilisation visibility
- Project-level profit and loss reporting
- Role-based access control

### Differentiating Features
- DCAA-compliant timekeeping and indirect cost rate management (Deltek, Unanet)
- Earned Value Management (BCWS/BCWP/ACWP) (Deltek, Unanet, Cora)
- Visual financial Gantt chart (Monograph's MoneyGantt™)
- True overhead cost absorption in profitability calculation (Productive)
- All-in-one payroll integration (BQE CORE)
- Extremely broad integration library (Birdview — 5,000+)
- AIA-aligned guided invoicing with payment links (Factor AE)
- AI-native ERP assistant for natural language data access (Unanet Champ, Deltek AI)

### Underserved Areas / Opportunities
- **AI-driven scope creep detection**: No existing tool monitors correspondence, RFI logs, and drawing revisions to automatically flag scope changes and generate change order drafts
- **Cross-portfolio earned value forecasting for mid-market**: EVM is largely confined to enterprise government contractors; mid-market A/E firms lack accessible EVM tooling
- **Natural language project status report drafting**: All tools produce data dashboards; none automatically write client-facing or internal prose status reports
- **Intelligent subconsultant compliance tracking**: Insurance certificates, deliverable milestones, and payment triggers are managed in spreadsheets outside all reviewed platforms
- **Audience-specific status communication**: PMs write the same update multiple times for different stakeholders; no platform auto-translates between technical, delivery, and executive views
- **Skill-based resource optimisation across portfolio**: Most platforms show capacity but cannot recommend optimal engineer-to-project assignments considering both availability and competency match
- **Contractor/1099 pricing flexibility**: Most platforms price 1099 contractors at the same per-seat rate as full employees, creating a barrier to engagement model diversity

### AI-Augmentation Candidates
- Automated project risk scoring from cost and schedule variance trends
- Natural language query against live project financial and schedule data
- Intelligent invoice review flagging underbilled or overbilled line items
- Scope change detection from document and email corpus
- Resource recommendation engine balancing skills, availability, and downstream project impact
- Automated client report drafting from dashboard data
- Predictive cash flow forecasting from project pipeline and billing patterns

---

## Legal & IP Summary

All reviewed products are proprietary commercial SaaS offerings with no open-source licensing. MoneyGantt™ (Monograph) is a branded feature name; no associated patent was identified in public records. Deltek's API is documented and available to vetted partners under an access agreement. BQE CORE, BigTime, Productive, and Unanet all publish public developer APIs under standard OAuth 2.0 terms. No copyright, patent, or IP concerns were identified that would restrict an open-source AI-native project from implementing equivalent features under independently developed code. The core functional patterns (phase billing, EVM calculations, time tracking, resource scheduling) are industry-standard practices not subject to any identified IP restrictions.

---

## Recommended Feature Scope

**Must-have (MVP)**
- Phase-based project budgeting with live burn-rate tracking
- Time and expense entry (web and mobile) with billable/non-billable classification
- Flexible invoicing: T&M, fixed-fee, and milestone billing with approval workflow
- Resource scheduling with capacity and utilisation visibility
- QuickBooks / Xero integration for accounting sync
- Basic project dashboard: budget vs. actual, margin, and schedule status

**Should-have (v1.1)**
- AI-assisted natural language status report drafting from project data
- Scope change detection from document and correspondence analysis
- Earned Value Management (BCWS/BCWP/ACWP) for government-contract projects
- Sub-consultant management with deliverable tracking and invoice pass-through
- Multi-project portfolio resource optimisation with downstream impact modelling
- DCAA-compliant timekeeping with indirect cost rate support

**Nice-to-have (backlog)**
- Automated audience-specific status update generation (technical / client / executive)
- Insurance certificate and compliance document tracking for subconsultants
- BIM/CAD file revision linking to project tasks and budget phases
- Predictive cash flow forecasting from pipeline and billing pattern analysis
- AIA-aligned invoice templates with payment link embedding
- 1099/contractor access tier with reduced per-seat pricing
