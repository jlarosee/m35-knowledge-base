
## Problems

- ~50-60% of infra provisioned via click-ops
- Amplify Gen1 is a major bottleneck — slow deploys, expensive, blocks new stack/feature branch creation; mixes custom Amplify components with CDK primitives
- Shared data layer across personal/beta/prod — single large DDB table risks data contamination, limits experimentation, can't be reproduced per-stack
- Shared lambdas and supporting infra (OpenSearch, SQS, EventBridge, StepFunctions) are coupled across all stacks with no isolation boundary
- IAM policies are inconsistent, not locked down, and difficult to audit
- No isolation at any level — application, infra, data, or security — including no ability to restrict prod access
