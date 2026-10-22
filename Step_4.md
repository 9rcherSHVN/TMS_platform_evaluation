
Define the Truck and Rail capability model

Interfor Truck and Rail TMS Capability Model

This capability model is designed as the master taxonomy for Interfor’s vendor-neutral 360-degree assessment. It separates Truck and Rail capabilities while retaining common enterprise controls for finance, integration, data, security, analytics and operations.

The model should be used consistently across:

current-state assessment;
business requirements;
incumbent baseline review;
RFI/RFP;
vendor demonstrations;
scripted scenario testing;
technical proof of concept;
total-cost analysis;
implementation planning;
final decision scoring.

It deliberately avoids assuming that one vendor must provide every capability.

1. Capability-model structure

Each capability is classified at four levels:

L0: Transportation Management
L1: Capability track, such as Truck or Rail
L2: Capability domain, such as Tendering
L3: Assessable capability, such as Sequential Tendering
L4: Detailed requirement or scenario, created later

Example:

Transportation Management → Truck → Tendering → Sequential Tendering → Tender a contract carrier and automatically cascade after timeout.

Capability treatment codes

Every capability should receive one of these dispositions:

Code	TreatmentM	Mandatory
I	Important
D	Differentiating
F	Future
N/A	Not applicable
G	Evaluation gate, failure may disqualify a vendor
Platform-placement codes

These prevent the assessment from assuming the TMS should own everything:

Code	Architectural placementTMS	Native TMS capability
ERP/OMS	LumberTrack, ERP or order-management responsibility
VIS	Visibility/control-tower platform
FAP	Freight audit and payment platform
INT	Integration platform or custom service
EXT	External carrier, railroad, broker or data provider
SHARED	Distributed across platforms
2. Track A: Truck capability model
T1. Demand intake and shipment creation
T1.1 Transportation-demand intake
Create transportation demand from sales orders
Create demand from shipments or releases
Create inbound transportation demand
Create intercompany and inter-mill transfers
Create manual and ad hoc shipments
Create customer-return movements
Create shuttle and local-haul movements
Import bulk shipment requirements
Maintain demand source and transaction lineage
T1.2 Shipment qualification
Determine TMS eligibility
Validate origin and destination
Validate ship and delivery windows
Validate mode and equipment
Validate weight, volume and quantity
Validate route and service requirements
Identify hazmat or regulated goods
Identify cross-border requirements
Detect incomplete or duplicate demand
Route invalid shipments into an exception queue
T1.3 Shipment synchronization
Create shipment in TMS
Update existing shipment
Cancel shipment
Split shipment
merge or consolidate shipments
Preserve source-system identifiers
Maintain version and update sequence
Prevent stale updates
Detect source/TMS discrepancies
Confirm processing to the source system

Interfor anchor: Existing documentation describes eligible LumberTrack shipments being made available to CarrierPoint, followed by transportation planning and the return of applicable shipment attributes. The precise publication event, transaction boundary and field-level ownership remain validation items. ATS-to-Order Process details_0.docx and LumberTrack Forecast-to-Cash Process Chain - V2.docx are useful baselines.

T2. Transportation planning and optimization
T2.1 Shipment planning
Plan single-order loads
Plan multi-order loads
Plan multi-stop loads
Consolidate compatible shipments
Deconsolidate loads
Support pool distribution
Support continuous-move planning
Plan inbound and outbound combinations
Plan backhauls
Plan empty repositioning
Lock or freeze approved plans
T2.2 Constraint management
Origin operating hours
Destination receiving hours
Mill production and availability dates
Customer-requested delivery dates
Weight and cube limits
Equipment constraints
Product compatibility
Carrier lane restrictions
Border crossing constraints
Driver-hours constraints
Appointment availability
Route restrictions
Seasonal and weather restrictions
T2.3 Optimization
Least-cost planning
Service-constrained optimization
Multi-objective optimization
Carrier-capacity-aware optimization
Consolidation optimization
Multi-stop sequencing
Dynamic replanning
What-if simulation
Planner override
Explain optimization results
Compare optimized and actual outcomes
T2.4 Plan approval and execution release
Approval workflow
Regional approval thresholds
Cost-variance approval
Manual override with reason
Release plan to tendering
Reopen approved plan
Audit planning changes
T3. Route, lane, rate and contract management
T3.1 Transportation network
Origin and destination master
Lane definitions
Region and operating division
Route guides
Transit-time profiles
Distance and mileage
Border crossings
Restricted routes
Alternate routes
T3.2 Contract management
Carrier contracts
Effective and expiry dates
Lane commitments
Volume commitments
Equipment commitments
Minimum charges
Fuel schedules
Accessorial schedules
Currency
Tax treatment
Contract document association
Contract approval and versioning
T3.3 Rating
Base freight calculation
Mileage-based rates
Flat rates
Zone rates
Weight and volume rates
Fuel surcharge
Multi-stop charges
Detention charges
Tarping and loading charges
Border and customs charges
Seasonal adjustments
Minimum and maximum charges
Rate stacking and precedence
Tax calculation inputs
Rate simulation
Rate explanation
Re-rating after shipment change
T3.4 Rate governance
Rate import
Rate validation
Duplicate detection
Approval workflow
Effective dating
Rate audit history
Expiry notification
Exception reporting
Contract-versus-spot comparison
T4. Carrier lifecycle and compliance
T4.1 Carrier onboarding
Carrier registration
Company and contact information
Operating authority
Tax identifiers
Banking/payment information
Supported modes and equipment
Service areas and lanes
Portal-user creation
Document submission
Approval workflow
T4.2 Carrier qualification
Insurance tracking
Insurance expiry controls
Safety-rating validation
Authority validation
Sanctions/compliance checks
Carrier status and blocking
Equipment qualification
Cross-border qualification
Regional qualification
Conditional approval
T4.3 Carrier master governance
Source-of-record assignment
Duplicate-carrier prevention
Carrier identifier cross-reference
Parent/subsidiary relationships
Broker/carrier distinction
Legal-name management
Payment-vendor linkage
Controlled master-data changes
Synchronization with source systems
T4.4 Carrier performance
Tender acceptance
Pickup performance
Delivery performance
Tracking compliance
POD compliance
Invoice accuracy
Claims performance
Capacity fulfilment
Service failures
Scorecards
Corrective-action tracking

Interfor anchor: Carrier-related information is exchanged through the current OMSI/CarrierPoint landscape, and internal discussion has identified proprietary configuration and uncertainty around some insurance-data transformations. This should become an explicit test of carrier-master ownership, extensibility, monitoring and error handling. Carrier insurance transformation discussion

T5. Procurement, tendering and capacity
T5.1 Strategic sourcing
Annual bid events
Mini-bids
Lane bundles
Carrier participation
Bid validation
Bid comparison
Scenario award analysis
Volume allocation
Award approval
Convert awards to operational rates
T5.2 Operational tendering
Manual tender
Automated tender
Sequential tender
Broadcast tender
Route-guide tender
Primary and backup carriers
Tender timeout
Auto-accept rules
Carrier rejection reasons
Retendering
Tender withdrawal
Tender history
T5.3 Spot procurement
Spot quote request
Multi-carrier spot bidding
Broker marketplace connectivity
Bid expiration
Bid comparison
Capacity confirmation
Approval thresholds
Spot-versus-contract variance
Convert spot award into shipment cost
T5.4 Capacity management
Contracted capacity
Carrier-provided capacity
Lane capacity
Daily and weekly allocation
Capacity shortfall alerts
Peak-season capacity
Equipment availability
Carrier commitment performance
Capacity forecasting
T6. Truck execution
T6.1 Dispatch and pickup
Dispatch confirmation
Driver and tractor assignment
Trailer assignment
Pickup appointment
Arrival and departure
Loading status
Pickup confirmation
Pickup exception
Reschedule pickup
Shipping-document availability
T6.2 In-transit management
Departed origin
En route
Border arrival and release
Stop arrival and departure
Delay event
Route deviation
Breakdown
Weather disruption
Missed appointment
Updated ETA
Recovery action
T6.3 Delivery completion
Delivery arrival
Unloading status
Delivery confirmation
Partial delivery
Refused delivery
Damage or shortage
Signed POD
Delivery date and time
Completion approval
Close shipment
T6.4 Shipment change control
Change carrier
Change equipment
Change pickup date
Change destination
Change quantity
Add or remove stop
Re-rate changed load
Re-tender changed load
Notify affected parties
Preserve change audit history
T7. Visibility and exception management
T7.1 Connectivity
Driver mobile application
Carrier portal
Telematics integration
ELD integration
Mobile-phone tracking
Visibility-network integration
API event ingestion
EDI 214 status messages
Manual status entry
T7.2 Tracking
Current vehicle position
Shipment status
Predicted arrival time
Milestone tracking
Stop-level tracking
Geofencing
Route adherence
Tracking-quality indicator
Last-known-position age
Data-source attribution
T7.3 Exception management
Late pickup prediction
Late-delivery prediction
Missing tracking
Route deviation
Unplanned stop
Excessive dwell
Missed appointment
Failed delivery
Missing POD
Configurable severity
Exception ownership
Escalation workflow
Resolution notes
Root-cause coding
T7.4 Customer and internal visibility
Customer tracking portal
Internal control-tower view
Mill shipment view
Logistics view
Customer-service view
Proactive notifications
Role-based event filtering
ETA sharing
Exception communication history
T8. Appointment, yard and facility operations
T8.1 Appointment scheduling
Pickup appointments
Delivery appointments
Carrier self-scheduling
Dock calendars
Appointment capacity
Blackout periods
Rescheduling
Appointment confirmation
Appointment reminders
No-show tracking
T8.2 Gate operations
Pre-arrival registration
Driver check-in
Trailer check-in
Security validation
Gate arrival
Gate departure
Queue position
Gate pass
Exception handling
T8.3 Yard management
Yard inventory
Trailer location
Loaded and empty status
Yard move requests
Spotter assignment
Dock-door assignment
Dwell time
Trailer aging
Yard exception alerts
T8.4 Dock coordination
Dock schedule
Door assignment
Load readiness
Loading start/end
Unloading start/end
Detention measurement
Facility throughput
Dock utilization
T9. Documentation and regulatory support
T9.1 Shipment documents
Bill of lading
Delivery slip
Packing documentation
Rate confirmation
Carrier instructions
Customs documentation
Document templates
Electronic document distribution
T9.2 POD management
Carrier POD upload
Driver image capture
Electronic signature
POD indexing
Image-quality validation
Required-field validation
Delivery-date extraction
Exception workflow
Source-system distribution
Retention and retrieval
T9.3 Cross-border support
Canada/US shipment attributes
Customs broker identification
Border-crossing location
Customs-status tracking
Document exchange
Regulatory-data completeness
Hold and release
Audit trail
T10. Truck freight financial management
T10.1 Planned and accrued cost
Planned freight cost
Carrier-accepted cost
Shipment accrual
Accessorial accrual
Fuel accrual
Cost allocation
Multi-order allocation
Currency conversion
Re-accrual after change
Source-system synchronization
T10.2 Freight audit
Invoice ingestion
Contract-rate validation
Duplicate invoice detection
Shipment-invoice matching
Accessorial validation
Fuel validation
Tax validation inputs
Tolerance rules
Invoice exceptions
Dispute workflow
Credit and adjustment processing
T10.3 Settlement and self-billing
Ready-to-pay status
POD prerequisite
Delivery confirmation prerequisite
Self-billed invoice creation
Carrier-submitted invoice
Approval workflow
Service/invoice date
Posting date
Unique invoice reference
Payment hold
Payment export
Remittance details
Reversal and reprocessing
T10.4 Legal-entity and tax controls
Paying legal entity
Operating division
Carrier billing entity
Ship-from and ship-to jurisdictions
GST/HST/QST inputs
US tax handling
Cross-border treatment
Effective-dated tax rules
Tax audit trail
Posting-period controls

Interfor anchor: The transcribed Lumbertrack AP Auto-Generated Invoices - Invoice Date (Carrierpoint, FRT-POS & FRT-RAIL) establishes the importance of delivery-confirmation dates, POD, Ready-to-Pay, service/invoice versus posting dates, unique invoice references and correct legal-entity billing. These should be mandatory scripted scenarios, not questionnaire-only capabilities.

3. Track B: Rail capability model
R1. Rail transportation demand
R1.1 Rail-order intake
Create rail transportation demand
Receive order/shipment information
Identify rail-eligible shipments
Identify origin and destination rail access
Determine product and equipment needs
Manage requested ship and delivery dates
Support unit-train and manifest demand
Support multi-order rail shipments
Preserve source references
R1.2 Demand validation
Validate serving carrier
Validate rail station and Standard Point Location Code
Validate route
Validate commodity
Validate equipment
Validate weight and loading limits
Validate customer rail capability
Validate customs requirements
Detect duplicate demand
Route incomplete demand to exception handling
R1.3 Demand-to-shipment conversion
Create rail shipment
Group demand into rail movements
Split shipments
Change shipment quantity
Cancel shipment
Reissue shipment
Synchronize status to LumberTrack
Maintain source-to-waybill lineage
R2. Rail network, route and carrier management
R2.1 Rail network master
Origin and destination stations
Serving railroads
Junctions and interchanges
Rail routes
Short-line relationships
Switching locations
Customer sidings
Mill tracks
Serving-yard definitions
Border gateways
Route restrictions
R2.2 Rail-carrier master
Railroad identifiers
Carrier codes
Contacts
Service regions
Billing relationships
EDI connectivity
Contract association
Carrier status
Parent/subsidiary relationships
R2.3 Route management
Single-line routes
Multi-carrier routes
Interchange routing
Preferred routes
Alternate routes
Embargo-aware routing
Transit standards
Route effective dating
Route approval
Route audit history
R2.4 Rail-service selection
Carrier selection
Route selection
Service-level comparison
Transit-time comparison
Cost comparison
Equipment availability
Customer restrictions
Manual override
Selection rationale
R3. Rail equipment and fleet management
R3.1 Railcar master
Car initials and number
Equipment type
Ownership
Lease information
Capacity
Dimensions
Product compatibility
Loading restrictions
Maintenance status
Inspection status
Home route
Active/inactive status
R3.2 Equipment planning
Equipment demand
Available-car inventory
Car-order creation
Car assignment
Empty-car allocation
Substitution rules
Shortage detection
Surplus detection
Repositioning
Pool management
R3.3 Railcar lifecycle
Empty release
Placement
Loading
Loaded release
In transit
Interchange
Constructive placement
Actual placement
Unloading
Empty return
Bad order
Maintenance event
Retirement
R3.4 Fleet utilization
Loaded versus empty days
Cycle time
Dwell time
Trips per car
Miles per car
Idle equipment
Fleet imbalance
Car availability forecast
Lease utilization
Equipment-performance scorecard
R4. Rail shipment planning
R4.1 Load planning
Product-to-car compatibility
Car-capacity utilization
Weight distribution
Shipment quantity allocation
Multi-car shipment
Unit-train planning
Loading sequence
Mill-track capacity
Customer unloading constraints
R4.2 Shipment scheduling
Requested ship date
Car-order lead time
Placement schedule
Loading window
Railroad cutoff
Interchange schedule
Estimated delivery
Customer receiving window
Schedule-change impact
R4.3 Constraint planning
Equipment availability
Track capacity
Mill loading capacity
Railroad service days
Seasonal restrictions
Embargoes
Route closures
Customer siding limits
Commodity restrictions
Cross-border constraints
R4.4 Plan approval
Equipment-plan approval
Route approval
Cost approval
Exception approval
Manual override
Release to execution
Plan-change audit
R5. Rail rates, tariffs and contracts
R5.1 Rail-rate management
Origin/destination rates
Commodity rates
Car-type rates
Weight-based rates
Mileage-based rates
Multi-carrier rates
Switch charges
Fuel surcharge
Border charges
Minimum charges
Accessorial charges
R5.2 Contract and tariff management
Railroad contracts
Tariffs
Circulars
Effective dates
Volume commitments
Equipment commitments
Route restrictions
Escalation clauses
Contract documents
Amendments and versions
R5.3 Rail rating
Pre-shipment rating
Route-cost comparison
Interline cost
Accessorial projection
Fuel calculation
Re-rating
Rate explanation
Contract-versus-invoice comparison
Estimated landed transportation cost
R6. Rail shipment execution and waybilling
R6.1 Shipping instructions
Create shipping instructions
Origin and destination
Route
Commodity
Weight
Car identification
Consignee
Care-of party
Notify party
Customs broker
Special instructions
Hazardous-material details where applicable
R6.2 Waybill management
Create waybill request
Submit waybill
Amend waybill
Cancel waybill
Receive waybill number
Receive waybill date
Associate waybill with shipment/BOL
Detect duplicate submissions
Manage rejected submissions
Preserve submitted and acknowledged versions
R6.3 EDI 404 processing
Generate EDI 404 data
Validate mandatory fields
Map source values
Transmit through trading-partner connectivity
Receive functional acknowledgement
Process acceptance or rejection
Capture waybill response
Correlate response to shipment
Replay failed transactions
Reconcile submitted and acknowledged records
R6.4 Delivery and completion
Arrival at destination
Placement
Customer notification
Unloading
Empty release
Delivery completion
Damage or shortage
Shipment closure
Source-system completion update

Interfor anchor: EDI_Interfaces_Lumbertrack_20250925_m.docx documents an Interfor rail BOL flow involving LumberTrack XML, SSIS validation and EDI 404 transformation, Kleinschmidt transmission, acknowledgements, and return of waybill number and date to LumberTrack. These controls should be converted into vendor-neutral capabilities rather than reproduced as mandatory future architecture.

R7. Rail event visibility and tracing
R7.1 Rail event ingestion
Railroad event feeds
EDI 214/417 or applicable event messages
CLM/event data
Carrier portal updates
Manual event entry
API event updates
Multi-railroad event normalization
R7.2 Railcar tracing
Current car location
Last event
Event date and time
Loaded/empty state
Train identification
Serving railroad
Estimated interchange
Estimated arrival
Trip history
Map and list views
R7.3 Interchange visibility
Interchange offered
Interchange accepted
Interchange completed
Connecting-carrier handoff
Interchange dwell
Missed interchange
Event discrepancy
Ownership during handoff
R7.4 Rail exceptions
No movement
Excessive dwell
Route deviation
Missed interchange
Bad order
Embargo
Car rejected
Incorrect destination
Late placement
Late delivery
Missing event
Lost or unlocated car
Exception ownership and escalation
R8. Demurrage, detention and accessorials
R8.1 Free-time management
Free-time rules
Constructive placement time
Actual placement time
Release time
Customer-specific rules
Facility-specific rules
Weekend and holiday rules
Rule effective dates
R8.2 Demurrage calculation
Chargeable days
Credits
Debits
Average agreement
Straight demurrage
Railroad-specific rules
Estimated exposure
Final charge calculation
Recalculation after event correction
R8.3 Demurrage prevention
Cars approaching free-time limit
Cars exceeding free time
Empty-release reminders
Facility congestion
Customer unloading delay
Exception assignment
Preventive-action workflow
R8.4 Accessorial audit
Invoice matching
Event-based validation
Rate validation
Duplicate-charge detection
Dispute creation
Supporting-event evidence
Credit tracking
Recovery reporting
R9. Rail facility, yard and inventory management
R9.1 Mill rail-yard inventory
Cars on site
Cars by track
Loaded cars
Empty cars
Cars awaiting loading
Cars awaiting release
Bad-order cars
Track capacity
Car aging
R9.2 Switching and moves
Internal move request
Switch-list creation
Track assignment
Move sequencing
Move confirmation
Railroad switch request
Switching status
Switching exceptions
R9.3 Loading operations
Car inspection
Loading readiness
Product assignment
Loading start and completion
Loaded weight
Seal information
Document readiness
Release approval
R9.4 Inventory reconciliation
Physical versus system car inventory
Missing-car identification
Duplicate-car identification
Track-location correction
Event reconciliation
Cycle-count support
Audit history
R10. Rail financial management
R10.1 Planned and accrued rail cost
Linehaul estimate
Fuel estimate
Switching charges
Handling charges
Demurrage exposure
Equipment lease cost
Cost allocation
Accrual generation
Accrual adjustment
R10.2 Rail freight audit
Railroad invoice ingestion
Waybill-to-invoice matching
Rate validation
Fuel validation
Route validation
Switching-charge validation
Demurrage validation
Duplicate invoice detection
Overcharge identification
Dispute workflow
R10.3 Rail settlement
Invoice approval
Self-billing where applicable
Payment hold
GL coding
Legal-entity assignment
Tax inputs
ERP/AP export
Remittance
Reversal and correction
Payment-status feedback
R10.4 Claims and recovery
Damage claims
Loss claims
Shortage claims
Service claims
Supporting documents
Railroad communication
Claim amount
Claim status
Recovery amount
Claim aging
4. Shared enterprise capability model

These capabilities must be scored independently from Truck and Rail functional depth.

E1. Integration and interoperability
REST APIs
SOAP services where required
Webhooks and event subscriptions
EDI
Managed file transfer
SFTP
Batch import/export
Streaming/event integration
Canonical transportation model
Idempotent processing
Correlation identifiers
Message sequencing
Duplicate detection
Retry and replay
Dead-letter handling
Interface reconciliation
Schema versioning
API lifecycle management
Integration health dashboard

For Interfor, testing should explicitly cover OMSI replacement/retention options, SSIS dependencies, LumberTrack invocation patterns, EDI connectivity and partner gateways. Current materials show that these technologies participate in the existing landscape, but they do not establish that each must remain in the target state. OMSI Manual V25.04.docx and Customer and Regulatory Integration.docx provide current-state evidence.

E2. Data management
Transportation master data
Carrier master
Location master
Equipment master
Lane and route master
Rate master
Reference-data crosswalks
Field-level system of record
Data-quality rules
Effective dating
Data lineage
Data retention
Archiving
Bulk extraction
Data portability
Historical migration
Reconciliation
Purge and privacy controls
E3. Workflow and extensibility
Configurable workflow
Business rules
Approval rules
User-defined fields
Configurable statuses
Configurable alerts
Configurable documents
Low-code extensibility
Supported custom services
Extension isolation
Upgrade-safe customization
Rule versioning
Promotion between environments
Audit trail
E4. Security, privacy and controls
Microsoft Entra ID SSO
MFA compatibility
Role-based access
Location-based access
Segregation of duties
Carrier-user isolation
Privileged access control
Service-account governance
API authentication
Encryption in transit
Encryption at rest
Security logging
Audit logs
Data residency
Retention
SOC 1 reporting
SOC 2 reporting
Vulnerability management
Incident notification
Business continuity
Disaster recovery

Current access documentation describes a process involving an IntelliTrans SSO Active Directory group and CarrierPoint user/location permissions. SOC 1 Type 2 and SOC 2 Type 2 reports are also held internally; future vendors should be evaluated against equivalent evidence, not merely security-questionnaire responses. TMS CarrierPoint Granting Access.docx, IntelliTrans - SOC 1 Type 2 Final Report 093025.pdf and IntelliTrans - SOC 2 Type 2 Final Report 093025.pdf

E5. Platform operations
Production environment
UAT environment
Integration-test environment
Training environment
Environment refresh
Configuration backup
Masked test data
Release calendar
Release notes
Regression testing
Backward compatibility
Availability monitoring
Performance monitoring
Interface monitoring
Alerting
Service-level reporting
Incident management
Problem management
Vendor escalation
Root-cause analysis
Recovery testing
Operational reconciliation

An IntelliTrans UAT bulletin states that a refresh replaces the current UAT dataset, configuration and user profiles with production data and may overwrite UAT-only configurations. This makes environment independence, backup, configuration promotion and regression testing material evaluation areas. FW: Action requested: IntelliTrans TMS UAT environment refresh

E6. Analytics and decision support
Shipment volume
Freight spend
Cost per unit
Cost per mile
Cost by lane
Cost by mill
Cost by customer
Tender acceptance
On-time pickup
On-time delivery
Transit performance
Carrier performance
Tracking compliance
POD compliance
Accessorial cost
Demurrage
Railcar utilization
Cycle time
Exception aging
Settlement accuracy
Accrual-versus-actual analysis
Savings measurement
Root-cause analysis
Self-service reporting
Power BI integration
Data-lake export
Scheduled reports
KPI definitions and lineage
E7. User experience and collaboration
Planner workspace
Dispatcher workspace
Rail-operations workspace
Carrier portal
Mobile experience
Customer-service view
Finance workspace
Exception work queue
Role-personalized dashboards
Search
Bulk actions
Accessibility
English and French support
Notifications
Email collaboration
Teams integration
Contextual help
User-adoption analytics
E8. Artificial intelligence and automation

These should initially be treated as differentiating or future, not allowed to compensate for missing core controls.

Predictive ETA
Disruption prediction
Carrier recommendation
Capacity prediction
Rate prediction
Load-consolidation recommendation
Route recommendation
Exception prioritization
Automated document classification
POD data extraction
Invoice anomaly detection
Demurrage-risk prediction
Natural-language analytics
Planner copilot
Explainable recommendations
Human approval
Model confidence
Model monitoring
AI audit trail
Customer-data isolation
E9. Vendor and commercial capabilities
Product viability
Transportation industry focus
Forest-products experience
Truck depth
Rail depth
Product roadmap
Research and development commitment
Implementation partners
North American support
Escalation model
Reference customers
Customer advisory program
Release governance
Data ownership
Contract exit rights
Data extraction on termination
Pricing transparency
Volume scalability
Acquisition risk
Subprocessor transparency
5. Recommended Interfor criticality profile

This is an initial architectural recommendation, not a statement of approved business priority.

Mandatory and potential gate capabilities
Truck gates
LumberTrack shipment synchronization
Date/time-zone correctness
Carrier tendering and acceptance
Carrier portal/connectivity
POD and delivery confirmation
Ready-to-Pay
Freight accrual and settlement integration
Legal-entity controls
Cross-border support
Replay and reconciliation
Full transaction audit trail

Internal email evidence documents ready-date mismatches and manual retrigger/resubmission patterns. These operational scenarios should be recreated during vendor testing. RE: Loads not coming across to CP this morning from LT and RE: Ready dates are not matching from LT to CP

Rail gates
Rail-route and carrier support
Rail equipment identification
Rail shipment and BOL creation
EDI 404 or equivalent railroad connectivity
Waybill acknowledgement and correlation
Waybill number/date return
Car tracing
Event normalization
Demurrage and dwell management
Rail freight-audit evidence
Transaction replay and reconciliation
Enterprise gates
Supported APIs and integration patterns
Idempotency and correlation
Environment separation
Configurable security
Audit logs
Data extraction and portability
Availability and disaster recovery
SOC/control evidence
Volume and performance validation
Upgrade-safe extensibility
6. Capability scoring method

Each shortlisted platform should receive more than a simple 1-to-5 score.

A. Functional fit
Score	Meaning0	Not available
1	External manual process required
2	Major customization or separate product required
3	Available through configuration or standard partner
4	Strong native capability
5	Advanced native capability validated through an Interfor scenario
B. Evidence strength
Code	EvidenceU	Vendor assertion only
D	Product documentation reviewed
C	Configuration demonstrated
S	Interfor scenario executed
T	Technical artifact inspected
R	Customer reference validated
P	Production evidence or measured result

A score of 5 should not be permitted with only U or D evidence.

C. Delivery impact

For every capability, record:

native module;
optional licensed module;
partner solution;
customization;
integration dependency;
process workaround;
unavailable;
implementation complexity;
recurring cost;
migration impact;
operating owner.
D. Derived risk

A useful evaluation formula is:

Evidence-adjusted fit = Functional fit × Evidence factor × Criticality factor

Suggested evidence factors:

U = 0.40
D = 0.60
C = 0.75
S = 0.90
T/R = 0.95
P = 1.00

This ensures a vendor’s unverified “yes” does not score the same as a successfully executed Interfor scenario.

7. Architectural decision enabled by the model

The completed model should support comparison of four target-state patterns:

Single multimode TMS
 One platform owns Truck and Rail.

Truck TMS plus rail specialist
 Separate execution platforms with shared enterprise integration and analytics.

Core TMS plus specialist services
 TMS combined with visibility, freight payment, appointment or rail services.

Composable transportation platform
 Truck, Rail, visibility and settlement services coordinated through an Interfor-controlled integration and data layer.

The final decision should therefore score both vendors and architecture combinations. A vendor that is excellent for Truck but moderate for Rail should not be eliminated if a two-platform design offers better overall fit, provided the integration, data consistency, support and total-cost impacts are acceptable.
