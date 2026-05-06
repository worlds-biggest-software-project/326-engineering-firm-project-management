# Engineering Firm Project Management

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source project management platform purpose-built for engineering firms — combining project accounting, resource planning, and deliverable tracking.

Engineering Firm Project Management is a candidate platform for architecture and engineering (A/E) consultancies that need integrated phase-based budgeting, flexible billing, resource scheduling, and deliverable coordination. It targets the gap between heavy enterprise ERPs and lightweight task trackers, bringing AI-driven forecasting and reporting to firms that today rely on spreadsheets or expensive incumbents.

---

## Why Engineering Firm Project Management?

- Enterprise incumbents like Deltek Vantagepoint require $50,000+ annual commitments and complex implementations described as "built for accountants," with cumbersome reporting and a steep learning curve for non-finance users.
- Mid-market tools (BQE CORE, BigTime, Productive) lack DCAA compliance and Earned Value Management, locking out government-contracting engineering firms from accessible options.
- Purpose-built A/E tools like Monograph and Factor AE deliver clean UX but have limited accounting depth, no DCAA support, and small integration ecosystems.
- Generic platforms (Microsoft Project, Wrike, Birdview) offer scheduling and automation but lack engineering-specific features such as AIA-aligned billing, phase-based fee management, and subconsultant pass-through.
- Across all reviewed tools, no platform offers AI-driven scope creep detection, natural language status report drafting, or intelligent subconsultant compliance tracking — these remain spreadsheet-managed gaps.

---

## Key Features

### Project Budgeting and Billing

- Phase-based project budgeting with live burn-rate tracking
- Flexible billing models: T&M, fixed-fee, milestone, retainer, and percentage-complete
- AIA-aligned invoice templates with payment link embedding
- Approval workflow with billing review before invoice send
- Subconsultant management with deliverable tracking and invoice pass-through

### Time, Expense, and Resource Management

- Web and mobile time and expense entry with billable / non-billable classification
- Resource scheduling with capacity and utilisation visibility
- Skills-based and capacity-based assignment recommendations
- Multi-project portfolio resource optimisation with downstream impact modelling
- Real-time profitability tracking including salaries and overheads

### Compliance and Government Contracting

- DCAA-compliant timekeeping with labour distribution and audit trails
- Indirect cost rate structures for federal contract reporting
- Earned Value Management with BCWS, BCWP, and ACWP calculations
- ISO 9001 and ISO 19650-aligned document control hooks
- FAR-aware reporting structures for government contractors

### Reporting and Analytics

- Project dashboards: budget vs. actual, margin, schedule status
- Real-time project health with profitability and margin tracking
- Cash flow forecasting from pipeline and billing patterns
- KPI dashboards for principals, project managers, and finance roles
- Customisable role-based views

### AI-Native Capabilities

- AI-driven earned value forecasting predicting cost-at-completion and schedule-at-completion
- Natural language status report drafting for client and internal audiences
- Scope change detection from correspondence, RFI logs, and drawing revisions
- Intelligent resource allocation matching skill profiles and availability across the portfolio
- Automated subconsultant compliance tracking covering deliverable milestones, payment triggers, and insurance certificate expiry

---

## AI-Native Advantage

Existing AI features in incumbents (Deltek's Vantagepoint AI, Unanet's Champ assistant) are limited to natural language queries against ERP data and have received mixed reviews for inconsistency. This project goes further: predictive earned value forecasting that surfaces likely overruns weeks before traditional reporting, scope creep detection from project document corpora, automated client-facing status report drafting, and skill-aware portfolio resource optimisation. These capabilities are absent from every reviewed platform and address documented spreadsheet workflows in subconsultant compliance and audience-specific status communication.

---

## Tech Stack & Deployment

The platform is intended as a cloud-native SaaS with self-hosted options for firms requiring on-premise deployment for DCAA audit posture. Integrations target QuickBooks (Online and Desktop), Xero, and Sage Intacct for accounting sync, with Jira linkage for engineering task workflows. APIs follow REST patterns aligned with the conventions used by Unanet, BQE CORE, and Productive (OAuth 2.0 or token-based authentication, JSON:API-style schemas where appropriate). Mobile-first time and expense entry is a baseline expectation.

---

## Market Context

The global project management software market is valued at USD 9.6–11.3 billion in 2026, growing at 13–15% CAGR toward USD 23–39 billion by 2031–2035 (Mordor Intelligence; Grand View Research; Business Research Insights). The A/E segment is dominated by Deltek's installed base of 12,000+ firms, with enterprise pricing at $50,000+ annually for mid-size firms and mid-market tools at $20–$50/user/month. Primary buyers include small civil and structural consultancies, mid-size multi-discipline engineering firms, large government-contracting firms, and infrastructure project management offices.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.
