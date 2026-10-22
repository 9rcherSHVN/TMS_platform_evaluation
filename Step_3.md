Use two capability tracks for truck and rail; I would like to see the proposed 360-degree assessment framework first;


Excellent. I actually agree with separating Truck and Rail.

One of the biggest mistakes in TMS evaluations is treating Rail as just another transportation mode. In reality:

Truck TMS vendors tend to optimize around tendering, carrier networks, pricing, visibility, appointment scheduling, POD, and freight settlement.
Rail operations introduce completely different business processes:
waybills
railcar lifecycle management
demurrage
rail routing
interchange
rail equipment utilization
railroad EDI
customs
car tracing
fleet management

For Interfor, Truck and Rail should be assessed as separate capability domains before deciding whether a single platform or multi-platform architecture is optimal.

Proposed 360° TMS Assessment Framework
Guiding Principle

The framework should answer:

"If Interfor were building its transportation technology landscape today, knowing everything we know now, would we still choose the same architecture?"

Notice:

NOT "Do we like CarrierPoint?"
NOT "Who has the prettiest UI?"
NOT "Which vendor has the biggest marketing budget?"

Instead:

Which transportation architecture best supports Interfor's business model over the next 5-10 years?

Assessment Layer 1 - Business Strategy Fit

Weight: 15%

Executive Audience: VP Supply Chain Director Logistics VP Operations CIO

Questions
Does the platform support:
Growth
Acquisitions
New mills
New regions
New carriers
New transportation modes
Strategic Alignment

Can platform support:

Canada
USA
Mexico
International expansion

without major redesign?

Future Readiness

Can it support:

AI optimization
Predictive ETA
Carbon reporting
Transportation Control Tower
Real-time visibility
Assessment Layer 2 - Transportation Functional Fit

Weight: 25%

This becomes the largest scoring category.

Track A - Truck Operations
Transportation Planning

Capability Areas:

Load planning
Consolidation
Multi-stop routing
Optimization
Capacity planning
Dynamic routing
Carrier Management

Capability Areas:

Carrier onboarding
Insurance tracking
Carrier qualification

Interfor currently maintains carrier-related synchronization activities through OMSI/CarrierPoint integrations and onboarding processes.

Tendering

Capability Areas:

Automated tendering
Spot bids
Mini-bids
Contract rates
Carrier ranking
Visibility

Capability Areas:

GPS visibility
Geofencing
Event management
ETA prediction
Exception management
Dock & Appointment

Capability Areas:

Appointment scheduling
Yard visibility
Dock planning
POD & Documentation

Capability Areas:

Electronic POD
Mobile POD
Image capture
Workflow approvals
Track B - Rail Operations

This is evaluated separately.

Rail Planning

Capability Areas:

Railcar assignment
Multi-railroad routing
Rate management
Capacity planning
Rail Execution

Capability Areas:

EDI 404
Waybill support
Rail event tracking

Interfor currently operates processes involving rail bill of lading and EDI 404 integrations.

Railroad Connectivity

Capability Areas:

CN
CPKC
BNSF
UP
CSX
Rail Fleet Management

Capability Areas:

Railcar lifecycle
Railcar utilization
Fleet tracking
Empty-car management
Demurrage Management

Capability Areas:

Detention
Storage
Demurrage analytics
Assessment Layer 3 - Financial & Audit Controls

Weight: 15%

For Interfor this becomes a critical category.

Recent Interfor discussions identified freight settlement, Ready-to-Pay processing, delivery-confirmation dates, self-generated invoices, audit controls, legal-entity billing, tax compliance concerns and carrier payment workflows.

Freight Settlement

Evaluate:

Audit capability
Charge validation
Exception resolution
Freight Payment

Evaluate:

AP integration
Self-billing
Auto-payment

Current AUTO-FAVI processes already rely on automated freight-related invoice generation and payment orchestration.

Tax & Compliance

Evaluate:

GST/HST
Cross-border
Legal entities
Audit traceability
Financial Integration

Evaluate:

Oracle integration
Posting controls
Accrual processing
Assessment Layer 4 - Technical Architecture

Weight: 15%

Audience:

Architecture
Integration
IT Operations
Integration Architecture

Evaluate:

REST APIs
Event architecture
EDI
Batch interfaces

Current evidence shows Interfor operates a mixed environment involving APIs, OMSI integration, SSIS processes, EDI transactions, and batch/event-driven synchronization.

Data Architecture

Evaluate:

Master data ownership
Data model extensibility
Custom attributes
Platform Architecture

Evaluate:

SaaS maturity
Scalability
Multi-tenant architecture
Security

Evaluate:

SSO
MFA
SOC reports

Interfor maintains both SOC 1 Type 2 and SOC 2 Type 2 reports for IntelliTrans.

Assessment Layer 5 - Operational Excellence

Weight: 10%

This area is frequently overlooked.

Environment Management

Evaluate:

Production
UAT
Sandbox
DR

Interfor documentation references production, testing and UAT environments, environment refreshes, OMSI environment configuration and backup UAT instances.

Monitoring

Evaluate:

Interface monitoring
Alerting
SLA tracking
Recoverability

Evaluate:

Replay
Resubmission
Reconciliation

Operational incidents and synchronization discussions indicate this should be explicitly assessed.

Release Management

Evaluate:

Vendor release cadence
Backward compatibility
Regression testing effort
Assessment Layer 6 - Vendor Assessment

Weight: 10%

Vendor Viability

Evaluate:

Revenue
Market share
Financial stability
Industry Focus

Evaluate:

Forest products
Manufacturing
Distribution
Product Roadmap

Evaluate:

AI investments
Visibility strategy
Transportation Control Tower direction
Customer Success

Evaluate:

Support model
Escalation process
Account management
Assessment Layer 7 - Total Cost of Ownership

Weight: 10%

Evaluate:

Direct Costs
Licenses
Transactions
Carriers
Visibility subscriptions
Indirect Costs
Integrations
Support
Upgrades
Testing
Replacement Costs

Evaluate:

Data migration
Carrier onboarding
Retraining
Change management
Assessment Layer 8 - Transformation Risk

Weight: Pass / Fail Gate

This scoring is independent.

Questions:

Can Interfor safely migrate?
Can carriers onboard?
Can rail operations migrate?
Can finance reconcile?
Can historical auditability be preserved?
Vendor Evaluation Structure

I recommend the following evaluation model.

Wave 1 (Long List)

10-15 vendors

Purpose:

Remove obvious non-fits.

Wave 2 (Short List)

4-6 vendors

Deep technical assessment.

Wave 3 (Scenario Validation)

2-3 vendors

Execute real Interfor scenarios.

Not demos.

Actual scenarios.

Examples:

Scenario #1

Truckload shipment

LumberTrack → TMS → Carrier → POD → Settlement

Scenario #2

Rail shipment

Order → Rail Assignment → EDI 404 → Waybill → Delivery

Scenario #3

Cross-border shipment

Canada → USA

Scenario #4

Ready-to-Pay

Carrier POD → Freight Settlement → Oracle Payment

Reflecting processes already discussed within Interfor.

Most Important Principle

Do not compare vendors feature-by-feature.

Instead compare them using:

"Can this vendor successfully execute Interfor transportation business scenarios with acceptable risk, complexity and operating cost?"

That distinction completely changes the quality of the assessment.

My recommendation for the next step would be to define the TMS capability model (approximately 150-250 capabilities) grouped into Truck, Rail, Financial, Integration, Operations, Security, Analytics, and Vendor domains. That capability model becomes the foundation for all scoring, RFP questions, demonstrations, and proof-of-concept activities.
