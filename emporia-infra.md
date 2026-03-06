1. traditional statement - project scope
2. pod mission elevate - month to month - support ongoing



## Problems

- ~50-60% of infra provisioned via click-ops
- Amplify Gen1 is a major bottleneck — slow deploys, expensive, blocks new stack/feature branch creation; mixes custom Amplify components with CDK primitives
- Shared data layer across personal/beta/prod — single large DDB table risks data contamination, limits experimentation, can't be reproduced per-stack
- Shared lambdas and supporting infra (OpenSearch, SQS, EventBridge, StepFunctions) are coupled across all stacks with no isolation boundary
- IAM policies are inconsistent, not locked down, and difficult to audit
- No isolation at any level — application, infra, data, or security — including no ability to restrict prod access

## High Level Work Items

### Phase 1 - Migration
- Migrate all Amplify apps Gen1 → Gen2 with resource dependency injection
- Migrate all shared lambdas (front-end dependencies + centralized services) from click-ops to CDK with CI/CD

### Phase 2 - Isolation
- Provision isolated Dev & Beta AWS accounts
- Create shared IAM resource policy package for all CDK resources
- Build shared data layer and core infra as CDK stacks with automated GitHub Actions deploys
- Build prod data import jobs to fully or selectively replicate prod in isolated dev environments

## Outcomes

- Full isolation of dev/local from prod with 100% CI/CD-managed stacks, apps, infra, and services
- All non-prod workloads contained in dedicated AWS accounts
- Faster onboarding and engineering velocity
- Foundation for autonomous agent workflows
- Foundation for compliance (SOC2) (MAYBE??)
- Safe environment for risky architectural changes and agentic workflow experimentation