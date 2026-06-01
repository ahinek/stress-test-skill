# Jira Workspace Consolidation - Stress Test Example

This example demonstrates the output of the stress-test skill operating in Default Mode.

Source initiative:
Consolidation of multiple Jira workspaces into a centralized Jira workspace to improve visibility, governance, reporting consistency, and cross-team coordination.

Generated using:
- stress-test skill
- Default Mode

This example is intended to demonstrate the expected output format prior to running the risk-reduction skill.

  Stress Test: Jira Workspace Consolidation
  
  Frame: It is six months from now. The Jira workspace consolidation has failed. Multiple teams have abandoned the centralized workspace. Leadership visibility is worse than before consolidation. Delivery
  throughput has declined. We are now working backward to explain why.

  ---
  Executive Summary

  Most Likely Failure

  Teams create shadow tracking systems outside Jira while superficially complying with centralized reporting requirements. Teams maintain the centralized workspace for leadership visibility but continue using
  team-specific tools (Notion, GitHub Projects, Slack threads, spreadsheets) for actual work coordination. The standardized workflows are too rigid for real delivery needs, so teams route around them while
  producing just enough Jira activity to satisfy reporting expectations.

  Most Dangerous Failure

  Migration breaks critical automation and integrations, causing weeks of delivery disruption during active release cycles. Teams discover broken CI/CD triggers, release automation, support ticket routing, and
  cross-system integrations only after migration. Because delivery commitments remain active and Jira admin capacity is limited, teams cannot quickly fix these issues. The disruption cascades: missed delivery
  milestones damage stakeholder trust, teams lose confidence in the consolidation, and resistance to the new system becomes permanent.

  Cheapest Failure to Prevent

  Historical data migration produces unusable backlogs with broken links, lost context, and corrupted field mappings. Preventing this requires pre-migration data quality audits and controlled pilot migrations
  with rollback capability. The cost is 2-3 weeks of careful preparation. The alternative is months of teams unable to reference historical work, broken sprint reports, and lost institutional knowledge that
  undermines adoption of the new system.

  Hidden Assumption

  The assumption that "standardized workflows" will fit all team needs simultaneously. The plan assumes that engineering teams, QA teams, and product teams can operate effectively using the same issue types,
  workflow states, and field definitions. In reality, different teams have different operational cadences, different handoff patterns, and different reporting needs. Forcing standardization without accommodating
  legitimate workflow differences will drive teams to work around the system rather than adopt it.

  Readiness Recommendation

  Conditionally Ready for Risk Reduction

  - Migration approach lacks pilot phase with rollback capability
  - No clear process for handling workflow exceptions without creating governance bottlenecks
  - Integration/automation inventory and testing strategy is unspecified
  - Success criteria focus on adoption metrics but not delivery health metrics
  - Pre-migration data quality assessment not mentioned in plan

  ---
  Failure Modes

  ┌──────────────────────────────────────────────────────────────────────────────┬────────────┬────────┬───────────────────────────────────────────────────────────────────────────────────────────────────────┐
  │                                 Failure Mode                                 │ Likelihood │ Impact │                                             Warning Sign                                              │
  ├──────────────────────────────────────────────────────────────────────────────┼────────────┼────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Teams create shadow processes outside Jira while superficially complying     │ High       │ High   │ Teams show high Jira update activity but actual coordination happens in Slack; sprint planning        │
  │ with centralized reporting                                                   │            │        │ meetings reference external docs                                                                      │
  ├──────────────────────────────────────────────────────────────────────────────┼────────────┼────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Migration breaks critical automation/integrations during active delivery     │ High       │ Severe │ Teams discover broken CI/CD triggers, release automation, or support routing only post-migration;     │
  │ cycles                                                                       │            │        │ fixes require weeks not days                                                                          │
  ├──────────────────────────────────────────────────────────────────────────────┼────────────┼────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Standardized workflows create bottlenecks that slow delivery more than       │ High       │ High   │ Cycle time increases; teams request workflow exceptions faster than governance can approve them; work │
  │ fragmentation did                                                            │            │        │  stalls in non-applicable states                                                                      │
  ├──────────────────────────────────────────────────────────────────────────────┼────────────┼────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Historical data quality issues make migrated backlogs unusable               │ Medium     │ Medium │ Teams cannot find historical context; broken links and field mappings force re-creation of tribal     │
  │                                                                              │            │        │ knowledge; reporting becomes unreliable                                                               │
  ├──────────────────────────────────────────────────────────────────────────────┼────────────┼────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Centralized governance becomes a bottleneck for operational decisions        │ Medium     │ High   │ Simple workflow adjustments require cross-team approvals; teams wait weeks for permission changes;    │
  │                                                                              │            │        │ local agility is lost                                                                                 │
  └──────────────────────────────────────────────────────────────────────────────┴────────────┴────────┴───────────────────────────────────────────────────────────────────────────────────────────────────────┘

  ---
  Base-Rate Analysis
  
  ┌─────────────────────────────────────────────┬─────────────┬────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
  │                Failure Mode                 │ Probability │                                                              Base-Rate Rationale                                                               │
  ├─────────────────────────────────────────────┼─────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Shadow processes emerge                     │ 70-80%      │ Enterprise tool consolidations routinely produce compliance theater where teams maintain parallel systems when centralized tools don't fit     │
  │                                             │             │ real workflow needs                                                                                                                            │
  ├─────────────────────────────────────────────┼─────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Integration breakage causes delivery        │ 60-70%      │ Large-scale Jira migrations commonly underestimate integration dependencies; automation breaks are discovered post-migration, not              │
  │ disruption                                  │             │ pre-migration                                                                                                                                  │
  ├─────────────────────────────────────────────┼─────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Standardization slows delivery              │ 50-60%      │ Workflow standardization across diverse teams typically optimizes for reporting consistency at the cost of local efficiency; teams with fast   │
  │                                             │             │ cadences suffer most                                                                                                                           │
  ├─────────────────────────────────────────────┼─────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Data quality undermines adoption            │ 40-50%      │ Historical data migrations with inconsistent source data routinely produce corrupted field mappings and broken references that erode trust in  │
  │                                             │             │ the new system                                                                                                                                 │
  ├─────────────────────────────────────────────┼─────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Governance bottlenecks block agility        │ 50-60%      │ Centralized governance models in large organizations commonly create approval delays that were absent in decentralized models; operational     │
  │                                             │             │ friction increases                                                                                                                             │
  └─────────────────────────────────────────────┴─────────────┴────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘

  ---
  Organizational Failure Patterns

  ┌──────────────────────────────────────────────────────┬─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
  │                       Pattern                        │                                                                   Why It Matters                                                                    │
  ├──────────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Optimizing for leadership visibility at the expense  │ The stated goals prioritize portfolio-level planning, standardized reporting, and executive visibility, but success criteria do not include         │
  │ of team operational efficiency                       │ delivery throughput or team satisfaction — teams will game metrics to satisfy reporting while working around the system                             │
  ├──────────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Limited Jira admin capacity during active delivery   │ Migration complexity and ongoing support needs will overwhelm limited admin capacity; teams will be blocked waiting for fixes while delivery        │
  │ commitments                                          │ deadlines continue, forcing workarounds and eroding adoption                                                                                        │
  ├──────────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Centralized governance replacing local               │ Teams currently have autonomy to adjust workflows and fields; consolidation introduces approval gates without defining what decisions can be made   │
  │ decision-making without clear escalation paths       │ locally versus centrally, creating friction and slowing operational changes                                                                         │
  └──────────────────────────────────────────────────────┴─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘

  ---
  Revised Plan Recommendations

  ┌──────────┬─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┬───────────────────────────────────────────────────────────────┐
  │ Priority │                                                         Recommendation                                                          │                    Failure Modes Addressed                    │
  ├──────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────┤
  │ 1        │ Run pilot migration with 2-3 diverse teams and full rollback capability before organization-wide rollout                        │ Integration breakage, data quality issues, workflow           │
  │          │                                                                                                                                 │ bottlenecks                                                   │
  ├──────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────┤
  │ 2        │ Create pre-approved workflow exception framework with team-level autonomy for non-cross-team processes                          │ Workflow bottlenecks, governance bottlenecks, shadow          │
  │          │                                                                                                                                 │ processes                                                     │
  ├──────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────┤
  │ 3        │ Inventory all automation and integrations; require migration testing with rollback plan before cutting over active delivery     │ Integration breakage, delivery disruption                     │
  │          │ work                                                                                                                            │                                                               │
  ├──────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────┤
  │ 4        │ Add delivery health metrics (cycle time, throughput, team satisfaction) to success criteria alongside reporting consistency     │ Optimizing for visibility over efficiency, workflow           │
  │          │ metrics                                                                                                                         │ bottlenecks                                                   │
  ├──────────┼─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────┤
  │ 5        │ Establish 2-week data quality assessment phase; migrate only projects that pass quality thresholds                              │ Data quality issues, lost historical context                  │
  └──────────┴─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┴───────────────────────────────────────────────────────────────┘

  ---
  Pre-Launch Checklist

  - [ ] Pilot migration completed with 2-3 diverse teams; lessons learned documented; rollback successfully tested
  - [ ] All active automation and integrations inventoried; migration testing plan exists; rollback procedures validated
  - [ ] Workflow exception framework defined; team-level autonomy boundaries clear; escalation paths documented
  - [ ] Historical data quality assessed; migration acceptance criteria established; teams acknowledge data limitations
  - [ ] Delivery health baseline metrics captured; monitoring dashboard created; threshold for rollback decision defined

  ---
  Early Warning Indicators
  
  ┌───────────────────────────────────────────────────────────────────────────────────────────┬────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
  │                                         Indicator                                         │                                                 Why It Matters                                                 │
  ├───────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Teams show increasing Jira activity but delivery coordination discussions move to Slack   │ Indicates teams are gaming metrics while working around the system — shadow processes are emerging             │
  │ or external tools                                                                         │                                                                                                                │
  ├───────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Cycle time or throughput declines in first 4 weeks post-migration for any team            │ Indicates workflow standardization is creating friction; without early intervention, teams will route around   │
  │                                                                                           │ the system permanently                                                                                         │
  ├───────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Workflow exception requests accumulate faster than governance can approve them            │ Indicates centralized governance is becoming a bottleneck; teams will stop asking and start working around     │
  │                                                                                           │ constraints                                                                                                    │
  ├───────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Teams reference "we used to be able to..." more than "the new system lets us..." in       │ Indicates adoption resistance is hardening; teams perceive consolidation as loss of capability rather than     │
  │ retrospectives                                                                            │ improvement                                                                                                    │
  ├───────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Support ticket volume to Jira admins increases week-over-week instead of declining after  │ Indicates integration/automation breakage or usability issues are not resolving; admin capacity will be        │
  │ initial migration                                                                         │ overwhelmed                                                                                                    │
  └───────────────────────────────────────────────────────────────────────────────────────────┴────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘

  ---
  Summary

  Most Likely Failure: Teams create shadow processes outside Jira while superficially complying with centralized reporting, because standardized workflows don't fit real operational needs.

  Hidden Assumption: That standardized workflows can simultaneously serve all team types without accommodating legitimate workflow differences or creating local efficiency losses.

  Most Important Revision: Run a pilot migration with diverse teams and full rollback capability before organization-wide rollout — this is the cheapest way to surface integration breakage, workflow friction,
  and data quality issues before they cause permanent adoption resistance.
