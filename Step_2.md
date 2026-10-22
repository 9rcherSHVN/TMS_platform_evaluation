This assessment is intended for Interfor. Yes, right now Interfor adopts IntelliTrans/CarrierPoint as the TMS business application platform. However, we want to perform a technical peer review (360 degree) on other TMS platforms available in the current TMS marketplace for a potential change - improvement - modernization. Interfor is a transportation-intensive enterprise, but we want to have a vendor-neutral TMS selection runbook (so keep the bias minimum). Any other questions if needed.



Understood. We are conducting an Interfor-specific, vendor-neutral 360-degree TMS peer review, not starting from a predetermined decision to replace IntelliTrans/CarrierPoint.

The intended outcome should be evidence-based:

Determine whether Interfor should retain and optimize CarrierPoint, modernize its CarrierPoint implementation, augment it with complementary platforms, progressively replace selected capabilities, or replace the TMS entirely.

Internal discovery found 6,278 file-domain results, 25 meetings, plus relevant emails and Teams discussions. The available evidence confirms that Interfor’s assessment must cover more than basic truck tendering. It needs to address LumberTrack integration, OMSI, shipment synchronization, carrier collaboration, dock scheduling, POD, freight settlement, rail-related processes, financial controls, legal entities, auditability, environment management, and operational support.

1. Confirmed assessment intent

I propose that the review answer six decision questions:

Business fit: Does the platform support Interfor’s actual transportation operating model?
Functional fit: Can it handle the required planning, execution, visibility, carrier, documentation and settlement capabilities?
Technical fit: Can it integrate cleanly and reliably with LumberTrack and the wider Interfor landscape?
Operational fit: Can Interfor support, monitor, test, reconcile and recover it efficiently?
Commercial fit: Is the total cost and vendor relationship sustainable?
Transformation fit: Does it enable Interfor’s future transportation strategy without excessive customization or lock-in?

The decision options should remain open:

Option A: Retain CarrierPoint as-is
Option B: Retain and remediate/modernize CarrierPoint
Option C: Retain CarrierPoint but add complementary services
Option D: Replace selected functional modules progressively
Option E: Replace CarrierPoint as the enterprise TMS
Option F: Adopt a composable transportation platform rather than a monolithic TMS

This prevents the assessment from becoming a disguised replacement justification.

2. Interfor facts already established

I will treat these as initially grounded facts, subject to field-level validation during the assessment.

Current platform and scope

Interfor uses IntelliTrans CarrierPoint, with documented functions including load tendering, quotation visibility, load-status updates and billing review. Rollout documentation indicates adoption across multiple East and Atlantic mill locations.

A 2024 statement of work identifies a truck-core implementation using an existing OMSI integration.

Current architectural boundary

Interfor documentation positions LumberTrack as the operational hub and CarrierPoint as an adjacent platform used for transportation planning and execution. The documented flow includes publishing an eligible shipment, selecting carrier/service/equipment/rate information, and returning applicable shipment attributes to LumberTrack.

Integration and reliability concerns that must become test criteria

Internal evidence identifies:

ready-date mismatches between LumberTrack and CarrierPoint involving date/time handling;
user-initiated changes used to retrigger transmission;
prior OMSI/server and transaction-resubmission issues;
operational reconciliation between CarrierPoint and LumberTrack;
uncertainty around some trigger and recalculation behavior;
UAT refresh impacts on test-specific configuration and security profiles.

These should not automatically be classified as CarrierPoint product deficiencies. Some may originate in Interfor custom integration, data ownership, middleware, configuration or process design. The peer review must use root-cause classification rather than attributing every current problem to the incumbent vendor.

Freight settlement and audit controls

A transcribed October 8, 2026 meeting documents the need to align self-generated invoice dates with delivery-confirmation or signed-BOL dates, distinguish service/invoice dates from posting dates, transmit delivery evidence into LumberTrack, generate appropriate invoice references, and enforce correct Interfor legal-entity billing. The meeting also identifies an audit trail concern where equivalent delivery evidence may not always exist.

These are therefore mandatory scenario-test subjects, not optional financial features.

Security and controls

Interfor has IntelliTrans SOC 1 Type 2 and SOC 2 Type 2 reports on file. The SOC 2 excerpt states that CarrierPoint and GVP are used for shipment management and invoice processing.

3. Additional information I need

Yes, I need some targeted input, but I do not need every answer before beginning. Unknowns can be explicitly recorded as discovery items.

A. Decision mandate and boundaries

What triggered the peer review?

license or renewal event;
executive modernization initiative;
business dissatisfaction;
integration/support cost;
capability gaps;
acquisition/divestiture considerations;
audit/compliance;
vendor concentration;
or a scheduled architecture review?

Is full replacement genuinely in scope, including carrier cutover, historical data migration, interface rebuilding and retraining?

Are there any constraints such as:

contract end or notice date;
budget ceiling;
expected implementation window;
blackout periods;
corporate SaaS or cloud standards;
required data residency;
restrictions on public-cloud providers?
B. Transportation scope

Please confirm the modes that must be evaluated:

truckload;
less-than-truckload;
rail;
intermodal;
ocean;
parcel;
private or dedicated fleet;
spot brokerage;
cross-border Canada/US;
inbound raw materials;
outbound finished lumber;
mill transfers or shuttles.

Most importantly: must one TMS handle truck and rail deeply, or may Interfor use a best-of-breed multimode architecture?

That is a major product-market separator.

C. Organizational model

I need the actual operating model:

centralized versus regional transportation planning;
mill-level shipping responsibilities;
who owns carrier procurement;
who tenders and awards loads;
who manages exceptions;
who confirms delivery;
who approves freight payment;
who owns carrier and rate master data;
which activities differ among West, South, East and Atlantic operations.

A vendor may look strong against an enterprise checklist but fail if it cannot support Interfor’s degree of regional autonomy.

D. Quantitative baseline

Approximate ranges are acceptable:

annual shipments by mode;
annual freight spend;
number of active carriers;
number of shipping locations and receiving/customer locations;
peak daily shipment volume;
cross-border shipment percentage;
percentage contract versus spot;
approximate annual freight invoices or self-billed transactions;
number of internal users and carrier users.

Without this, vendor sizing, performance requirements, subscription comparison and business case cannot be defensible.

E. Current capability satisfaction

For each area, I need a simple score:

Green: working adequately
Amber: working but needs improvement
Red: material problem
Not used
Unknown

Areas:

shipment planning;
load consolidation;
routing;
rating;
contract rates;
spot bids;
carrier tendering;
rail execution;
equipment/car management;
appointment and dock scheduling;
real-time visibility;
ETA/event management;
carrier portal/mobile;
POD and document management;
claims;
freight audit;
accruals;
self-billing/settlement;
carrier performance;
analytics;
carbon/emissions;
APIs/integration;
configuration;
security;
support and release management.
F. Technical landscape

I will need confirmation of:

deployed LumberTrack environments and versions;
OMSI ownership and deployed versions;
SSIS interfaces and scheduling;
direct REST APIs currently used;
EDI transactions in scope;
Informatica IDMC/MFT/B2B responsibilities;
Oracle ERP touchpoints;
Power BI reporting;
identity and SSO model;
monitoring and alerting;
ServiceNow operational workflow;
master-data ownership;
production, UAT, test and disaster-recovery topology.

The existing documentation already identifies LumberTrack, CarrierPoint, OMSI/SSIS, EDI 404 and 601, Informatica delivery channels, Kleinschmidt and other partner connectivity, but the production boundaries still require validation.

G. Vendor universe

I recommend evaluating vendors by archetype first, not by brand:

Enterprise multimode TMS
Mid-market configurable TMS
Bulk/rail and industrial transportation specialists
Real-time transportation visibility platforms
Freight audit and payment providers
Carrier connectivity and digital freight networks
ERP-native transportation management
Composable transportation execution platforms

This prevents products such as project44, which may occupy a different architectural role from a complete TMS, from being scored as though all products are direct substitutes.

Please identify any vendors that executives require in the long list. Candidate names may include:

IntelliTrans
MercuryGate
Descartes
Oracle Transportation Management
SAP Transportation Management
Blue Yonder
Manhattan Active Transportation Management
e2open
Infor Nexus
Trimble
project44
FourKites

Inclusion in research would not imply suitability or equivalence.

H. Evidence and scoring governance

Please identify:

executive sponsor;
procurement owner;
architecture owner;
transportation SMEs;
logistics representatives by region;
finance/AP/tax representation;
security and privacy reviewers;
support/operations representatives;
final decision authority.

I also recommend requiring every score to carry an evidence class:

D: vendor documentation;
C: configuration demonstrated live;
S: scenario executed successfully;
R: customer reference validated;
T: technical artifact inspected;
P: production measurement;
U: unverified vendor assertion.

This will prevent polished demonstrations from outweighing verified operational fit.

4. Assumptions I suggest using initially

Unless corrected, I will proceed with these working assumptions:

-The assessment is a modernization and strategic fit review, not an approved replacement project.
-CarrierPoint remains the incumbent baseline and must be scored using the same criteria as peers.
-LumberTrack remains the core operational system during the evaluation.
-Truck and rail capabilities must be assessed separately.
-Canada/US cross-border and multi-legal-entity requirements are material.
-Freight settlement, POD, delivery dates, taxes, accruals, invoice controls and audit traceability are mandatory.
-Interfor wants SaaS solutions but will evaluate integration, data portability, security and vendor lock-in rigorously.
-A modular “TMS plus visibility plus settlement” architecture may compete against a single-suite design.
-Vendor marketing claims will not receive credit without evidence.
-Current incidents will be classified by root cause: product, configuration, customization, integration, data, process, support or governance.

The one decision I need from you now

Should the first runbook evaluate truck plus rail as one combined enterprise-TMS decision, or should it use two capability tracks, truck TMS and rail/industrial logistics, with a later architecture decision on whether one platform or multiple platforms should support them?
