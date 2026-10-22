Create the initial current-state heat-map template


Interfor TMS 360° Assessment
Initial Current-State Capability Heat Map Template (Version 1.0)

This template is intended to be completed jointly by:

Supply Chain
Logistics Operations
Transportation SMEs
Rail SMEs
Finance/AP
IT Operations
Enterprise Architecture
Integration Team
Application Support

The goal is not to score vendors.

The goal is to establish:

"How well does Interfor's current transportation ecosystem perform today?"

CarrierPoint, LumberTrack, OMSI, SSIS, Oracle, Informatica, EDI processes, and supporting operational procedures should all be considered part of the evaluated solution landscape. Existing Interfor documentation and operational discussions indicate that transportation outcomes currently depend on multiple systems rather than CarrierPoint alone.

Scoring Model
Business Satisfaction Score
Score	Meaning5	Excellent
4	Good
3	Acceptable
2	Significant Pain
1	Major Deficiency
0	Not Available
Operational Risk
Score	MeaningL	Low Risk
M	Medium Risk
H	High Risk
Root Cause Classification
Code	MeaningPROD	Product Limitation
CONF	Configuration
INT	Integration
DATA	Data Quality
PROC	Process
GOV	Governance
USER	Adoption
OPS	Operations
SECTION A
Truck Transportation Heat Map
A1 Shipment Intake & Synchronization
Capability	Score	Risk	Root Cause	CommentsShipment Creation				
Shipment Updates				
Shipment Cancellation				
Split Shipments				
Shipment Consolidation				
LumberTrack Synchronization				
Data Reconciliation				
Error Recovery				
Replay Capability				
Transaction Traceability				
Guidance

Known synchronization, resend, reconciliation and OMSI transaction issues should be evaluated here. Historical evidence exists involving synchronization, retransmission and manual recovery procedures.

A2 Transportation Planning
Capability	Score	Risk	Root Cause	CommentsLoad Planning				
Multi-Stop Planning				
Consolidation Planning				
Capacity Planning				
Dynamic Replanning				
Manual Override				
Route Optimization				
Planning Visibility				
Planning Productivity				
A3 Carrier Management
Capability	Score	Risk	Root Cause	CommentsCarrier Onboarding				
Carrier Profiles				
Insurance Tracking				
Carrier Qualification				
Carrier Communications				
Carrier Scorecards				
Master Data Governance				
Carrier Data Synchronization				

Carrier onboarding, insurance tracking and synchronization processes already exist within the current OMSI/CarrierPoint ecosystem and should be assessed separately from the core TMS engine.

A4 Tendering & Procurement
Capability	Score	Risk	Root Cause	CommentsAutomated Tendering				
Contract Tendering				
Spot Tendering				
Carrier Acceptance				
Capacity Management				
Retendering				
Tender Reporting				
Tender Automation				
A5 Execution & Dispatch
Capability	Score	Risk	Root Cause	CommentsDispatching				
Pickup Scheduling				
Appointment Management				
Shipment Updates				
Delay Handling				
Exception Management				
Delivery Confirmation				
POD Collection				
A6 Visibility & Tracking
Capability	Score	Risk	Root Cause	CommentsReal-Time Tracking				
ETA Prediction				
Geofencing				
Event Tracking				
Milestone Tracking				
Customer Visibility				
Internal Visibility				
Exception Visibility				
A7 Freight Settlement
Capability	Score	Risk	Root Cause	CommentsReady-To-Pay				
POD Validation				
Freight Accruals				
Auto Billing				
Self Billing				
Invoice Matching				
Dispute Handling				
Remittance Capability				

Current AUTO-FAVI and Ready-to-Pay processes should serve as baseline evaluation scenarios.

A8 Compliance & Audit
Capability	Score	Risk	Root Cause	CommentsLegal Entity Controls				
Audit Traceability				
GST/HST Support				
Cross Border Support				
Invoice Dating				
Tax Compliance				
Exception Audit Trail				

Recent audit-related discussions identified invoice-date controls, legal-entity billing concerns and tax-compliance risks as material assessment areas.

SECTION B
Rail Transportation Heat Map
B1 Rail Planning
Capability	Score	Risk	Root Cause	CommentsRail Shipment Creation				
Rail Route Planning				
Equipment Assignment				
Car Allocations				
Empty Management				
Capacity Planning				
Unit Train Support				
B2 Rail Connectivity
Capability	Score	Risk	Root Cause	CommentsEDI 404				
Waybill Generation				
Waybill Updates				
Functional Acknowledgements				
Railroad Connectivity				
Error Recovery				
Replay Support				

Interfor's current landscape includes EDI 404 generation, acknowledgement processing and waybill updates back into LumberTrack.

B3 Railcar Lifecycle
Capability	Score	Risk	Root Cause	CommentsRailcar Visibility				
Loaded Car Tracking				
Empty Car Tracking				
Car Utilization				
Car Inventory				
Car History				
Fleet Management				
B4 Rail Visibility
Capability	Score	Risk	Root Cause	CommentsTrace Events				
Interchange Tracking				
ETA Visibility				
Exception Monitoring				
Dwell Monitoring				
Railroad Event Integration				
B5 Demurrage & Dwell
Capability	Score	Risk	Root Cause	CommentsDemurrage Prevention				
Dwell Analytics				
Free Time Management				
Cost Visibility				
Claims Recovery				
B6 Rail Financials
Capability	Score	Risk	Root Cause	CommentsRail Rate Management				
Rail Cost Accrual				
Invoice Validation				
Rail Settlement				
Audit Support				
SECTION C
Enterprise Architecture Heat Map
C1 Integration Architecture
Capability	Score	Risk	Root Cause	CommentsREST APIs				
Event Architecture				
OMSI Architecture				
EDI Integration				
SSIS Integration				
Oracle Integration				
Informatica Integration				
Error Recovery				

Current-state integration inventory should explicitly assess OMSI, SSIS, EDI, Oracle and related middleware dependencies.

C2 Data Architecture
Capability	Score	Risk	Root Cause	CommentsSource Of Record Clarity				
Master Data Ownership				
Data Quality				
Data Lineage				
Historical Retention				
Data Reconciliation				
C3 Security & Controls
Capability	Score	Risk	Root Cause	CommentsSSO				
MFA				
Role Security				
Carrier Access Controls				
Audit Logging				
Segregation Of Duties				
SOC Controls				

Current evidence shows enterprise SSO and documented security administration processes. SOC reports are available for the incumbent platform.

C4 Environment Management
Capability	Score	Risk	Root Cause	CommentsProduction Stability				
UAT Management				
Environment Refresh				
Test Data Management				
Release Process				
Disaster Recovery				

Existing UAT refresh and environment-management procedures should be assessed here.

C5 Operational Support
Capability	Score	Risk	Root Cause	CommentsMonitoring				
Alerting				
Incident Management				
Problem Management				
Vendor Escalation				
Root Cause Analysis				
Knowledge Transfer				
Executive Summary Heat Map

After workshops are completed, convert scores into:

Color	Meaning🟢 4.5-5.0	Strategic Strength
🟩 3.5-4.4	Healthy
🟨 2.5-3.4	Needs Improvement
🟧 1.5-2.4	Significant Concern
🟥 0-1.4	Modernization Candidate
Expected Outcome

This first heat map should answer four critical questions before any vendor comparison begins:

What does Interfor already do well?
What are the true pain points versus perceived pain points?
Which deficiencies belong to CarrierPoint versus integrations, data, process, or governance?
Is the business case pointing toward optimization, augmentation, or replacement?

Only after this baseline is completed should the assessment move into vendor scoring and market comparison.
