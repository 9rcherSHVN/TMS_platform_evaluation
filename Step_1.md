Yes. Before I build the runbook, I would not start with vendor scoring yet.

As a solution architect, the biggest mistake I see organizations make is:

"Compare MercuryGate vs IntelliTrans vs project44 vs Descartes" before they fully understand what business problem they are trying to solve.

In reality, a TMS selection project is typically 70% business operating model assessment and only 30% software evaluation.

What Are We Actually Trying To Accomplish?

First, we need to define which of these scenarios applies:

Scenario A - TMS Replacement

You already have a TMS.

Examples:

IntelliTrans / CarrierPoint
MercuryGate
Oracle Transportation Management (OTM)
SAP TM
Descartes
Blue Yonder

Goal:

Replace existing TMS because of limitations, cost, technical debt, poor adoption, lack of functionality, poor integrations, etc.

Scenario B - First-Time TMS Implementation

No centralized TMS exists.

Current landscape:

ERP
spreadsheets
carrier portals
emails
manual freight tendering

Goal:

Standardize transportation planning, execution, visibility, and freight settlement.

Scenario C - TMS Transformation

Keep existing TMS but significantly expand functionality.

Examples:

Add real-time visibility
Add carrier onboarding
Add freight audit/pay
Add appointment scheduling
Add dock management
Add AI optimization
What I Need From You

To produce a high-quality executive-level and architecture-level runbook, I would need answers to the following questions.

1. Business Model

This is the most important section.

What industry?

Examples:

Forest Products (Interfor-like)
Manufacturing
Automotive
Retail
Food & Beverage
Mining
Agriculture
Chemical
Oil & Gas
What do you ship?

Examples:

Lumber
Pallets
Finished goods
Containers
Bulk products
Hazardous materials
Typical shipment modes?
Truckload (TL)
Less Than Truckload (LTL)
Rail
Intermodal
Ocean
Parcel
Air
Geographic footprint?
Canada
US
Mexico
Global
2. Transportation Volume

Vendors differ dramatically based on volume.

Examples:

Annual Shipments
5,000
50,000
500,000
5 million
Annual Freight Spend
$5M
$50M
$500M
$5B
3. Business Drivers

Why are we doing this?

Rank these:

Driver	PriorityFreight Cost Reduction	?
Carrier Compliance	?
Visibility / Tracking	?
Customer Service	?
Rail Management	?
Carrier Procurement	?
Freight Payment	?
Digital Transformation	?
Legacy Replacement	?
4. Current-State Assessment

For replacement projects:

What system today?

Examples:

IntelliTrans CarrierPoint
MercuryGate
Oracle OTM
SAP TM
Current pain points?

Examples:

poor UI
lack of APIs
difficult reporting
expensive licenses
weak optimization
weak rail support
limited integrations
5. Transportation Operating Model

This is where many TMS projects fail.

Centralized dispatch?

or

Mill/Plant-level dispatch?

For example, in a forest products company:

each mill dispatches independently

vs

centralized logistics team

Result: different TMS requirements.

6. Carrier Model
Dedicated Carriers?
Spot Market?
Contract Carriers?
Broker-heavy?
Mix?

This heavily influences vendor selection.

7. Visibility Expectations

How important are:

Real-time tracking?

Providers:

project44
FourKites
Descartes MacroPoint
Estimated Time of Arrival?
Geofencing?
POD capture?
Event management?
8. Financial Requirements

Many executives underestimate this area.

Need to know:

Freight Audit

Required?

Freight Settlement

Required?

Self-billing / Auto-pay

Required?

Carrier Invoicing

Required?

Accruals

Required?

GL Integration

Required?

Your current Interfor environment already shows freight self-billing and TMS-ready-to-pay concepts tied into freight settlement processes. Those types of capabilities can become major vendor selection criteria.

9. ERP Landscape

Critical question.

What must TMS integrate with?

Examples:

Oracle Fusion ERP
SAP S/4HANA
Dynamics 365
Epicor
JD Edwards

Required integrations?

Examples:

Orders
Shipments
Inventory
Vendors
Freight Charges
Invoices
AP
AR
10. Architecture Strategy

What is the desired architecture?

Examples:

Cloud SaaS First
Best-of-Breed
ERP-Centric
API-First
Integration Platform

Examples:

OIC
MuleSoft
Boomi
Informatica IICS
Azure Integration Services
11. Future State Vision

Where should the organization be in 5 years?

Examples:

AI-assisted carrier selection
Dynamic routing
Transportation control tower
Carbon emissions tracking
Autonomous carrier tendering
Supplier collaboration portal
Real-time supply chain visibility
My Recommended Deliverables

Once you answer the above, I would build a complete TMS Selection Runbook containing:

Executive Evaluation Framework
Current-State Assessment Methodology
Transportation Process Assessment
Functional Requirements Matrix
Technical Architecture Assessment
Integration Assessment Framework
Vendor Shortlisting Methodology
RFP/RFI Strategy
Scoring Model (Weighted)
TCO & ROI Model
Proof-of-Concept Methodology
Implementation Risk Assessment
Migration Strategy
Executive Decision Matrix
Final Vendor Recommendation Framework

My first question:

Is this assessment intended for a specific company (for example, Interfor and the current IntelliTrans/CarrierPoint ecosystem), or should I build a vendor-neutral TMS selection runbook that could be used by any transportation-intensive enterprise?

That answer will significantly change the depth, examples, scoring criteria, and vendor recommendations.
