# Pilot A — owner-scoped A4 execution

Reviewed fixture source: NTinkicht/OneCompany main, commit 97eea23b8c36c5cea5b4a17b9c60621fa4130c61.

This is an independently authorized disposable public repository, not customer code. Only WU-A may create docs/onecompany-fixture/WU-A.md via the canonical branch onecompany-a4-wu-a and one PR. OneCompany source remains L1. No extra paid spend.

Before running, verify local policies, default-branch SHA and exact reviewed worker/workflow Git blobs; configure repo vars ONECOMPANY_A4_PRODUCER_ENABLED=true, ONECOMPANY_A4_APPROVED_DISPATCHER=NTinkicht, ONECOMPANY_A4_LOGICAL_ACTOR=fixture-bot. The variable is default-off and must be intentionally enabled by the owner after installation review.

Trigger repository_dispatch event onecompany.a4-produce with client_payload {"work_unit":"WU-A","actor":"fixture-bot"}. Capture real Actions run ID. After PR creation dispatch .github/workflows/onecompany-a4-fixture-validation.yml against exact PR branch SHA and preserve run IDs. This README is not evidence of a completed pilot.

STOP: Actions variable ONECOMPANY_EMERGENCY_STOP must remain absent/false to allow new producer jobs; true or unrecognized value skips before runner allocation. Cancel existing live job in Actions separately. Keep producer flag OFF until exact-head source review and run preflight.
