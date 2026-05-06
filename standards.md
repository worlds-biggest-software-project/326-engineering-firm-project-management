# Standards & API Reference

> Project: Engineering Firm Project Management · Generated: 2026-05-03

## Industry Standards & Specifications

### ISO Standards

**ISO 21502:2020 — Project, Programme and Portfolio Management: Guidance on Project Management**
- URL: https://www.iso.org/standard/74947.html
- The successor to ISO 21500:2012, this standard defines 111 processes across all phases of a project lifecycle. Applicable to any organisation size or sector, it provides the international baseline for project management methodology that engineering firms and their software tools are expected to align with. Software implementing project workflows should support the process groups and subject groups defined here.

**ISO 21500:2021 — Project, Programme and Portfolio Management: Context and Concepts**
- URL: https://www.iso.org/standard/75704.html
- Updated in 2021 to become the context and concepts layer of the ISO 21500 family. Defines the governance and environmental framework within which project management operates. Relevant for multi-project portfolio management features and organisational governance structures in engineering firm software.

**ISO 21503:2022 — Guidance on Programme Management**
- URL: https://www.iso.org/standard/75705.html
- Covers the management of interdependent projects and activities as a programme to deliver benefits. Relevant to portfolio-level features in engineering project management platforms where multiple related projects must be managed as a coordinated programme.

**ISO 21504:2015 — Guidance on Portfolio Management**
- URL: https://www.iso.org/standard/56654.html
- Provides guidance for managing a portfolio of projects and programmes within an organisation. Directly relevant to portfolio-level resource planning, financial forecasting, and reporting features for mid-to-large engineering firms.

**ISO 9001:2015 — Quality Management Systems: Requirements**
- URL: https://www.iso.org/standard/62085.html
- The world's most adopted quality management standard; widely required for engineering consultancies. Software must support document control, process traceability, non-conformance tracking, and audit readiness to enable certified firms to demonstrate compliance.

**ISO 19650-1:2018 — Organisation and Digitisation of Information about Buildings and Civil Engineering Works (BIM) — Part 1: Concepts and Principles**
- URL: https://www.iso.org/standard/68078.html
- International standard for BIM information management across the full built-asset lifecycle. The Common Data Environment (CDE) concept defined here is a prerequisite for engineering project management tools that handle deliverable coordination and document management alongside project financials.

**ISO 19650-2:2018 — BIM Information Management: Delivery Phase of the Assets**
- URL: https://www.iso.org/standard/68080.html
- Specifies requirements for information management during the design and construction phase. Engineering project management software that integrates with BIM workflows must align with the information container naming conventions, revision states, and approval workflows defined in this part.

---

### W3C & IETF Standards

**RFC 5545 — Internet Calendaring and Scheduling Core Object Specification (iCalendar)**
- URL: https://datatracker.ietf.org/doc/html/rfc5545
- Defines the .ics data format for exchanging calendar events, to-dos, and scheduling information. Engineering project management tools that export project milestones, resource bookings, or deadlines to calendar applications (Outlook, Google Calendar, Apple Calendar) must produce RFC 5545-compliant output.

**RFC 6749 — The OAuth 2.0 Authorization Framework**
- URL: https://datatracker.ietf.org/doc/html/rfc6749
- The authorisation standard underpinning all reviewed engineering project management APIs (Deltek, BQE CORE, BigTime, Productive, Unanet). Any API exposing project, financial, or resource data to third-party integrations must implement OAuth 2.0 compliant flows.

**RFC 7231 — Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content**
- URL: https://datatracker.ietf.org/doc/html/rfc7231
- Baseline HTTP semantics standard that all REST APIs in this space rely upon. Relevant for designing resource-oriented API endpoints for projects, timesheets, invoices, and resources.

**RFC 7807 — Problem Details for HTTP APIs**
- URL: https://datatracker.ietf.org/doc/html/rfc7807
- Standard format for machine-readable error responses in HTTP APIs. Recommended for engineering PM API error responses to enable integrators to handle errors programmatically.

**JSON:API Specification**
- URL: https://jsonapi.org/format/
- A widely adopted convention for building JSON REST APIs with standardised resource relationships, filtering, sorting, and pagination. Productive.io's API is documented as JSON:API-compliant; an AI-native engineering PM product should consider adopting this for consistency with ecosystem tools.

---

### Data Model & API Specifications

**OpenAPI Specification 3.1**
- URL: https://spec.openapis.org/oas/v3.1.0
- The de facto standard for documenting REST APIs in machine-readable YAML/JSON. All major engineering PM vendors (Deltek, BQE CORE, BigTime) publish or reference OpenAPI-compliant documentation. An AI-native product should publish an OpenAPI 3.1 spec to enable MCP server generation, client SDK auto-generation, and Postman collection publishing.

**ANSI/EIA-748-C — Earned Value Management Systems (EVMS)**
- URL: https://www.sae.org/standards/eia748d-earned-value-management-systems
- The US national standard defining 32 guidelines for an EVMS. Any engineering project management tool targeting US government contractors must calculate and report BCWS (Budgeted Cost of Work Scheduled), BCWP (Budgeted Cost of Work Performed), and ACWP (Actual Cost of Work Performed) in compliance with these guidelines. Maintained by NDIA/SAE International and reviewed every five years.

**PMI PMBOK Guide — 7th Edition (2021)**
- URL: https://www.pmi.org/standards/pmbok
- PMI's flagship standard defining 12 project management principles and 8 project performance domains. Engineering firms commonly require software to support PMI-aligned terminology and process groupings. The 7th edition shift to principles-based guidance (vs. process-based) means software must support multiple delivery approaches (predictive, agile, hybrid).

---

### Security & Authentication Standards

**OAuth 2.0 (RFC 6749) and OpenID Connect**
- URL: https://openid.net/connect/
- All reviewed engineering PM APIs use OAuth 2.0 for authorisation; OpenID Connect adds identity layer for single sign-on. Required for enterprise integrations with Microsoft 365, Google Workspace, and corporate identity providers common in engineering firms.

**OWASP API Security Top 10**
- URL: https://owasp.org/www-project-api-security/
- The OWASP API Security Top 10 defines the most critical API vulnerabilities. Engineering PM platforms handle sensitive financial and project data (contract values, government project details) and must be designed to address broken object-level authorisation, broken authentication, excessive data exposure, and rate limiting failures.

**NIST SP 800-171 — Protecting Controlled Unclassified Information in Non-Federal Systems**
- URL: https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final
- Applicable to engineering firms working on US government contracts. CUI (Controlled Unclassified Information) handling requirements in NIST SP 800-171 and the associated CMMC (Cybersecurity Maturity Model Certification) framework impose data handling, access control, and audit logging requirements on project management software used in these environments.

**FAR (Federal Acquisition Regulations) / DCAA Compliance**
- URL: https://www.acquisition.gov/browse/index/far
- Federal Acquisition Regulations and Defense Contract Audit Agency (DCAA) requirements govern how engineering firms with US federal contracts structure their accounting systems, timekeeping, and indirect cost rates. Software must support compliant general ledger structure, timekeeping with supervisor approval, and indirect cost pool reporting to pass DCAA floor checks and audits.

---

### MCP Server Specifications

**Model Context Protocol (MCP)**
- URL: https://modelcontextprotocol.io/introduction
- Anthropic's open protocol for connecting AI assistants to data sources and tools via standardised server definitions. An AI-native engineering PM product should expose an MCP server enabling AI assistants (Claude, Cursor, etc.) to query project status, financial data, resource availability, and generate reports through natural language — providing the "AI-native" differentiation absent from all reviewed incumbents. The OpenAPI 3.1 spec should be used as the basis for MCP tool definitions.

---

## Similar Products — Developer Documentation & APIs

### Deltek Vantagepoint
- **Description:** Enterprise ERP for A&E and government contracting firms; industry-standard for DCAA compliance and EVM. Covers CRM, project accounting, resource planning, and financial management.
- **API Documentation:** https://vantagepointapi.deltek.com/ (current version) and https://help.deltek.com/Product/Vantagepoint/5.0/DPS_REST_API.html
- **SDKs/Libraries:** No official SDKs published; REST API with JSON responses; Postman-compatible
- **Developer Guide:** https://learning.deltek.com/category/vantagepoint_api_guides and https://www.deltek.com/en/learn/developer-resources
- **Standards:** REST/JSON, OAuth 2.0; OpenAPI-referenced documentation
- **Authentication:** OAuth 2.0; vetted partner access agreement required for API credentials

### BQE CORE
- **Description:** Integrated practice management for A&E and professional services firms. Covers project management, billing, time/expense, payroll, and accounting in a single SaaS product.
- **API Documentation:** https://api-explorer.bqecore.com/
- **SDKs/Libraries:** Code samples in ASP.NET MVC, Java, PHP, Angular, iOS — available via developer portal
- **Developer Guide:** https://corehelpcenter.bqe.com/hc/en-us/articles/1500008338801-How-to-get-started-with-BQE-CORE-APIs and https://api-developer.bqecore.com/
- **Standards:** REST/JSON; OAuth 2.0
- **Authentication:** OAuth 2.0 with clientId/clientSecret; token-based access

### Unanet ERP AE
- **Description:** Cloud ERP purpose-built for architecture and engineering firms; strong DCAA compliance and integrated analytics. Covers project management, resource planning, CRM, financials, and time/expense.
- **API Documentation:** https://dev.portal.unanet.io/
- **SDKs/Libraries:** No official SDKs; REST API with JSON
- **Developer Guide:** https://dev.portal.unanet.io/platform/swagger/ (Swagger UI) and https://help.unanet.com/current/unanet_menu/admin/integration.htm
- **Standards:** REST/JSON, OpenAPI (Swagger); Basic auth or API key depending on endpoint
- **Authentication:** API key + firm access code; Basic auth on some endpoints

### BigTime
- **Description:** PSA platform for professional services including engineering; strong billing model flexibility and in-house-maintained accounting integrations (QuickBooks, Sage, NetSuite, Dynamics).
- **API Documentation:** https://iq.bigtime.net/BigtimeData/api/v2/Help/Overview
- **SDKs/Libraries:** Postman collection — https://www.postman.com/bigtime-restful; no official language SDKs
- **Developer Guide:** https://help.bigtime.net/hc/en-us/articles/10565842022423-Getting-Started-With-BigTime-s-API and https://kb.bigtime.net/bigtime-configuration/integration-guide/getting-started-with-bigtimes-api/
- **Standards:** REST; supports XML and JSON via Content-Type header negotiation
- **Authentication:** Session token — POST credentials to /session/firm to obtain a token; 30 API calls/minute rate limit

### Productive
- **Description:** Agency and professional services PSA with strong overhead cost absorption and profitability tracking; growing adoption among engineering consultancies.
- **API Documentation:** https://developer.productive.io/reference
- **SDKs/Libraries:** No official SDKs; JSON:API-compliant REST; Pipedream connector available
- **Developer Guide:** https://developer.productive.io/ and https://productive.io/integrations/open-api/
- **Standards:** JSON:API specification; REST/JSON
- **Authentication:** X-Auth-Token header + X-Organization-Id header; token obtained via account settings

### Monograph
- **Description:** Project management for architecture and engineering firms; known for MoneyGantt™ visual fee tracking and clean UX targeting small-to-mid practices.
- **API Documentation:** https://apitracker.io/a/monograph-io (third-party tracker; official docs not publicly prominent)
- **SDKs/Libraries:** Not publicly documented
- **Developer Guide:** Limited public developer documentation; QuickBooks Online integration is the primary documented integration path
- **Standards:** REST/JSON (inferred); integration details not publicly published
- **Authentication:** Not publicly documented

### Factor AE
- **Description:** Affordable project management for small A/E firms; AIA-aligned invoicing with guided billing workflow and sub-consultant management.
- **API Documentation:** Not prominently published
- **SDKs/Libraries:** Not publicly available
- **Developer Guide:** QuickBooks Online integration documented via help centre; no public developer API guide found
- **Standards:** Not publicly documented
- **Authentication:** Not publicly documented

---

## Notes

**Earned Value Management data models**: The EIA-748-C standard defines the functional requirements for EVMS but does not specify a data exchange format. No universal open schema exists for EVM data interchange; most implementations use proprietary data models. An AI-native product has an opportunity to define and publish an open EVM data schema (e.g., as JSON Schema or OpenAPI components) that could become a community standard.

**BIM integration gap**: ISO 19650 defines information management requirements but does not specify a project management API interface. The Common Data Environment (CDE) platforms (Autodesk Construction Cloud, Trimble Connect, Aconex) each have proprietary APIs; no open standard governs how project management and BIM platforms exchange cost and schedule data. This is an underserved interoperability gap.

**MCP opportunity**: None of the reviewed products currently expose an MCP server. An AI-native engineering PM platform that publishes an MCP server alongside its REST API would be uniquely positioned to integrate into AI assistant workflows, enabling project managers to query financial status, generate reports, and manage resources through natural language without building custom integrations.

**FIDIC and AIA contract alignment**: FIDIC contract forms (international) and AIA document series (US) define milestone billing triggers and deliverable acceptance processes widely used by engineering firms. No reviewed product embeds FIDIC or AIA contract templates as structured data; they are handled as file attachments. Structuring contract terms as machine-readable data would enable AI-assisted billing trigger detection and change order management.
