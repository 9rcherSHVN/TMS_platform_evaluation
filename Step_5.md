Proceed with the initial runbook assumptions.

Interfor TMS Modernization & Replacement Program
Phase 1: 360-Degree Transportation Platform Assessment Runbook
Executive Objective

Establish whether Interfor should:

Retain CarrierPoint unchanged
Modernize CarrierPoint
Augment CarrierPoint with specialized platforms
Replace selected capabilities
Replace CarrierPoint entirely
Adopt a composable transportation architecture

This assessment is intentionally vendor-neutral and uses CarrierPoint as the incumbent baseline, not the preferred outcome.

Current Interfor documentation confirms CarrierPoint's role in transportation planning, carrier assignment, shipment execution, billing workflows, and LumberTrack integrations. Existing evidence also highlights integration complexity involving OMSI, SSIS, EDI processes, Ready-to-Pay workflows, POD handling, freight settlement, and audit-related controls.

Program Guiding Principles
Principle 1

Do not evaluate products.

Evaluate business outcomes.

Bad question:

Can Vendor X do carrier tendering?

Better question:

Can Vendor X execute Interfor's complete transportation lifecycle with acceptable risk?

Principle 2

Separate current problems into categories:

Category	ExampleProduct Limitation	Missing rail function
Configuration	Misconfigured workflow
Integration	OMSI synchronization issue
Data Quality	Invalid carrier data
Process	Manual workaround
User Adoption	Users bypass process
Vendor Support	Escalation delays
Governance	Undefined ownership

Several historical issues found in Interfor records appear to involve synchronization, date handling, OMSI processing, resubmission procedures, and operational workflows. These must be root-caused before they are classified as product deficiencies.

Assessment Phase Structure
Phase	ObjectivePhase 1	Current State Baseline
Phase 2	Truck Capability Assessment
Phase 3	Rail Capability Assessment
Phase 4	Financial & Compliance Assessment
Phase 5	Technical Architecture Assessment
Phase 6	Operational Excellence Assessment
Phase 7	Market Scan
Phase 8	Vendor Shortlisting
Phase 9	Scenario Validation
Phase 10	Executive Recommendation
Phase 1
Current State Baseline Assessment
Deliverables
Business Architecture

Document:

Transportation operating model
Logistics organization
Dispatch model
Mill responsibilities
Regional differences
Process Architecture

Map:

Order to Shipment
Shipment Planning
Tendering
Carrier Acceptance
Execution
POD
Freight Settlement
AP Payment

Current LumberTrack and CarrierPoint process documentation already provides the starting baseline for transportation planning and shipment lifecycle mapping.

Application Architecture

Identify:

System	RoleLumberTrack	Transportation source system
CarrierPoint	Transportation execution
OMSI	Integration framework
Oracle	Financial processing
Informatica	B2B/File movement
Kleinschmidt	Rail connectivity

Elements of this landscape appear in existing Interfor documentation and integration inventories.

Interface Inventory

Document:

APIs
OMSI feeds
SSIS jobs
EDI transactions
File transfers
Scheduled processes
Manual touchpoints
Phase 2
Truck Capability Assessment

The complete Truck Capability Model previously defined becomes the evaluation framework.

Key Evaluation Domains
Transportation Planning

Questions:

Can planners build optimal truck plans?
How much manual intervention exists?
How much automation exists?
Carrier Management

Questions:

Carrier onboarding effort?
Insurance management?
Performance management?

Carrier data synchronization and insurance-related integrations are already known operating concerns.

Tendering

Questions:

Contract tendering
Spot tendering
Capacity management
Market responsiveness
Visibility

Questions:

Real-time status?
POD acquisition?
ETA quality?
Exception management?
Freight Settlement

Questions:

Invoice matching?
Accruals?
Ready-to-Pay workflow?
Self-billing?

Current AUTO-FAVI and Ready-to-Pay design should become benchmark scenarios.

Phase 3
Rail Capability Assessment

Conduct separately from Truck.

Evaluate
Rail Planning
Car allocation
Empty car management
Route selection
Railroad Connectivity
Waybill creation
EDI 404
Acknowledgements
Exception recovery

Interfor's documented EDI 404 process and waybill-return workflow should become mandatory test scenarios.

Rail Visibility
Car tracing
Interchange visibility
Dwell management
Demurrage
Prevention
Monitoring
Analytics
Rail Financials
Invoice validation
Cost allocation
Audit support
Phase 4
Financial, Compliance & Audit Assessment

This should carry unusually high weight for Interfor.

Reason:

Internal evidence already identifies:

invoice dating concerns
tax compliance concerns
legal entity concerns
billing accuracy concerns
audit recommendations
Domains
Freight Audit

Evaluate:

automated validation
dispute handling
duplicate prevention
Settlement

Evaluate:

self-billing
carrier invoicing
AP integration
Tax

Evaluate:

GST
HST
QST
USA requirements
Legal Entity Management

Evaluate:

billing entity assignment
regional entity support
audit traceability
Phase 5
Technical Architecture Assessment

Audience:

Solution Architects
Integration Architects
Enterprise Architects
Integration

Assess:

Current State
OMSI
SSIS
APIs
EDI
Future State
Event-driven architecture
API-first architecture
SaaS integrations
Data streaming
Data Architecture

Assess:

ownership
source systems
synchronization model
master data
Extensibility

Assess:

workflow engine
low-code configuration
custom fields
APIs
Security

Assess:

SSO
MFA
RBAC
Audit

CarrierPoint currently supports enterprise SSO and associated user/location security administration.

Phase 6
Operational Excellence Assessment

This phase frequently exposes hidden TCO.

Environment Management

Review:

Production
UAT
Test
DR

Interfor's environment-management processes and refresh procedures demonstrate that this must be evaluated explicitly.

Supportability

Measure:

Incident response
Monitoring
Alerting
Escalation
Recoverability

Measure:

Replay
Resubmission
Reconciliation

Interfor has historical examples involving shipment synchronization, OMSI processing, retransmission and reconciliation activities.

Phase 7
Market Scan

Create vendor archetypes.

Group 1

Enterprise Multimode

Examples:

Oracle Transportation Management
SAP Transportation Management
Blue Yonder
Group 2

Transportation Specialists

Examples:

MercuryGate
Descartes
IntelliTrans
Group 3

Visibility Platforms

Examples:

project44
FourKites
Group 4

Composable Transportation Platforms

Examples:

Combination solutions
API-first architectures
Best-of-breed ecosystems
Phase 8
Vendor Shortlisting

Recommended approach

Long List

10-15 vendors

Score:

Truck fit
Rail fit
Architecture fit
Financial fit
Short List

4-6 vendors

Perform:

demonstrations
architecture reviews
integration reviews
Finalists

2-3 vendors

Move to scenario testing.

Phase 9
Interfor Scenario Validation

This is the most important phase.

No PowerPoint scoring.

No marketing scoring.

Execute real Interfor scenarios.

Scenario 1

Truck Order Lifecycle

LumberTrack
   ↓
Shipment
   ↓
Planning
   ↓
Tender
   ↓
Carrier Acceptance
   ↓
Execution
   ↓
POD
   ↓
Ready To Pay
   ↓
Settlement

Scenario 2

Cross-Border Shipment

Canada
   ↓
USA
   ↓
Customs Validation
   ↓
Execution
   ↓
Delivery

Scenario 3

Rail Lifecycle

Order
   ↓
Rail Planning
   ↓
Car Assignment
   ↓
EDI 404
   ↓
Waybill
   ↓
Tracing
   ↓
Delivery


Current Interfor rail processes provide a concrete baseline for this validation scenario.

Scenario 4

Freight Audit

Delivery
   ↓
POD
   ↓
Invoice
   ↓
Validation
   ↓
Settlement

Scenario 5

Transportation Disruption

Load Delay
   ↓
Notification
   ↓
Escalation
   ↓
Recovery

Phase 10
Executive Recommendation

The final recommendation should not identify the "best vendor."

Instead it should answer:

Question 1

What is the best future-state architecture?

Possible outcomes:

Single TMS
Multi-platform
Composable architecture
Question 2

What delivers the highest business value?

Question 3

What produces the lowest operational risk?

Question 4

What produces the best 5-10 year strategic fit?

Expected Executive Decision Outcomes

At the end of the program, Interfor should be able to defend one of the following conclusions:

Outcome A

CarrierPoint remains strategically appropriate.

Outcome B

CarrierPoint remains, but modernization is required.

Outcome C

CarrierPoint plus complementary platforms.

Outcome D

Partial replacement.

Outcome E

Full replacement.

Outcome F

Composable Transportation Platform strategy.

My architectural recommendation

Before evaluating any vendor, create a Current-State Capability Heat Map against the Truck Capability Model (~150+ truck capabilities) and Rail Capability Model (~120+ rail capabilities).

That heat map will reveal:

what CarrierPoint already does well,
what Interfor has customized around,
where business pain truly exists,
where modernization should focus,
and whether a replacement business case actually exists.

Without that baseline, every vendor comparison becomes subjective. With it, the market evaluation becomes evidence-based and defensible.
