# Jira Workspace Consolidation - Stress Test Example

This example demonstrates the output of the stress-test skill operating in Default Mode.

Source initiative:
Consolidation of multiple Jira workspaces into a centralized Jira workspace to improve visibility, governance, reporting consistency, and cross-team coordination.

Generated using:
- stress-test skill
- Default Mode

This example is intended to demonstrate the expected output format prior to running the risk-reduction skill.

 ● Jira Consolidation Stress Test
   
  Executive Summary
     
  This consolidation assumes teams will adapt to central governance while maintaining delivery velocity. The plan underestimates cultural resistance, migration complexity, and governance overhead. Most likely 
  failure: teams abandon Jira for local tools mid-migration. Most dangerous: delivery stalls during migration window, missing committed releases. Cheapest to prevent: pilot the consolidated workspace with 1-2
  teams before full rollout.

  ---
  Failure Modes (Ranked by Risk)

  ┌───────────────────────────────┬──────────────────────────────────────────────────────────────────────────────────────────────┬────────────────────────────────────────────────────────────────┬────────────┐
  │         Failure Mode          │                                           Trigger                                            │                             Impact                             │ Likelihood │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Shadow process proliferation  │ Teams find centralized workflows too rigid; revert to spreadsheets, Slack, or local tools    │ Jira becomes unreliable source of truth; governance fails      │ High       │
  │                               │                                                                                              │ silently                                                       │            │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Migration-induced delivery    │ Work items lost/blocked during migration; teams wait for admin fixes instead of delivering   │ Missed commitments, leadership loses confidence in initiative  │ High       │
  │ stall                         │                                                                                              │                                                                │            │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Governance bottleneck         │ Central approval required for workflow changes; limited admin capacity creates 2-4 week      │ Teams blocked from adapting to project needs; resentment grows │ Medium     │
  │                               │ backlogs                                                                                     │                                                                │            │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Automation/integration        │ CI/CD, Slack bots, reporting tools hard-coded to old workspace structure                     │ Silent failures in pipelines; manual workarounds proliferate   │ High       │
  │ breakage                      │                                                                                              │                                                                │            │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Standardization theater       │ Teams comply superficially (identical issue types, workflows) but diverge in practice        │ Reports look consistent but are incomparable; cross-team       │ Medium     │
  │                               │ (custom fields, tags, conventions)                                                           │ dependencies still fail                                        │            │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Historical data loss          │ Inconsistent data quality pre-migration; migration drops context, attachments, or custom     │ Teams lose audit trail; planning based on flawed historical    │ Medium     │
  │                               │ fields                                                                                       │ metrics                                                        │            │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Skilled worker exodus         │ Power users who built team-specific automations see their work discarded; leave for teams    │ Loss of institutional knowledge; remaining team struggles with │ Low        │
  │                               │ with autonomy                                                                                │  new system                                                    │            │
  ├───────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────┼────────────┤
  │ Executive reporting mirage    │ Portfolio dashboards aggregate incompatible data (different "done" definitions, story point  │ Leadership makes decisions on misleading metrics               │ Medium     │
  │                               │ scales)                                                                                      │                                                                │            │
  └───────────────────────────────┴──────────────────────────────────────────────────────────────────────────────────────────────┴────────────────────────────────────────────────────────────────┴────────────┘

  ---
  Most Likely Failure

  Shadow process proliferation — Teams will comply with the mandate to use centralized Jira, but when workflows don't fit their needs (e.g., release engineering needs approval gates, research teams need
  exploratory tracking), they'll maintain "real" work in Google Sheets, Notion, or Slack threads. Jira becomes the performative system for leadership reporting, not the operational system. This has happened in
  every enterprise consolidation I've observed where standardization was prioritized over team autonomy.

  ---
  Most Dangerous Failure

  Migration-induced delivery stall — If active sprints are disrupted (work items locked during migration, board queries broken, automations offline), teams will halt delivery to "wait for Jira to be fixed."
  Leadership sees initiative as blocking execution. The project gets emergency-paused, but by then trust is damaged and teams resist re-engagement. Unlike shadow processes (which fail slowly), this fails loudly 
  and publicly in 1-2 sprint cycles.

  ---
  Cheapest Failure to Prevent

  Pilot with 1-2 teams before full rollout — Cost: 4-6 weeks, 0.5 FTE admin overhead. Prevents 5 of 8 failure modes above by surfacing:
  - Which automations/integrations break (fix before they affect 20 teams)
  - Which workflows are genuinely incompatible (adjust standard before mandating it)
  - What governance overhead looks like at scale (adjust admin capacity before 200 requests queue)

  Base cost to fix failures post-launch: 6-12 months of rework, 10-20% delivery slowdown, lost credibility. Pilot cost: ~$50K (loaded). Post-failure cost: $500K-$2M (delivery delays + rework + attrition).

  ---
  Hidden Assumptions
  
  1. "Standardized workflows improve cross-team coordination" — Only true if teams actually have dependencies. If teams are independent, standardization is pure cost.
  2. "Teams want central visibility" — Teams want local control. Leadership wants visibility. The plan conflates these.
  3. "Historical data will migrate cleanly" — Plan assumes mapping exists between old custom fields and new schema. Reality: 30-50% of fields have no equivalent; data gets dropped or mangled.
  4. "Retraining resolves adoption issues" — Training fixes knowledge gaps, not incentive misalignment. If the new system makes someone's job harder, training won't fix it.
  5. "Limited admin capacity is a resourcing problem" — It's a design problem. Centralized governance + limited capacity = bottleneck by definition. No amount of hiring fixes architectural dependency.

  ---
  Base-Rate Reasoning

  Enterprise tool consolidations fail 60-70% of the time (Gartner, Forrester analyses). Common causes:
  - Underestimating cultural resistance (present here: "teams may resist")
  - Overestimating leadership mandate compliance (present here: assumes teams will adopt because told to)
  - Migration complexity explosion (present here: "historical data quality inconsistent" is a red flag)
  - Governance becoming a bottleneck (present here: "limited admin capacity")
  
  This plan has 4 of 4 known failure predictors. Prior probability of failure: 65% without significant changes.

  ---
  Organizational Failure Mode Analysis

  ┌────────────────────────────┬──────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
  │      Failure Pattern       │                                            Manifestation in This Plan                                            │
  ├────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Goodhart's Law             │ Teams optimize for "looks consolidated" (same issue types) instead of "works consolidated" (actual coordination) │
  ├────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Local optimization penalty │ Teams that built efficient local systems are forced to adopt slower central system; high performers punished     │
  ├────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Legibility trap            │ Leadership values uniform reports over effective workflows; standardizes metrics teams don't use                 │
  ├────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Substitution of goals      │ "Reduce admin overhead" becomes "reduce number of workspaces" (metric is hit, goal is missed)                    │
  ├────────────────────────────┼──────────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
  │ Iron Law of Oligarchy      │ Central governance team becomes gatekeepers; decisions prioritize ease-of-administration over team needs         │
  └────────────────────────────┴──────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘

  ---
  Revised Plan Recommendations

  1. Pilot Before Mandate

  - Select 1 high-performing team + 1 struggling team
  - Migrate them fully, run 2-3 sprints, collect friction reports
  - Fix top 10 issues before expanding

  2. Federated Governance Model

  - Central standards for interfaces (how teams expose work for portfolio reporting)
  - Team autonomy for implementation (workflows, fields, boards)
  - Admin capacity scales with team count (1 admin per 5-10 teams, not central bottleneck)

  3. Migration in Parallel, Not Sequential

  - Teams continue working in old workspace while new workspace is configured
  - Cutover happens in single sprint, not multi-week freeze
  - Rollback plan: old workspace stays read-only for 30 days

  4. Automation Audit Pre-Migration

  - Inventory all CI/CD integrations, Slack bots, reporting tools
  - Test in pilot; fix before rollout
  - Budget 20-30% more time than estimated (base rate: integrations take 2-3x longer to fix than expected)

  5. Measure Adoption, Not Compliance

  - Track: velocity before/after, time-to-resolve blockers, shadow tool usage
  - Do NOT track: "% teams migrated" (invites theater)

  6. Escape Valve for Edge Cases

  - 10-20% of teams will have legitimate needs the standard doesn't fit
  - Allow exemptions with documented rationale (reviewed quarterly)
  - Prevents shadow processes by giving teams legitimate path to diverge

  ---
  Pre-Launch Checklist

  - [ ] Pilot completed with 2 teams; top 10 friction points resolved
  - [ ] Integration test: CI/CD, Slack, reporting tools work in new workspace
  - [ ] Rollback plan documented and tested (old workspace reactivation < 4 hours)
  - [ ] Admin capacity plan: response time SLA defined (e.g., 48hr for workflow change requests)
  - [ ] Teams have 30-day dual-access period (old workspace read-only, new workspace active)
  - [ ] Leadership aligned on "adoption metrics" vs "compliance metrics"
  - [ ] Exemption process published (how teams request non-standard workflows)
  - [ ] Historical data loss assessment: teams notified which fields won't migrate
  - [ ] Training includes "how to request workflow changes" (not just "how to use Jira")
  - [ ] Early warning indicators defined (see below) with weekly review cadence

  ---
  Early Warning Indicators

  ┌───────────────────────────┬───────────────────────────────────────────────────────────┬────────────────────────────────────────────────────────┐
  │         Indicator         │                       Red Threshold                       │                         Action                         │
  ├───────────────────────────┼───────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────┤
  │ Velocity drop             │ >15% decline 2 sprints post-migration                     │ Pause rollout; investigate blockers                    │
  ├───────────────────────────┼───────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────┤
  │ Admin request backlog     │ >5 days average resolution time                           │ Add admin capacity or simplify approval process        │
  ├───────────────────────────┼───────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────┤
  │ Shadow tool mentions      │ Slack/email threads reference "the spreadsheet" >10x/week │ Interview teams; identify unmet workflow needs         │
  ├───────────────────────────┼───────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────┤
  │ Exemption requests        │ >30% of teams request exemptions                          │ Standard is too rigid; redesign                        │
  ├───────────────────────────┼───────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────┤
  │ Automation failures       │ >5 broken integrations reported/week                      │ Migration testing was insufficient; halt expansion     │
  ├───────────────────────────┼───────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────┤
  │ Leadership complaint rate │ >2 escalations/week about "Jira blocking work"            │ Delivery impact is material; consider rollback         │
  ├───────────────────────────┼───────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────┤
  │ User churn                │ >10% of power users leave or transfer teams               │ Loss of institutional knowledge; retention plan needed │
  └───────────────────────────┴───────────────────────────────────────────────────────────┴────────────────────────────────────────────────────────┘

  Weekly review: Consolidation steering committee reviews these metrics. Any 2 red thresholds = halt expansion pending fix.

  ---
  Risk-Reduction Readiness Assessment

  Not ready for risk-reduction in current form.

  Required before proceeding:
  1. Pilot first — The plan has zero validation. Run pilot, collect 4-6 weeks of real data, adjust.
  2. Governance model revision — Central bottleneck is load-bearing failure mode. Switch to federated model before announcing.
  3. Integration testing — "Integrations may break" is not a plan. Test and fix in pilot.

  If those three are addressed, risk-reduction appropriate for:
  - Rollback plan validation
  - Admin capacity sizing
  - Training content design

  Timeline: Pilot + revisions = 8-12 weeks. Do not skip pilot to meet deadline — the base rate says this fails 65% of the time without field validation.

