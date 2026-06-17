# ET-W2IT meeting (8/10-JUN-2026, Brasilia): Minutes

## Summary of actions:

### 2. Designation and decommissioning procedures for WIS2 services

- [ ] ACTION (@hhaddouch) to update Manual 2.6.2.3 with new paragraph on balancing overall WIS2 performance against additional Global Service instances
- [x] ACTION (@tomkralidis) to draft new Manual text for Other Services and Sensor Centre sections (3.2.15, 3.2.16) — complete
- [x] ACTION (@6a6d74) to draft the Other Services designation process — complete
- [ ] ACTION (@hhaddouch) to amend Manual 2.6.5.2 to introduce "experimental marking" for centre-id in the Code Registry
- [x] ACTION (@hhaddouch) to add a statement to Manual 2.8.2.1 on Secretariat engagement regarding incidents — complete
- [x] ACTION (@tomkralidis) to move "General" from Guide 2.7.2.4 to 2.7.2.1 — complete
- [ ] ACTION (@tomkralidis) to consider updating/complementing the global-service-type code list to include Sensor Centre Types and Other Services
- [x] ACTION (@kaiwirt) to change DCPC designation procedure 2.3.4 wording — complete
- [x] ACTION (Secretariat) to change DCPC designation process to require only p/INFCOM approval — complete
- [ ] ACTION (Secretariat) to add a brief note on decommissioning/phasing-out RTHs to the INFCOM-4 report

### 3. Performance measures and monitoring for WIS2 services

- [ ] ACTION (@golfvert) to add `rel` label (canonical/update) to SCGC metrics and update `metrics/scgc.csv`
- [ ] ACTION (@golfvert) to confirm via further analysis that 60-second cut-off is optimal for SCGB "missed message" detection
- [ ] ACTION (@shirley-xuelei, @elgarraichemseddine) to port SCGB and SCGC dashboards to the Global Monitors
- [ ] ACTION (Secretariat) to update Guide Part II 2.7.2.6 (planned outage wording; fix section cross-reference)
- [ ] ACTION (@6a6d74) to move "per-component operational criteria" from Guide Part II 2.7.2.9 to an Annex, focusing on Global Broker and Global Cache
- [ ] ACTION (Secretariat) to amend INFCOM-4 paper to introduce SC/KPI concepts and note upcoming Sensor Centres/KPIs for SCGDC, SCGM, SCGREP
- [ ] ACTION (@tomkralidis) to further develop GDC assessment methodology and KPIs (post-INFCOM-4) — see [#62](https://github.com/wmo-im/et-w2it/issues/62)
- [ ] ACTION (@shirley-xuelei, @elgarraichemseddine) to develop a Global Monitor performance dashboard and KPI proposal — see [#63](https://github.com/wmo-im/et-w2it/issues/63)
- [ ] ACTION (@tomkralidis, @6a6d74) to develop SCGREP proposals and Global Replay assessment methodology/KPIs — see [#64](https://github.com/wmo-im/et-w2it/issues/64)
- [ ] ACTION (@elgarraichemseddine, @shirley-xuelei) to develop a Global Monitor dashboard for Sensor Centre metrics end-point health — see [#65](https://github.com/wmo-im/et-w2it/issues/65)
- [ ] ACTION (TBC) to update "per-component operational criteria" for SCGDC, SCGM, SCGREP, and Sensor Centres — see [#66](https://github.com/wmo-im/et-w2it/issues/66)
- [ ] ACTION (@tomkralidis) to push WME event types into the WMO Codes Registry and draft Guide updates on Monitoring


### 5. (Other) Updates to Technical Regulation and Cookbook

- [ ] ACTION (Secretariat) to progress recommendation to move technical standards (WCMP2, WNM, WTH) to a Manual, and resolve references as Appendices in Manual on WIS
- [ ] ACTION (@tomkralidis) to lead progress on publication of service metadata, including developing exemplars
- [ ] ACTION (@hhaddouch) to follow up with Secretariat/Yuki to motivate conclusion of TT-NWPMD best practices activity for NWP data

#### 5.3 Duplicate data-id

- [x] ACTION (@tomkralidis) to replace Recommendation 1 with a recommendation to start data-id with the WCMP2 metadata-id — complete
- [x] ACTION (@6a6d74) to create a new issue on Global Broker "message storm" / WNM message ID retention — complete ([#61](https://github.com/wmo-im/et-w2it/issues/61))

**Tracking duplicate data-id fixes:**
- [ ] jp-jma-gts-to-wis2 — @ktsuboi-jms
- [ ] de-dwd-gts-to-wis2 — @kaiwirt
- [x] ca-eccc-msc — @tomkralidis (complete)
- [ ] wis2box — @tomkralidis
- [ ] IBL — @josusky

**Aligning WNM message ID retention period at 2 hours across all Global Brokers:**
- [ ] ACTION (@golfvert) — implement at Global Broker France
- [ ] ACTION (@JMauror) — implement at Global Broker Brazil
- [ ] ACTION (@solson-nws) — implement at Global Broker USA
- [ ] ACTION (@shirley-xuelei) — implement at Global Broker China

### 6. Release logistics

- [ ] ACTION (@hhaddouch) to inform @amilan17 (re: FAST TRACK release schedule)
- [ ] ACTION (@elgarraichemseddine, @shirley-xuelei) to create and publish a new dashboard for the new GC metrics
- [ ] ACTION (@elgarraichemseddine, @shirley-xuelei) to update `alerts.yml` for Global Cache to use amended metrics
- [x] ACTION (@tomkralidis) to cut new Cookbook release (1.1.0) ready for final review — complete

### 7. INFCOM-4 papers

- [ ] ACTION (@hhaddouch) to consider proposed [text on Sensor Centres](https://github.com/wmo-im/et-w2it/issues/38#issuecomment-4613477956) for inclusion in the INFCOM-4 Information paper (Sensor Centres section)

### 8. Any other business

- [ ] ACTION (@kay-goranlee52) to share KMA's GRep access details / service URL
- [ ] ACTION (@tomkralidis) to coordinate with South Korea to compare GRep functionality/performance, targeting mid-September testing
- [ ] ACTION (Secretariat) to coordinate and identify internal WMO opportunities to help deliver a WIS2 portal
- [ ] ACTION (ET-W2IT) to provide feedback on the Community Page to Secretariat
- [ ] ACTION (Secretariat) to build the "global service health status" dashboard on the Community Page
- [ ] ACTION (@solson-nws) to lead a collaborative Global Cache response on storing updated resources, engage Alberto (Secretariat) on WIS2-Downloader, propose WNM spec changes
- [ ] ACTION (Secretariat) to develop and propose options for improving the FAST TRACK review process
- [x] ACTION (Rémy) to update Guide 2.7.2.2 to specify "no less than 16" parallel downloads — complete

----

## 1.Opening

Opening comments from Director General, INMET, WMO Secretariat (@efucile), Chair SC-IMT (@golfvert), and Chair ET-W2IT (@6a6d74).
Tour-de-table to introduce all participants.
Working arrangements for the meeting were agreed. 

## 2.Designation and decommissioning procedures for WIS2 services

### 2.1.i Task: Review / amend / approve draft proposals for Global Services designation procedures. This should include clauses on suspension / revocation of designation due to poor performance.

#### Summary

Review, amend, and approve draft proposals for Global Services designation procedures ([here](https://wmoomm.sharepoint.com/:w:/s/INFCOMWorkspace/IQAmai3yiVoQS5fqs0o3pm6uAXI947RQ2i-OFbMYDsjNGhA?e=lNefA0)), including clauses on suspension/revocation of designation due to poor performance.

**Issue:** [Issue wmo-im/et-w2it#28: Create process for registering WIS2 Services](https://github.com/wmo-im/et-w2it/issues/28).

#### Discussion

**Who can operate a Global Service**

@JMauror asked who can operate a Global Service. @golfvert confirmed any Member may apply (Manual 2.6.3.1), subject to minimum performance criteria.

**Purpose of suspension/revocation**

Suspension/revocation exists to protect WIS2 as a whole, not to punish WIS Centres; the best outcome is performance improvement, supported where possible. @kaiwirt flagged revocation as the biggest sensitivity, and suggested ensuring Members understand the implications, with emphasis on the support provided during suspension (+1 from @josusky). @golfvert noted the Manual and Guide already describe this clearly. @josusky recalled that WIS1 had an audit process with potential revocation, though it didn't work in practice; @golfvert noted that audit existed but the consequences of failing were never explicit.

**Number of Global Service instances**

@kaiwirt raised the need to discuss how many instances of each Global Service are needed, to avoid the burden of too many instances. @golfvert agreed exact numbers are hard to specify, but supported ongoing discussion (+1 from @hhaddouch). Agreed to add a sentence to the draft designation procedures noting the need to balance overall WIS2 performance against offers of additional Global Service instances, given the added overhead. @kaiwirt suggested referencing this in the Manual too.

Add new paragraph to proposed draft of Manual 2.6.3.2:

> There is an optimal number of instances for each Global Service type: sufficient to support resilience, but not so many that duplicate messages from additional instances adversely affect overall performance. Each service offer will therefore be considered carefully in light of the performance of WIS2 as a whole.


**Duration of service commitments**

@davidpodeur asked whether there's a limit on the duration of a service commitment. @hhaddouch noted the Guide specifies no duration, but does include a decommissioning process. @golfvert noted no commitment should be indefinite — Météo-France's service offer specifies a 4-year commitment. @davidpodeur suggested, as an alternative to removing poor performers, simply not renewing at the end of a commitment period. @hhaddouch flagged the risk of WIS2 being exposed to poor performance for an extended period under that approach. @tomkralidis questioned whether fixed terms and renewals would create administrative fatigue. @hhaddouch expressed a preference for long-term commitments combined with an option for decommissioning; @golfvert agreed, favouring not disturbing the existing arrangement unnecessarily. Agreed: long-term commitments with an option for decommissioning.

@hhaddouch flagged the need to avoid last-minute changes to provision of services. @6a6d74 asked whether the decommissioning process includes a lead time. Decision: no fixed lead time; the process instead involves discussion with the Secretariat, through which a reasonable transition period is agreed.

**Revocation process for Global Brokers**

@davidpodeur noted the revocation process is clear, but for a Global Broker, subscribers need to be informed. This is an internal Secretariat process; no documentation change needed.

**Ongoing engagement with operators**

@solson-nws asked whether the Secretariat or SC-IMT should periodically check in with Global Service operators on their future commitment. WISOP was deemed sufficient, alongside continuous (monthly) engagement to assess commitment to the service offer.

**Governance level for GRep and other value-added services**

Discussion on whether GRep should require the same governance as the core Global Services (GB, GC, GDC, GM), and whether GRep is just one of potentially several "value-added" Global Services (e.g. a WDQMS-like service for RBON), with reference to Manual 2.6.1.1.

- @golfvert questioned the need to complicate matters. @hhaddouch noted Sensor Centres are different, but these value-added services matter to all users. @kaiwirt cautioned against creating first-class and second-class Global Services — a single governance process should apply.
- @golfvert raised whether this would require new Manual sections for "Other Global Services," and expressed concern that GRep isn't part of the core architecture and shouldn't be treated as such. He proposed using the same approval procedure for Global Services, but not including GRep in the Manual — instead referencing it from Guide Part III, Section 3.2 ("Other services"), listed separately from the "core" Global Services.
- @efucile suggested keeping a copy of the designation process in the Guide rather than referring back to the Manual. @golfvert disagreed but accepted this position.
- @hhaddouch and @kaiwirt argued that if it functions like a Global Service, it should be treated as one and listed in the Manual.
- @tomkralidis suggested following @golfvert's approach for now, with the option to add to the Manual later.
- @efucile felt adding GRep to the Manual would give the impression that WIS2 is in continual evolution, which isn't desirable — though acknowledged the team may need to admit the Global Replay Service was missed in the original architecture.
- @golfvert noted that making GRep part of the core architecture would require substantial documentation and technical work (Manual changes, new tests/scripts per the Global Services testing procedure, new WIS TechSpec, etc.), and questioned the benefit given limited expert team resources.
- @golfvert, @kaiwirt, @tomkralidis, @efucile, and @6a6d74 took this offline to reach a decision.

The offline decision concluded that Other Global Services (e.g., GRep) and Sensor Centres would be described in the Guide. The Manual would be updated only to mention that these categories of service exist (see below).

**Outcome on core vs. other services**

GB, GC, GDC, and GM are essential to WIS2's operation; WIS2 is improved by GRep but still functions without it. Manual 4.1.1 refers to four core services as WIS2's foundation, with "Other Services" building on top. The group considered whether Members might be reluctant to operate "2nd-tier" services, and whether a lower approval/operation threshold for Other Services could mitigate this. @golfvert advised not to disturb the foundation, building on top of it instead, and cautioned against overloading the Manual. @tomkralidis raised the challenge of "selling" operation of a 2nd-tier service to MSC/ECCC management.

Proposal: Other Services are described in the Guide, not the Manual, and carry a slightly less onerous threshold for approval and operation. Agreed that Section 3.2 could be subdivided into Global and Regional sections in future to give more emphasis to Other Services with global scope, and that the decision to keep Other Global Services out of the Manual can be revisited later. Future Other Services may include metadata management and archive services, among others.

**Decision**

Remove references to GRep and Sensor Centre from the new Manual Section 2.6 (Procedure for the Designation of a WIS 2.0 Global Service). In Guide Part III, Section 3.2 (Other Services), copy and adapt the Global Services designation procedure from the Manual, with necessary changes (e.g. the list of Other Services will not appear in Manual Appendix C). It should be made clear that the Other Services performance validation/suspension/revocation process is based on the Manual process.

Add a sentence to the Manual noting the value of Other Services and Sensor Centres — for example, that they are valuable components of the WIS2 ecosystem extending its utility and effectiveness, with further description in Guide Part III. In Manual Section 3.2 (Functional Architecture of WIS), add new sections 3.2.15 (Other Services, citing GRep as a specific example) and 3.2.16 (Sensor Centre); the existing 3.2.15 (GISCs) becomes 3.2.17.

Sensor Centre designation process remains distinct and will be listed in Guide Part III, Section 3.3.

**Listing of Other Services and Sensor Centres**

@6a6d74 asked where Other Services and Sensor Centres would be listed, given they won't appear in the Manual Appendix. @hhaddouch and @efucile confirmed the Secretariat will maintain and publish a list outside the Tech Regs; only the four core services appear in the Manual.

**Technical validation and operational assessment**

- Technical validation criteria (Manual 2.6.4.2, items A–E): @golfvert confirmed this reflects current Global Services testing practice. Agreed: no change required.
- SC-IMT performing technical validation (2.6.4.1) and operational assessment (2.6.5.1): @efucile noted “Standing Committee“ is used because sub-teams can't be named individually. Agreed: no change required.

**Experimental marking**

Regarding experimental marking during operational assessment (Manual 2.6.5.2) when connected to the WIS2 ecosystem: proposal to amend Manual 2.6.5.2 to indicate that a centre-id in the Code Registry would be marked as "experimental" during this phase.

**Suspension/revocation timelines and KPI evaluation**

Discussion on suspension after 3 months of sub-standard performance (Manual 2.7.2.2) and revocation after 6 months (2.7.2.3), noting that sub-standard performance need not be consecutive — just 3 or 6 months within a 12-month period, with KPI performance evaluated monthly (12 values per year).

- @davidpodeur stressed the KPI calculation must account for systemic problems (e.g. a global internet outage) outside a provider's control. @hhaddouch confirmed this is already covered and not automatic.
- @josusky asked when these Tech Regs provisions would be enforced. @efucile noted the change requires EC Resolution approval, which can clarify the start date. @golfvert proposed counting from January 2027, with enforcement starting from a later date specified in the EC resolution. @kaiwirt could accept this in principle, but would prefer to avoid a single 2-day problem/outage affecting KPI scores for 2 months. @6a6d74 noted such a situation might trigger the suspension process, but dialogue with the Secretariat/SC-IMT would establish it as an exceptional circumstance.
- Proposal: add to Manual 2.8.2.1 a statement that WMO Secretariat shall engage with the operating Member about incidents to determine the course of action, and will notify SC-IMT and GISCs. ET-W2IT explicitly agreed.

**Other confirmations**

- Revocation is a decision of the EC or Congress (Manual 2.9.3.2): confirmed.
- Members may reapply after a revoked designation (Manual 2.9.4.2): confirmed.

#### Next Steps

- [ ] ACTION (@hhaddouch) to update the Manual to reference the balance between overall WIS2 performance and additional Global Service instances. Add the following paragraph to Manual 2.6.2.3:

> There is an optimal number of instances for each Global Service type: sufficient to support resilience, but not so many that duplicate messages from additional instances adversely affect overall performance. Each service offer will therefore be considered carefully in light of the performance of WIS2 as a whole.

- [x] ACTION (@tomkralidis) to draft new Manual text for Other Services and Sensor Centre sections (3.2.15, 3.2.16). This action is complete (see [commit 7b2095d](https://github.com/wmo-im/wis2-manual/commit/7b2095d2563403e5f2ca73da81e99299120eb152)).
- [x] ACTION (@6a6d74) to draft the Other Services designation process. This action is complete (see [commit 0080d08](https://github.com/wmo-im/wis2-guide/commit/0080d081c4902f8d5701e58867b11afe248497eb)).
- [ ] ACTION (@hhaddouch) to amend Manual 2.6.5.2 to introduce "experimental marking" for centre-id in the Code Registry during operational assessment
- [x] ACTION (@hhaddouch) to add a statement to Manual 2.8.2.1 on WMO Secretariat engagement with operating Members regarding incidents. This action is complete. New text reads:

> [...] the WMO Secretariat shall engage with the operating Member about the incidents to determine the course of the action and will notify SC-IMT and the GISCs.

- [x] ACTION (@tomkralidis) to move "General" from Guide 2.7.2.4 to 2.7.2.1. This action is complete (see [commit 0080d08](https://github.com/wmo-im/wis2-guide/commit/0080d081c4902f8d5701e58867b11afe248497eb)).


### 2.1.ii Task: Review / amend / approve draft proposals for Sensor Centre designation procedures.

#### Summary

Review, amend, and approve draft proposals for Sensor Centre designation procedures. See [original draft](https://wmoomm.sharepoint.com/:w:/s/INFCOMWorkspace/IQDH7FNJQO-NQ52gWB2stqzlAeZ2zD4B5R4frrBw1iM_Hfs?e=odNVY9) and [updated proposal](https://github.com/wmo-im/et-w2it/issues/28#issuecomment-4615103774).

**Issue:** [Issue wmo-im/et-w2it#28: Create process for registering WIS2 Services](https://github.com/wmo-im/et-w2it/issues/28).

#### Discussion

- @golfvert proposed keeping things simple for Sensor Centres by not addressing suspension and revocation of designation for these. Agreed.
- ET-W2IT agreed the designation process should be consistent across all Additional Components: Other Global Services and Sensor Centres.
- @shirley-xuelei raised a concern about Members who operate both a Sensor Centre and a Global Service, where monitoring one's own performance could result in artificially favourable measurements. @6a6d74 responded that there will be multiple instances of Sensor Centres, allowing the performance of Global Services to be monitored from different locations.

**Sensor Centre lifecycle**

- Idea stage: a Sensor Centre can be implemented and run with no authority needed.
- Increased visibility: publish a Cookbook recipe for the Sensor Centre, including its specification.
- Official (WIS2) status: the Sensor Centre is recognised as a valuable contribution to the WIS2 ecosystem; its Cookbook recipe is promoted to the Guide; a designation process is required, with GISCs performing the assessment; metrics are harvested by Global Monitors to inform dashboards.
- Other authorities may impose their own governance and assessment requirements.

**Designation process**

- Applies only to "official" Sensor Centres listed in the Guide that are considered a valuable contribution to the WIS2 ecosystem, such as those contributing to KPI evaluation for monitoring Global Service performance.
- Proposed wording: "We welcome proposals for new Sensor Centres that contribute to the monitoring of WIS2 functions. Proposals should be made to the Secretariat who will coordinate evaluation and development of the proposal with SC-IMT."
- Assessment of "official" Sensor Centres is carried out by the GISC in coordination with SC-IMT.

@6a6d74 updated the Sensor Centre designation procedure — see [proposed text](https://github.com/wmo-im/et-w2it/issues/28#issuecomment-4654652221) and [commit 0080d08](https://github.com/wmo-im/wis2-guide/commit/0080d081c4902f8d5701e58867b11afe248497eb).

#### Next Steps

- [ ] ACTION (@tomkralidis) to consider updating/complementing the [global-service-type code list](http://codes.wmo.int/wis/global-service-type) to include Sensor Centre Types and Other Services

### 2.2 Task: Review / amend / approve update to DCPC designation procedure.

#### Summary

Review, amend, and approve the [update to the DCPC designation procedure](https://wmoomm.sharepoint.com/:w:/s/INFCOMWorkspace/IQDvf7Qi3QwPS7F2l4sa65oIAWKZepHLecedC5tobfNa4lc?e=e2qQkE).

#### Discussion

ET—W2IT reviewed the proposed changes which focus only on giving p/INFCOM the lead role in the designation process. 

#### Outcome

Agreed that DCPC designation will always require p/INFCOM approval. This change applies only to new designations; existing DCPCs will need to migrate to WIS2 Nodes as part of the transition, in the same way as National Centres.

#### Next Steps

- [x] ACTION (@kaiwirt) to change clause 2.3.4 of the [DCPC designation procedure](https://wmo-im.github.io/wis2-manual/manual/wis2-manual-APPROVED.html#_2_3_procedure_for_designating_a_data_collection_or_production_centre) to refer to "operating a WIS2 Node" instead of "DCPC capabilities”. This action is complete - see this [commit](https://github.com/wmo-im/wis2-manual/commit/7b2095d2563403e5f2ca73da81e99299120eb152).
- [x] ACTION (Secretariat) to change the DCPC designation process to require approval only from p/INFCOM. This action is complete.

### 2.3 Task: Review / amend / approve draft for performance management of GISCs.

#### Summary

Review, amend, and approve the [draft](https://wmoomm.sharepoint.com/:w:/s/INFCOMWorkspace/IQCwmmcf9nRlS5eWjGoWtCs-AToUi9af97dxtZUfi2qzO8E?e=2AFXp9) for performance management of GISCs.

#### Outcome

Agreed.

### 2.4 Task: Agree whether to provide information on decommissioning RTHs to INFCOM-4; if so, how? 

#### Summary

Agree whether to provide information on decommissioning RTHs to INFCOM-4, and if so, how.

**Issue:** [wmo-im/et-w2it#50](https://github.com/wmo-im/et-w2it/issues/50)

#### Discussion

- @golfvert noted that RTHs are a function of the GTS, and will disappear along with the GTS itself. The procedure for stopping an RTH is already listed in the Transition Guide.
- @hhaddouch felt now is not the time to provide this information in response to the EC-78 resolution, suggesting it wait until the transition is more advanced.
- @6a6d74 raised whether the Secretariat should ask Argentina what is missing from the Transition Guide — this was declined, on the basis of not wanting to draw unnecessary attention to the matter.
- @golfvert proposed a single line or side-note in the p/INFCOM report to INFCOM-4, noting the procedure is already in the Transition Guide, placed adjacent to the report that Chile (and possibly Belize) have completed their migration.

#### Next Steps

- [ ] ACTION (Secretariat) to add a brief note about decommissioning / phasing-out RTHs into the INFCOM-4 report referencing the Transition Guide, alongside the migration status update for Chile (and possibly Belize).

## 3.Performance measures and monitoring for WIS2 services

### 3.1 Task: Agree thresholds for corrective action (e.g., alerts, warnings) and KPIs for long-term performance assessment of GISC, Global Broker, Global Cache, and Global Discovery Catalogue.

#### Summary
Defining the assessment methodology and KPIs for WIS2 Components:

- Global Broker
- Global Cache
- Global Discovery Catalogue
- Global Monitor
- Additional Components: Other services (GRep) & Sensor Centre

Related Issues:

- [Issue wmo-im/et-w2it#23: Objective (under-)performance measures need to be defined in the Guide […]](https://github.com/wmo-im/wis2-guide/issues/23)
- [Issue wmo-im/et-w2it#39: […] set thresholds for corrective action and KPIs for long-term performance assessment](https://github.com/wmo-im/et-w2it/issues/39)
- [Issue wmo-im/et-w2it#43: Monitor the performance of the Global Services […]](https://github.com/wmo-im/et-w2it/issues/43)

#### Discussion
**Timeline?**

Previously ET-W2IT suggested defining the KPI concept for INFCOM-4 and setting the KPI values later once (meta)data is flowing. Is this still the preferred approach?
@6a6d74 > Based on earlier discussion, should we publish the KPIs yet?
@golfvert > We need to define these KPIs now - else it will be a long time before we have another opportunity and even longer before we start the measurement.
Agree: now is the time to define the KPIs.

**Over-arching Assessment Methodology**

ET-W2IT reviewed the proposed text for the [Guide Part II 2.7.2.6 Assessment methodology](https://wmo-im.github.io/wis2-guide/guide/infcom/guide/wis2-guide-DRAFT-INFCOM-4.html#_2_7_2_6_assessment_methodology). This describes the assessment methodology and is deliberately high-level.
@kaiwirt > this provides sufficient description of how the monthly KPI is calculated 
@golfvert > We need to write the details of KPIs somewhere - maybe [Guide Part II 2.7.2.9 Per-component operational criteria](https://wmo-im.github.io/wis2-guide/guide/infcom/guide/wis2-guide-DRAFT-INFCOM-4.html#_2_7_2_9_per_component_operational_criteria) is not the right place? We need: 

- What we measure
- How we measure it
- What is good/bad performance

@josusky > given that this could be used to remove designation, it needs to be in an official document
@golfvert, @hhaddouch > Annex to the Guide
Agreed. KPIs will be published in an Annex in the Guide.

Note: 98% uptime = 14.4h per month. 98% uptime excludes _planned outages_
@golfvert > why 98%? Starting with Global Caches. At any given time (99.99%) we need at least 3 GCs operating… so with 6 GCs this means individual GCs at 98%.

**Planned outages**

@tbuessel > 4-hours per month scheduled maintenance (See [Guide Part II 2.7.2.6 Assessment methodology](https://wmo-im.github.io/wis2-guide/guide/infcom/guide/wis2-guide-DRAFT-INFCOM-4.html#_2_7_2_6_assessment_methodology)) is too short.
@golfvert > MSS has been out for minutes only - why should Global Service be any worse?
@kaiwirt > if you exceed threshold for scheduled maintenance - that is only one of three months needed to trigger suspension process.
@kaiwirt > there’s also the additional clause about discussing with Secretariat any extraordinary issues (e.g., major security alert). It’s not a (completely) automated process - it recognises that there are some things outside the control of the Service operator.
@kaiwirt > need to balance risk of hacking against risk of service downtime - in some situations, it makes sense to turn off the operational service until fixed. But then this is only [one strike in three] 
@hhaddouch > There will always be exceptions - force majeur (e.g., earthquake).
@kaiwirt > The Guide should distinguish between planned and unplanned outages.
@josusky > WIS2 risks are different to GTS - GTS was private network; WIS2 is internet facing.
@kaiwirt > should also coordinate planned maintenance to avoid clashing with outage from another Global Service instance.

**Global Cache**

Related: see [wmo-im/wis2-operation#53](https://github.com/wmo-im/wis2-operation/issues/53) for WISOP discussion on KPIs and [wmo-im/wis2-operation#48](https://github.com/wmo-im/wis2-operation/issues/48) for the details.

Measure (calculated each hour):

1. Percentage of data items published by the Global Cache compared with total number of data items published by all WIS2 Nodes (on `origin` topics): SLA = 95% of data items must be cached. Cross-reference between Global Cache and origin based on compound key of `data-id` + `pubtime` + (if available) checksum. HTTP HEAD request on URLs to check data items are actually available from the Global Cache's download server. Messages where `cache=false` are excluded.
2. Successful download from the GC, including validation of data integrity (if checksum available in message); based on a sample set (200 randomly selected data items each hour; same set for all GCs) must be successfully downloaded: SLA = 95% of sample set is downloaded.

KPI evaluation: 

- Each hour, the KPI value is set to "pass" for a Global Cache if both number of data items cached >= 95% (compared to origin) AND number of successful downloads >= 95%, else KPI is set to "fail" for the hour.
- Hourly KPI evaluation is based on the best result from all Sensor Centre Global Cache instances - KPIs are calculated at the Global Monitor not the Sensor Centre itself.
- Each month, the overall KPI is set to "pass" if the hourly KPI passes >= 98% (i.e., the Global Cache may experience 14 "failure" hours in one month and still be considered performing OK).
- Hours coinciding with planned outages (or other "force majeur") agreed by SC-IMT are excluded from the monthly KPI calculation.
- Monthly KPI used in the assessment of Global Cache performance.

A sample set of 200 messages is used to avoid overloading both Global Caches and Sensor Centres.

**Issue:**
There is a valid concern that testing the download for a data item that a Global Cache had failed to cache would result in a double-count against its performance (with a sample-size of 200, only 10 messages can fail to download before the hourly SLA is breached; it’s possible that all 10 of these could be missed messages) - and it wouldn’t be a true assessment of the operation of the download server. It would be better to assess downloads using a sample from the list of data items cached by all Global Caches. However, if one Global Cache instance was offline for part or all of the hour (e.g., for maintenance) then the number of data items downloaded by _all_ Global Caches could be zero.

**Post-meeting note on robust measurement of Global Cache download performance:** @golfvert considered this further and updated the methodology as follows:
Every minute select maximum of 5 data items that have been cached by all Global Caches (less than 5 data items may be cached by all Global Caches; worst case is a Global Cache is offline and the number is zero). Increment `wmo_wis2_scgc_download_selected_total` by the number of selected data items. Attempt to download these data items from all Global Caches. For each Global Cache increment `wmo_wis2_scgc_download_successful_total` on each successful download (and, if available, checksum evaluation). Evaluate the hourly successful downloads KPI. If `wmo_wis2_scgc_download_selected_total` is zero for the previous hour, the successful downloads KPI cannot be calculated: automatically set the KPI to "pass" for all Global Caches. Else evaluate the KPI as `wmo_wis2_scgc_download_successful_total` / `wmo_wis2_scgc_download_selected_total`. The Global Cache that is offline for the hour will always fail the cached data items KPI (they’re offline - they won’t have cached anything!), so the compound KPI of cached data items KPI + successful downloads KPI will always be “fail”.        

**Issue:** 
By design Global Caches discard out-of-sequence updates. Discarded updates would be seen as a “miss”. These misses should not affect the KPI calculation.
Propose that the KPI for Global Cache performance is calculated based only on messages with `rel=canonical`. Agreed. 
Given that metrics for “update” messages remain useful in diagnosing Global Cache behaviour, suggest adding the WNM message link-relation (`rel`) type as a label in the SCGC metrics. This way, metrics related to canonical and update messages can be easily separated out.

ET-W2IT approved both the assessment methodology (subject to changes above) and the KPI threshold values for Global Cache performance monitoring. 

**Global Broker**

Measure (calculated each hour):

1. Percentage of WNM messages published by the Global Broker within cut-off time (60-seconds) compared to “baseline”, assessed using a randomised sample of approximately 10% of messages.

Randomised sample based value of message-id (UUIDs follow a predicable pattern so some bytes, or hex digits, of the UUID can be treated as a uniformly distributed random number; selecting a range of these random numbers gives a randomised sample). Only 10% of messages are checked to keep the workload of a Sensor Centre Global Broker at a manageable level.

The “baseline” is the highest number of messages published by any Global Broker, as recorded by any Sensor Centre Global Broker. 

Cut-off time is 60-seconds: a message is considered “missed” if a Global Broker has not published a that message 60-seconds after it was first published by any other Global Broker. 60-seconds cut-off is semi-arbitrary; analysis of message flows indicates that the vast majority of messages are normally published within this time. 

For each Sensor Centre instance, the workflow is as follows:

1. Evaluate UUID of message (message-id). Is UUID in randomised sample group?
   1. No: Discard this message (outside sample range)
   2. Yes: Has message with this UUID already been seen from another Global Broker?
      1. No: Store the `message-id` + timestamp (time message received) in SCGB database. Increment the `wmo_wis2_scgb_messages_published_total` metric for the Global Broker that published the message
      2. Yes: Is the timestamp for this message older than 60-seconds?
         1. No: Increment the `wmo_wis2_scgb_messages_published_total` metric for the Global Broker that published the message (received within cut-off time)
         2. Yes: Discard message, do not increment `wmo_wis2_scgb_messages_published_total` for the Global Broker that published the message (received after cut-off time - considered a "miss")

Sensor Centre Global Broker should store the identifiers of messages received for a minimum of 2-hours so that it doesn’t “forget” that it has already seen messages.

KPI evaluation:

- Each hour, the KPI value is set of "pass" if number of messages published >= 95% (compared to baseline), else KPI is set to "fail" for the hour.
- "Baseline" is the highest number of messages published by any Global Broker within the previous hour.
- Hourly KPI evaluation is based on the best result from all Sensor Centre Global Broker instances - KPIs are calculated at the Global Monitor not the Sensor Centre itself.
- Each month, the overall KPI is set to "pass" if the hourly KPI passes >= 98% (i.e., the Global Broker may experience 14 "failure" hours in one month and still be considered performing OK).
- Hours coinciding with planned outages (or other "force majeur") agreed by SC-IMT are excluded from the monthly KPI calculation.
- Monthly KPI used in the assessment of Global Broker performance.

ET-W2IT approved both the assessment methodology and the KPI threshold values for Global Broker performance monitoring.

**Global Discovery Catalogue**

Current implementation of the Sensor Centre Global Discovery Catalogue focuses on observing consistency of discovery metadata holdings between Global Discovery Catalogues. The consistency evaluation is proposed as follows:

- evaluation daily, based on the metadata record archive published by each GDC.
- ignore number invalid records (these would have been valid at the time of ingest) - these still count towards the total number of records and should be consistent.
- \# total records = highest number of records held by any GDC.
- \# consistent records = number of records that match with the same record in other GDCs.
- where inconsistency is found, the "correct" record is the one with latest update time (if no update time included in any version of the record, mark the record as inconsistent for all GDCs).
- 10 records inconsistent would be 98% consistency.
- KPI could be: %consistent = (# consistent records / # total records)x100.
- Evaluated on a daily basis - one failure would give a 97% pass - suugest the monthly aggregate KPI is 95%.

**Issue:** 
Each GDC may receive and ingest WCMP2 records at slightly different times and/or the GDCs may publish their archives at different times each day. This may lead to “race conditions” where different GDC archives have slightly different sets of records. Consequently, a KPI of 100% consistent records is not appropriate. Options include: (1) coordinate when GDCs publish their archives, (2) ignore the archive for consistency checking - query the GDC API directly.

Further work is required to assess “operational performance” of Global Discovery Catalogue instances - e.g., the performance of the search API end-point. @golfvert also worries about the different nature of the static checks (records consistency) and the dynamic checks about API performance.

ET-W2IT agree that the assessment methodology and KPIs for Global Discovery Catalogue is incomplete. Rather than rushing this and publishing something un-tested and/or ill-considered, ET-W2IT agree to defer inclusion of the performance assessment methodology for GDCs into the Guide until after INFCOM-4. @golfvert adds that we should keep the SCGDC section, but not include any performance assessment or KPI parts for GDC.

**Global Monitor**

No assessment methodology had yet been developed for the Global Monitor. @shirley-xuelei noted that it is difficult to judge if dashboard content is correct. @golfvert suggested a KPI on automated provision of Monitoring Event messages and/or JIRA tickets. @6a6d74 suggested measuring up-time of the Grafana dashboard. @golfvert proposed creating a dashboard for assessment by KPI - and routinely test the correct availability of this dashboard. This would (should) also test that the metrics from Global Services are being properly collected. @hhaddouch noted that the Global Monitor is used daily by GISC Watch - they could report issues arising from their use, and record issues for the KPI reporting. However, @davidpodeur points out this would be ineffective given that GISC Watch typically use dashboards from only a single Global Monitor.

ET-W2IT agree to defer provision of the assessment methodology and KPIs for Global Monitor until after INFCOM-4.

**Global Replay** 

No assessment methodology had yet been developed for the Global Monitor. @tomkralidis offered to develop some proposals. @6a6d74 suggested the [GRep test client](https://github.com/wmo-im/wis2-champions/blob/main/Bali-workshop-MAR2026/GREP_TEST_CLIENT.md) ([github: 6a6d74/mqtt-subscriber-web](https://github.com/6a6d74/mqtt-subscriber-web/blob/main/README.md)) as a potential basis for a Sensor Centre for GRep.

ET-W2IT agree to defer provision of the assessment methodology and KPIs for Global Replay until after INFCOM-4. 

**Sensor Centre**

No assessment methodology had yet been developed for the Sensor Centres.

@6a6d74 asked how to monitor Sensor Centres, e.g., a simple metrics end-point uptime check. 
Self-hosted options (which could be run in multiple locations) include:

- blackbox_exporter [github.com/prometheus/blackbox_exporter](https://github.com/prometheus/blackbox_exporter) - native part of the Prometheus project; allows blackbox probing of endpoints over HTTP, HTTPS, DNS, TCP, ICMP and gRPC; published OpenMetrics; no UI; docker deployment.
- Uptime Kuma "a fancy self-hosted monitoring tool" [uptimekuma.org](https://uptimekuma.org) - can monitor HTTP and HTTPS URLs, TCP Ports and HTTP(s) Keywords, HTTP and HTTPs JSON queries, Databases (etc.); broad set of features; UI components; docker deployment; open source.

@golfvert noted that these are not needed because the Global Monitors already connect to the Sensor Centres and could monitor the availability of the SC metrics end-point, and produce a dashboard accordingly.

Suggested assessment / KPI:

- SC producing correct metrics - what percentage of time?
- Metrics available at GMs 98% of time during a calendar month gives a "pass".

ET-W2IT agree to defer provision of the assessment methodology and KPIs for Sensor Centres until after INFCOM-4. 

**GISC**

See suggestions of KPIs for GISC performance here: https://github.com/wmo-im/et-w2it/issues/43#issuecomment-3645999691. ET-WISOP requested to develop proposals for GISC KPIs based on their experiences. **Post meeting note:** This was discussed during ET-WISOP meeting (11/12-JUN-2026).

**Overall**

@golfvert stated that he is mindful of the time/resource available to the Expert Team. The Global Broker and Global Cache are two most services to monitor the performance of - through the SCGB and SCGC - and evaluate KPIs. For INFCOM-4 we should introduce the concepts of SC, KPI, etc., include these operationally critical Sensor Centres & their KPIs - SCGB, SCGC - and identify that Sensor Centres and KPIs are coming soon for other services - SCGDC, SCGM, SCGREP, Sensor Centres.
Agreed. 

#### Outcomes
Performance assessment methodology and KPIs agreed for Global Broker and Global Cache. These will be included in the Guide for INFCOM-4. Assessment methodology and KPIs for other WIS2 components is deferred.

#### Next steps

**Relating to INFCOM-4**

- [ ] ACTION (@golfvert) to update the Sensor Centre Global Cache specification and implementation to add the link-relation type (either `canonical` or `update`) to the metrics as label "rel". Also update [wmo-im/wis2-metric-hierarchy `metrics/scgc.csv`](https://github.com/wmo-im/wis2-metric-hierarchy/blob/main/metrics/scgc.csv)
- [ ] ACTION (@golfvert) to confirm through further analysis that a 60-second cut-off time is the best choice for identifying "missed messages" in SCGB
- [ ] ACTION (@shirley-xuelei, @elgarraichemseddine) to port the SCGB and SCGC dashboards to the Global Monitors
- [ ] ACTION (Secretariat) to update [Guide Part II 2.7.2.6 Assessment methodology](https://wmo-im.github.io/wis2-guide/guide/infcom/guide/wis2-guide-DRAFT-INFCOM-4.html#_2_7_2_6_assessment_methodology): (1) regarding planned outage, to say something like "not exceed 4-hrs per calendar month planned outage unless by exception agreed with SC-IMT … and then restore within the agreed time-window"; (2) to fix a section cross-reference (the statement "The Global Service meets the service level for the calendar month where the proportion of operational time is not less than the value set out in section 2.7.2.5." appears to reference the wrong section; the correct reference may be 2.7.2.9, though this section on "per-component operational criteria" will become an Annex to the Guide)
- [ ] ACTION (@6a6d74) to update Guide Part II by re-writing/moving the "per-component operational criteria" descriptions from [Guide Part II 2.7.2.9 Per-component operational criteria](https://wmo-im.github.io/wis2-guide/guide/infcom/guide/wis2-guide-DRAFT-INFCOM-4.html#_2_7_2_9_per_component_operational_criteria) to an Annex to the Guide, focusing on Global Broker and Global Cache
- [ ] ACTION (Secretariat) to amend the INFCOM-4 paper to introduce the concepts of SC, KPI, etc., and the operationally critical Sensor Centres (and their KPIs) - SCGB, SCGC - and to note that Sensor Centres and KPIs are coming soon for other services - SCGDC, SCGM, SCGREP

**Not relating to INFCOM-4**

- [ ] ACTION (@tomkralidis) to further develop the assessment methodology and KPIs for Global Discovery Catalogue, for inclusion in the Guide after INFCOM-4, including "functional" metrics such as consistent API search queries against all GDC instances, where all GDCs should respond within a time-window and with the same results. See new Issue [wmo-im/et-w2it#62](https://github.com/wmo-im/et-w2it/issues/62).
- [ ] ACTION (@shirley-xuelei, @elgarraichemseddine) to develop a dashboard that could be used to automatically evaluate Global Monitor performance, and develop a proposal for a Global Monitor performance assessment methodology and KPIs. See new Issue [wmo-im/et-w2it#63](https://github.com/wmo-im/et-w2it/issues/63).
- [ ] ACTION (@tomkralidis, @6a6d74) to develop proposals for a Sensor Centre Global Replay (SCGREP) and associated assessment methodology and KPIs for Global Replay. See new Issue [wmo-im/et-w2it#64](https://github.com/wmo-im/et-w2it/issues/64).
- [ ] ACTION (@elgarraichemseddine, @shirley-xuelei) to develop a Global Monitor dashboard for Sensor Centre metrics end-point health (to evaluate monthly availability). See new Issue [wmo-im/et-w2it#65](https://github.com/wmo-im/et-w2it/issues/65).
- [ ] ACTION (TBC) to update "per-component operational criteria" for Global Discovery Catalogue / SCGDC, Global Monitor / SCGM, Global Replay / SCGREP, and Sensor Centres. See new Issue [wmo-im/et-w2it#66](https://github.com/wmo-im/et-w2it/issues/66).

### 3.X [Extra agenda item] Task: WME spec approval.

#### Summary

WME specification approval, including resolution of the sub-topics question.

#### Discussion

- @josusky raised the question of sub-topics (see [related discussion](https://github.com/wmo-im/wis2-guide/issues/233#issuecomment-4432887880)).
- @golfvert advocated for keeping things simple first, then adding sophistication later, noting no clear demand for server-side filtering across two separate systems handling different event types.
- @6a6d74 noted that since the WME spec was already changed to support wildcards in WME topic subscriptions, adding sub-topics later would be backward compatible. Given the aim to keep things simple for now, proposed not adding sub-topics to the WME spec at this time.
- Agreed.

#### Outcome

ET-W2IT approved the WME specification.

### 3.2 Task: Resolve outstanding issues relating to publication of monitoring event messages by Global Services.

#### Summary

Resolve outstanding issues relating to the publication of monitoring event messages by Global Services. See [outstanding sub-issues](https://github.com/wmo-im/wis2-guide/issues/233#issuecomment-4432900644).

**Issue:** [wmo-im/wis2-guide#233](https://github.com/wmo-im/wis2-guide/issues/233)

#### Discussion

Five outstanding sub-issues were addressed: naming convention for event types; which event types are required; severity per event type; the conditions (including frequency) under which Global Services create each event type; and the use of sub-topics for specific event types when publishing WME messages.

**Naming convention**

ET-W2IT agreed the naming convention should be resource-based rather than component-based (i.e. not referencing Cache, Broker, Catalogue, etc. directly).

**Sub-topics**

Resolved separately under the WME spec approval task.

**General principle**

A WME message should generally be published when an error condition occurs, which typically also increments an error metric. This applies to events of severity "error." As a rule of thumb, WME messages should be published under the same conditions that trigger an error metric increment.

**Payload specification**

The event JSON payload is lightly specified for now — a few properties are required, with the rest left to implementation choice. This is acceptable for now, with the possibility of tightening the specification later.

**Event types by component**

All WIS2 components: `int.wmo.wis.wme.event.maintenance` (Info) — published when a component shares planned maintenance, automatically created by the Global Monitor based on receipt of a JIRA ticket.

Global Broker: `int.wmo.wis.wme.event.wnm.validation.topic`, `int.wmo.wis.wme.event.wnm.validation.metadata`, and `int.wmo.wis.wme.event.wnm.validation.schema` (all Error). Some validations are currently Info/Warning where a spec change is upcoming or a best practice isn't being followed. @kaiwirt suggested simplifying to a single `int.wmo.wis.wme.event.wnm.validation` type; @golfvert cited a real user example (UKMO) wanting to filter on the more granular type. No WME message is published when `wmo_wis2_gb_connected_flag` is set to false for a component — that responsibility sits with the Global Monitor.

Sensor Centre Global Broker: none.

Global Cache: Download fail (Error), Integrity fail (Error), Content doesn't match download (Warning, optional?), Cache override (Info).

Sensor Centre Global Cache: `int.wmo.wis.wme.event.log` (Info).

Global Discovery Catalogue: Metadata download, Metadata archive, WCMP2 ETS (schema validation), WCMP2 KPI (KPI validation).

Sensor Centre Global Discovery Catalogue (SCGDC): none yet — a deployment is needed to test first; the generic `int.wmo.wis.wme.event` type can be used in the interim.

Global Monitor: Alerts and warnings based on the AlertManager YAML, each resulting in a WME message. More work is required to review these cases. Decision: WME messages published by the Global Monitor will not be defined for INFCOM-4 and will instead be added in a future FAST TRACK release. In the interim, the Global Monitor will use the generic `int.wmo.wis.wme.event` type.

Sensor Centre Global Monitor (SCGM), Global Replay Service, and Sensor Centre Global Replay Service (SCGREP): none.

The complete set of proposed WME event types is published in the [event-type codelist](https://github.com/wmo-im/wis2-monitoring-events-codelists/blob/main/codelists/event-type.csv).

#### Outcome

Publish the WME spec for INFCOM-4, and publish WME event types in the WMO Codes Registry. Update the Guide with high-level information about Monitoring for Global Service providers, plus a short addition to the WIS2 Node Technical Considerations explaining the use of Monitoring. Future updates may describe the specific conditions under which Global Services and Sensor Centres should publish WME messages, but the high-level, overarching statement is deemed sufficient for now.

#### Next Steps

- [ ] ACTION (@tomkralidis) to push WME event types into the WMO Codes Registry, and draft a changes to the Guide: high-level information about Monitoring for Global Service providers, plus a short addition to the WIS2 Node Technical Considerations explaining the use of Monitoring. 

### 3.3 Discussion.

Item not discussed. See Issue [wmo-im/et-w2it#56: Resource planning to support transition to WIS2 with resilient, performant Global Services](https://github.com/wmo-im/et-w2it/issues/56).

## 4.What next for WIS2?
### 4.1 Discussion

#### Discussion

Discussion curtailed due to lack of time. A broad range of topics were debated: aviation data, cessation of GTS data transmission (particularly in Chile), standardising the use of Web services in WIS2, how to support “AI-ready” (or “ARCO” analysis-ready, cloud-optimised) data, metadata publication service, archive service(s), harvesting discovery metadata from other catalogues (particularly the Global Cryosphere Watch catalogue). No specific outcomes or conclusions reached.

## 5.(Other) Updates to Technical Regulation and Cookbook:

### 5.X [additional agenda item] Discuss removing WCMP2, WNM, WTH from Manual and moving to Guide (or somewhere else)?

#### Summary

Discussion on removing WCMP2, WNM, and WTH from the Manual on WIS and relocating them — either to the Guide, a new "compendium of WIS2 technical standards," or the Manual on Codes.

#### Discussion

- @efucile explained that the Manual on WIS currently mixes governance and technical content, which is problematic since it forces both types of detail to be brought to Intergovernmental sessions of INFCOM. The objective is to separate technical standards out. The Manual on Codes already serves as a collection of format standards in one place. The Guide is not an acceptable destination, since Guides represent recommended practice only — these technical specifications must reside in a Manual. Two options were identified: a new Volume in the Manual on Codes (which still requires a change to WMO No. 49), or a new Manual entirely (more work, since it would need to be bound into the WMO No. 49 Technical Regulations). There is limited appetite within the Secretariat for creating a new Manual. @efucile also noted there will be a future technical standard for the First Mile.
- @6a6d74 noted that 99% of people will use the technical standards as published on GitHub regardless of where they formally sit. Semantically, WCMP2, WNM, and most of WME concern formats; WTH concerns topic hierarchies but is closely bound to WNM. These mostly would fit with the Manual on Codes, and also relate to data exchange.
- @golfvert expressed a preference for publishing the standards as individual technical standards, so Members who choose to use a given standard can refer to the relevant document directly. However, a new Volume in the Manual on Codes was accepted as a workable approach.
- @6a6d74 supported moving to another Manual as the path of least resistance. Agreed. @6a6d74 added that WME would follow wherever WCMP2, WNM, and WTH are relocated to.
- @golfvert noted there are some "shall" statements in the Guide that will need attention in the long run.
- @efucile will provide a recommendation to the EC, with the EC making the final decision.

#### Next Steps

- [ ] ACTION (Secretariat) to progress the recommendation to move the technical standards to a Manual (either new, or a new Volume of the Manual on Codes), and resolve all references to WCMP2, WNM, and WTH as Appendices in the Manual on WIS

### 5.1 Task: Agree if Sensor Centre and Global Replay service concepts should (or should not) be included in Manual on WIS2. If yes, draft new text.

#### Summary

Agree whether the Sensor Centre and Global Replay service concepts should be included in the Manual on WIS2, and if so, draft the relevant text.

**Context:** Sensor Centre and Global Replay are currently referenced in the updated Guide ([new Part 3](https://github.com/wmo-im/wis2-guide/blob/INFCOM-4/guide/sections/part3/index.adoc)), and in the [draft Global Services designation procedure](https://wmoomm.sharepoint.com/:w:/s/INFCOMWorkspace/IQAmai3yiVoQS5fqs0o3pm6uAXI947RQ2i-OFbMYDsjNGhA?e=0ZAIQB).

#### Outcome

Already agreed: Sensor Centre and other Global Services are mentioned briefly in the Manual. @tomkralidis has already added the relevant text at Manual sections 3.2.15 and 3.2.16. The remaining detail resides in the Guide.

### 5.2 Task: Review / amend / approve draft text for inclusion in the WIS2 Guide providing an overview of the Sensor Centre “ecosystem”.

#### Summary

Review, amend, and approve draft text for inclusion in the WIS2 Guide providing an overview of the Sensor Centre "ecosystem" (drafted by @6a6d74 ahead of the meeting).

**Issue:** [wmo-im/et-w2it#40](https://github.com/wmo-im/et-w2it/issues/40)

#### Discussion

The [first version](https://github.com/wmo-im/wis2-guide/pull/254/changes) was already discussed on Monday afternoon, with changes requested that have now been implemented (see `guide/sections/part3/sensor-centres.adoc` in this [commit](https://github.com/wmo-im/wis2-guide/commit/0080d081c4902f8d5701e58867b11afe248497eb)). ET-W2IT approved the text.

**On publishing WCMP2 records**

- Agreed to not include a requirement for Members to publish a WCMP2 service record for a Sensor Centre; this may instead be generated from the WIS2 Global Registry.
- @golfvert raised whether service records should start being added to the GDC.
- @tomkralidis noted the Global Registry is private and contains private information, but that TT-Metadata always intended to include service metadata in the GDC to help people find services.
- @golfvert suggested the first services to focus on would be Global Brokers and Global Caches, with WIS2 Nodes potentially also useful — even where a WIS2 Node isn't publicly accessible, a service record describing it would still have value.
- @6a6d74 noted that, as a minimum, all WIS Centres are listed in the centre-id code table, so at least the Member (country) running a given WIS component is identifiable.

#### Outcome

This approach for publishing service metadata would be useful. To be progressed after INFCOM-4.

#### Next Steps

- [ ] ACTION (@tomkralidis) to lead progress on publication of service metadata, including developing exemplars for service metadata records

### 5.3 Task: Agree amendments to data_id specification to remedy issues with (lack of) uniqueness.

#### Summary

Agree amendments to the `data_id` specification and/or remedial action to remedy issues with (lack of) uniqueness.

**Issue:** [wmo-im/wis2-notification-message#179](https://github.com/wmo-im/wis2-notification-message/issues/179)

#### Discussion

**Defining uniqueness**

- @kaiwirt noted WIS Centres interpret "unique" differently, and questioned whether a definition for how Members ensure data-id uniqueness is needed.
- @josusky suggested including the centre-id would ensure uniqueness between WIS Centres.
- @tomkralidis noted that wis2box already concatenates the WCMP2 metadata-id with the file name.
- @6a6d74 proposed this as the new recommendation: concatenate the WCMP2 metadata-id with the file name.
- @golfvert countered that people already struggle to make their file name unique, and suggested a UUID instead. @6a6d74 responded that file names are often used for internal purposes, so a UUID would be disruptive. @kaiwirt added that a UUID would be problematic for tracking updates. @tomkralidis noted the meaningful file name is useful for traceback to upstream systems.
- @golfvert pointed out the WNM spec already states `data_id` shall be unique within the scope of the dataset, which is implicitly equivalent to prepending the WCMP2 metadata-id — the issue is that people aren't reading the existing spec.
- @shirley-xuelei expressed a preference for a UUID.

**Operational approach**

- @golfvert proposed an alternative framing: leave the spec alone and treat this as an operational issue. The Sensor Centre can track duplicate data-id problems and raise JIRA tickets when seen, prompting the WIS2 Node to fix it. The most problematic centres are the GTS-to-WIS2 Gateways (Japan, Germany) and ECCC/MSC. Both wis2box and the IBL implementation are widely used, so focus should be on resolving current issues with existing implementations. Agreed.

**Recommendation 1 (opaque data-id)**

- @tomkralidis explained that WNM Recommendation 1 (favouring an opaque data-id) existed because there was previously no formal mechanism for client-side filtering, so people used the data-id for that purpose. Now that a client-side filtering mechanism exists, he suggested removing this recommendation, noting it would not be a breaking change.
- @josusky raised a concern, since people push data between systems.
- @6a6d74 clarified this is only the removal of a recommendation — the practice would still be permitted.
- Agreed to remove Recommendation 1, and replace it with a recommendation to start the data-id with the WCMP2 metadata-id.

**Uniqueness duration**

- @6a6d74 suggested a 24-hour uniqueness window. @tomkralidis and @josusky suggested mapping this instead to the retention period of the Global Replay service. @golfvert argued no spec update is needed: unique is unique. Agreed.

**WNM message ID**
- @golfvert noted that he had seen cases of “message storms” where Global Brokers seemed to publish new messages from nowhere. His analysis suggested that this was caused by some Global Brokers being slow to process a backlog of messages. Upon their publication, other Global Brokers had already forgotten that they had seen those message previously and republished them once again.  A test where two Global Brokers increased the duration of their message ID “memory” (i.e., retention period) seemed to remedy the problem. @golfvert suggested making the Global Broker WNM message ID retention period consistent across all Global Brokers, proposing 2 hours. Agreed.

#### Next Steps

-  Tracking implementation of fixes to duplicate data-id problem:
  - [ ] jp-jma-gts-to-wis2 @ktsuboi-jms
  - [ ] de-dwd-gts-to-wis2 @kaiwirt 
  - [x] ca-eccc-msc @tomkralidis 
  - [ ] wis2box @tomkralidis 
  - [ ] IBL @josusky 
- [x] ACTION (@tomkralidis) to replace Recommendation 1 with a recommendation to start the data-id with the WCMP2 metadata-id. This action is complete - see [PR wmo-im/wis2-notification-message#181](https://github.com/wmo-im/wis2-notification-message/pull/181)
- [x] ACTION (@6a6d74) Create a new issue about the Global Broker “message storm” and WNM message ID retention period. (Done: see https://github.com/wmo-im/et-w2it/issues/61)
- [ ] ACTION (Global Brokers) to align the WNM message ID retention period at 2 hours across all Global Brokers
  - [ ] ACTION (@golfvert) to implement retention period at Global Broker France
  - [ ] ACTION (@JMauror) to implement retention period at Global Broker Brazil
  - [ ] ACTION (@solson-nws) to implement retention period at Global Broker USA
  - [ ] ACTION (@shirley-xuelei) to implement retention period at Global Broker China

### 5.4 Task: Review / amend / approve update to Technical Considerations for the Global Monitor regarding automatic creation of WME message when JIRA “maintenance” ticket raised.

#### Summary

Review, amend, and approve update to Technical Considerations for the Global Monitor regarding automatic creation of a WME message when a JIRA "maintenance" ticket is raised.

**Issue:** [wmo-im/wis2-guide#148](https://github.com/wmo-im/wis2-guide/issues/148)

#### Outcome

Done. See [comment](https://github.com/wmo-im/wis2-guide/issues/148#issuecomment-4671087440) and [commit 5195830](https://github.com/wmo-im/wis2-guide/commit/5195830e3581085d639659a7f6cea263c82fd828).

Issue closed.

### 5.5 Task: Review best practices (if available) for publishing NWP data in WIS2.

#### Summary

Review of best practices (if available) for publishing NWP (Numerical Weather Prediction) data in WIS2.

**Issue:** [wmo-im/wis2-guide#158](https://github.com/wmo-im/wis2-guide/issues/158)

#### Discussion

- @tomkralidis reported that TT-NWPMD is finalizing their proposal and will submit it to ET-Metadata/TT-WISMD for review. No timeline is attached to this action, other than a target of end of June.
- @6a6d74 noted this will not be included in the second Cookbook release.
- @golfvert requested that this work be motivated towards conclusion.

#### Next Steps

- [ ] ACTION (@hhaddouch) Follow up with Secretariat/Yuki to motivate conclusion of the TT-NWPMD activity to develop best practices for publishing NWP (Numerical Weather Prediction) data in WIS2.

## 6.Release logistics:
### 6.1 Task: Agree the updated (increased) FAST-TRACK release schedule to cater for more frequent updates to topic hierarchy. 

#### Summary

Agree the updated (increased) FAST TRACK release schedule to accommodate more frequent updates to the topic hierarchy.

**Issue:** [wmo-im/wis2-topic-hierarchy#286](https://github.com/wmo-im/wis2-topic-hierarchy/issues/286)

#### Discussion

Recommendation: a quarterly release schedule at maximum frequency, with releases occurring only when needed.

#### Next Steps

- [ ] ACTION (@hhaddouch) to inform @amilan17

### 6.2 Task: Agree implementation schedule for Global Services to implement changes in FT2026-1.

#### Summary

Agree implementation schedule for Global Services to implement changes in FT2026-1. See the [FT2026-1 changes document](https://wmoomm.sharepoint.com/:b:/s/Collaboration/IQCZlsGiL6pjSZZidsuOORF5AeksERMvD5gorHca4i8sbKo?e=FCfOyZ) for details.

**Issue:** [wmo-im/et-w2it#54](https://github.com/wmo-im/et-w2it/issues/54)

#### Discussion

- Changes must be implemented between 20 June 2026 and 1 November 2026, per the FT2026-1 release. CMA has already implemented the changes to their Global Cache.
- The key concern is avoiding disruption to Global Monitor dashboards through inconsistent metrics. Two options were considered: coordinating implementation dates across Global Caches, or having Global Monitors create a new dashboard for the amended metrics alongside the existing one.
- Creating an alternative dashboard is the preferred approach, as it allows Global Caches (and others) to implement the change on a schedule that suits local plans.
- ET-W2IT will revisit this action later for a status update.

#### Issue Identified

The Global Monitor [`alerts.yml` for Global Cache](https://github.com/wmo-im/wis2-metric-hierarchy/blob/main/alerts/gc.yml) is out of date and still references the old Global Cache metrics (superseded in FAST TRACK 2026). Until this is fixed, automated alerts may be incorrect. It is proposed to suspend automated alert creation for Global Caches until the YAML is updated.

#### Next Steps

- [ ] ACTION (@elgarraichemseddine, @shirley-xuelei) to create and publish a new dashboard for the new GC metrics
- [ ] ACTION (@elgarraichemseddine, @shirley-xuelei) to update [`alerts.yml`](https://github.com/wmo-im/wis2-metric-hierarchy/blob/main/alerts/gc.yml) for Global Cache to use the amended metrics; automated alert creation for Global Caches is suspended until this is complete

### 6.3 Update: GDC metrics implementation. 

#### Summary

Update on GDC metrics implementation coordination.

**Issue:** [wmo-im/et-w2it#55](https://github.com/wmo-im/et-w2it/issues/55)

#### Discussion

@tomkralidis confirmed convergence on a cutover date of 24 June 2026 at 12:00 UTC (REF: WI-84).

### 6.4 Task: Go/no-go decision on which recipes to be included in June-release of Cookbook.

#### Summary

Go/no-go decision on which recipes to include in the June release of the Cookbook.

**Issue:** [wmo-im/et-w2it#49](https://github.com/wmo-im/et-w2it/issues/49)
**See also:** [wmo-im/wis2-guide#158](https://github.com/wmo-im/wis2-guide/issues/158)

#### Discussion

Following earlier discussion, [wis2-guide#158](https://github.com/wmo-im/wis2-guide/issues/158) (Best practices for publishing NWP data) will not be included in this release.

@golfvert proposed proceeding with the release, comprising 3 new recipes.

#### Next Steps

- [x] ACTION (@tomkralidis) to cut the new Cookbook release ready for final review. This action is complete - see WIS2 Cookbook 1.1.0: https://wmo-im.github.io/wis2-cookbook/cookbook/latest/wis2-cookbook-STABLE.html

## 7.INFCOM-4 papers:
### 7.1 Task: Review / amend / approve draft section describing Sensor Centres for inclusion in INFCOM-4 Information paper about WIS2 performance. Text should include how performance dashboards (from Sensor Centre metrics) are shared with Members. 

#### Summary

Two changes proposed to the draft section describing Sensor Centres. Issue [wmo-im/et-w2it#38](https://github.com/wmo-im/et-w2it/issues/38).

#### Discussion

- Remove the reference to the WCMP2 daily archive, as it is too implementation-specific.
- Add a note that operating a Sensor Centre is an easy way for Members to contribute to WIS2.

#### Outcome

Text amended accordingly. ET-W2IT approved the text for use.

#### Next Steps

- [ ] ACTION (@hhaddouch) to consider the proposed [text](https://github.com/wmo-im/et-w2it/issues/38#issuecomment-4613477956) for inclusion in the INFCOM-4 Information paper

Closing issue [wmo-im/et-w2it#38](https://github.com/wmo-im/et-w2it/issues/38) as ET-W2IT actions are complete.

### 7.2 Task: Review status of WIS2 report for INFCOM-4.

#### Summary

Review of the status of the WIS2 report for INFCOM-4.

#### Outcome

ET-W2IT reviewed the draft INFCOM paper presented by Secretariat, and confirmed that it was headed in the right direction.

## 8.Any other business:
### 8.1 Update: GRep service pilot implementation.

#### Summary

Update on the pilot implementation of the Global Replay (GRep) service. Issue [wmo-im/et-w2it#51](https://github.com/wmo-im/et-w2it/issues/51)

#### Discussion

- @tomkralidis noted little to report this cycle. Some messages are still being lost, related to the hardware environment.
- The action on @davidpodeur (to open a new issue in [wmo-im/wis2-grep](https://github.com/wmo-im/wis2-grep) describing the concern, with @tomkralidis to respond - see [wmo-im/et-w2it#51](https://github.com/wmo-im/et-w2it/issues/51#issuecomment-4430853792)) has been discarded.
- The Guide has been updated to reflect 24-hour retention on WNM.
- South Korea confirmed they are running a GRep instance.
- @golfvert noted formal testing isn't needed, but a comparison would be valuable. These Services should be publicly available by INFCOM-4.

#### Next Steps

- [ ] ACTION (@kay-goranlee52) to share access details / service URL for KMA's GRep implementation
- [ ] ACTION (@tomkralidis) to coordinate with colleagues from South Korea to compare functionality / performance, aiming to schedule testing for mid-September

### 8.2 Discussion: WIS2 portal.

#### Summary

Discussion on developing a "shiny portal" for WIS2, including funding, ownership, and specification questions.

**Raised by:** @hhaddouch

#### Discussion

- @hhaddouch noted that WMO should seek volunteers to develop and run a WIS2 portal.
- @6a6d74 noted that Members would likely find it difficult to fund an additional service, particularly since it is not part of the Tech Regs, and suggested it would be better to coordinate with Members or WMO programmes already undertaking similar work. @6a6d74 also pointed out that commercial offerings already exist in this space, such as the [Synoptic Data viewer](https://viewer.synopticdata.com).
- @golfvert raised that, politically, any such portal would need to carry a WMO logo, and noted there is currently no specification for how the portal should function or what it should do.
- @shirley-xuelei mentioned that China is developing a portal, but questioned whether this would be appropriate to position as a "WMO" WIS2 portal.
- @tomkralidis emphasised the need to first understand what the portal should do, in order to assess whether the WIS2 Global Services can support that functionality.

#### Next Steps

- [ ] ACTION (Secretariat) to coordinate and identify any internal WMO opportunities that might help deliver a portal

### 8.3 WIS2 Node testing and backups: what level is backup a recommendation or a requirement?

#### Summary

Clarification on whether a backup WIS2 Node is a recommendation or a requirement, and at what level resilience should be specified.

**Raised by:** @solson-nws

#### Discussion

A backup WIS2 Node is "only an option" — there are multiple ways to deliver the required resilience for a WIS2 Node, and a backup node is just one approach among several.

#### Outcome

No action required. All four Global Brokers have agreed to implement the proposal as set out in the Guide.

### 8.4 WIS2 Community page:

#### Summary

Discussion on how to notify WIS2 users about the suspension or revocation of a Global Service, and how to communicate overall service health.

**Raised by:** @hhaddouch

#### Discussion

- @hhaddouch raised the question of how to notify WIS2 users about suspension or revocation of a Global Service. The group agreed to use the [WIS2 Community Page](https://community.wmo.int/site/knowledge-hub/programmes-and-initiatives/wmo-information-system-wis/wis2-overview), and to also include a simple "global service health status" indicator on the page.
- @hhaddouch outlined notification options: publishing to the Community Page and distributing through WIS2 newsletters.

#### Next Steps

- [ ] ACTION (ET-W2IT) to provide feedback on the Community Page to Secretariat
- [ ] ACTION (Secretariat) to build the "global service health status" dashboard on the Community Page

### 8.5 Making sure that all Global Caches  behave the same

#### Summary

Discussion on ensuring consistent behaviour across all Global Caches.

**Raised by:** @kaiwirt

#### Discussion

- @kaiwirt noted there are specific situations to consider regarding inconsistent Global Cache behaviour.
- @golfvert identified two dominant causes of problematic behaviour: the need for better rules on `data_id` (see task 5.3) and the over-use of updates.

#### Outcome

Both issues have already been resolved in previous discussions.

### 8.6 Publishing Updates (MSC-ECCC)

#### Summary

Discussion of update behaviour for Canada's WIS2 Node (CA-ECCC-MSC), which was publishing daily hydrological observation data as CSV files and appending an hourly observation as an update to that same data item — resulting in 24 updates per day to a single data item, which @golfvert's analysis indicates confuses Global Caches.

**Raised by:** @tomkralidis, @golfvert

#### Discussion

- @6a6d74 asked whether the group was looking for a policy or recommendation on what constitutes "appropriate" update behaviour.
- @golfvert clarified that updates in WIS2 are designed to accommodate corrections in GTS, and there are no limits on how many updates can be made to a data item. As an extreme example, treating each new NWP forecast run from a global centre as an "update" to the same data item would clearly be inappropriate.
- MSC/ECCC's pattern of appending an hourly observation to a daily CSV record (treating the daily record as the data item, updated 24 times per day) was identified as a similar case. MSC/ECCC is the only organisation exhibiting this repeated update behaviour; the next highest is Brazil, with 2 updates.
- Since only one centre is affected, @golfvert noted there's no need for changes to the Tech Regs or Cookbook — the behaviour itself just needs to be fixed.
- @tomkralidis confirmed the fix had already been deployed (approximately an hour prior to the meeting), publishing a "new" data item each hour rather than updating the existing one.

#### Outcome

No further action required, other than monitoring the effectiveness of the deployed fix.

### 8.7 Uniqueness of download URL in WNM message

**Issue:** [wmo-im/wis2-notification-message#180](https://github.com/wmo-im/wis2-notification-message/issues/180)

#### Discussion

Two assumptions were noted for a WNM message: the URL should be valid, and the URL should be unique within the retention period of GRep (replay). If a WIS2 Node or Global Cache overwrites the data-item resource at the same URL, a message pointing to an earlier version would no longer match the integrity checksum, appearing to a user as data corruption. GRep does not flatten out updates (i.e. it does not remove intermediate messages).

- @kaiwirt argued that publishing an update should invalidate the older version, and consequently the Global Cache overwrites the data object; storing multiple versions adds a storage burden for both Global Caches and WIS2 Nodes.
- @tomkralidis noted wis2box defaults to 30-day storage but overwrites the data object on update.
- @golfvert asked whether the Global Replay service returns the newest WNM first. @tomkralidis explained this isn't the default behaviour — HTTP requests default to first-in-first-out, though last-in-first-out can be requested by sorting by `pubtime` descending (e.g. via the [GRep collections endpoint](https://wis2-grep.weather.gc.ca/collections/wis2-notification-messages/items?sortby=-pubtime&f=json)); MQTT FETCH mode defaults to last-in-first-out.
- @6a6d74 suggested users should ignore data objects with an older `pubtime`, and that receiving the newest WNM first should prevent issues under normal behaviour. It was noted that even with newest-first ordering, issues could still arise if a user requests an interval that excludes the latest message. Where messages arrive out of order, a checksum failure would lead a user to discard the message and continue processing until the latest message arrives — acknowledged as a potential source of frequent errors.
- @golfvert noted the integrity checksum is not mandatory.
- @josusky added that the URL must be uniquely associated with a data-id regardless of whether it's an update.
- @golfvert asked whether this should be accepted as an edge case, affecting only a small fraction of the millions of messages sent daily. @6a6d74 proposed accepting this as an edge case ("grit in the machine") with no further action. @josusky suggested further analysis to gauge the scale of the problem.

**Global Cache responses on feasibility of incrementing URLs**

Germany: feasible to append an incrementing counter to URLs of updated data items. China: already stores all copies with incrementing URLs for updates. USA: prepared to implement a change. Japan: technically possible, current situation to be checked. IBL: already implements this. France (national cache): already implements this.

#### Outcome

Agreed solution: retain updates plus the original (for the original and 5 updates, this means 6 file names/URLs total), with each Global Cache deciding how to implement the incrementing name scheme.

#### Next Steps

- [ ] ACTION (@solson-nws) to lead a collaborative response from Global Caches to store updated resources, including engaging with Alberto (Secretariat) to ensure the WIS2-Downloader works correctly, and to propose any changes to the WNM spec needed to mitigate the non-unique URL issue

### 8.8 Reduce NFP review period for FAST TRACK to one-month

#### Summary

Proposal to reduce the NFP (National Focal Point) review period for FAST TRACK changes from the current duration to one month.

**Raised by:** @hhaddouch

#### Discussion

- @golfvert noted that valuable comments have rarely, if ever, been observed during FAST TRACK review. They questioned whether NFPs are the right reviewers for this process and suggested the review process itself may need to be reconsidered, rather than simply shortening the timeline.
- @kaiwirt countered that this review remains important, as it is currently the only mechanism for Members to intervene in FAST TRACK proposals.

#### Outcome

No objection to the proposal in principle. However, this is **not a decision for ET-W2IT** to make. Secretariat will progress options for improving the review process more broadly.

#### Next Steps

- [ ] ACTION (Secretariat) to develop and propose options for improving the FAST TRACK review process

### 8.9 Maximum number parallel downloads from one IP for Global Cache

#### Summary

Discussion on the parallel download limit specified in Guide 2.7.2.2, which currently caps connections at 5 — insufficient for multi-threaded Global Cache downloads from other Global Caches (or GTS-to-WIS2 Gateways) and for the multi-threaded workers used by the WIS2-Downloader.

**Raised by:** @guwj0609

#### Discussion

- Germany currently uses 16 parallel downloads and sees no rate-limiting in its logs; this could potentially be extended further.
- @golfvert's national cache implementation works effectively with 12 workers.
- Japan and the USA use AWS S3, where there is effectively no limit on parallel downloads.
- @golfvert proposed "no less than 16" as the new minimum, allowing flexibility for services like China to offer more.

#### Next Steps

- [x] ACTION (Rémy) to update Guide 2.7.2.2 to specify "no less than 16" parallel downloads

## 9.Closure
ET-W2IT reviewed changes to Manual and Guide (in `2026-06-brasilia` branch; see pull requests `wmo-im/wis2-guide#256` and `wmo-im/wis2-manual#15`).
Following editorial amendments, these changes were merged into the `INFCOM-4` branch.



