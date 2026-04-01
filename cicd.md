# 3 CI/CD

## Introduction

When a startup grows, the team needs a CI/CD process that is both fast and reliable. For our context, the challenge is to release more often without increasing production risk. The three selected sources show the same pattern: manual delivery slows teams down, while automation improves quality, speed, and confidence.

Developers need quick delivery but the organization also needs stable releases. Without a structured pipeline, the can teams spend too much time on manual steps such as rework on code base and late bug detection.

In order to fix this issue, the team should define a CI/CD baseline that fits the current engineering context and can scale with future projects.

## Base Pipeline

The base pipeline should cover the minimum quality gates expected in modern CI/CD like automated build, automated tests, and controlled deployment steps. This baseline should run on every relevant change to keep feedback fast and consistent.

As highlighted across the sources, a strong foundation includes:

- Full automation for build, test & deployment tasks.
- Version controlled code and configuration, with traceable release tags.
- Caching to reduce waiting time for heavy process.

The team should also keep the pipeline simple at first, then extend it progressively. A practical sequence is: `build + test` first, then add deployment, notifications, security scanning, and advanced release strategies.

## Delivery Safeguards

In order to keep releases safe while moving quickly, the pipeline should include clear safeguards.

First of all, branch protection and release tagging should be mandatory for critical branches. This reduces accidental changes and improves release traceability.

Secondly, environment separation should be strict. Staging and production must remain isolated, and changes should be validated in staging before production rollout.

Thirdly, the team should enforce rollback and fail-fast behavior. If checks fail, the release must stop immediately, notify the team, and allow a fast rollback path.

Additional safeguards from the sources can be adopted depending on platform and maturity:

- Use multi-stage Docker builds to reduce image size and attack surface.
- Prefer secure container build approaches (e.g., Kaniko in Kubernetes contexts) over privileged Docker-in-Docker setups.
- Add flexible trigger rules so heavy pipelines run only when relevant files, branches, or events are involved.
- Integrate security checks (SAST, dependency scans, secret handling) directly into CI.

## Team Enablement Package

After defining the baseline and safeguards, the team should provide operational support that makes CI/CD sustainable in daily work.

This may include:

- Clear pipeline documentation for onboarding and troubleshooting.
- Team notifications (Slack/email/status checks) for immediate failure visibility.
- Shared templates for repositories to standardize CI/CD across projects.
- Collaboration habits: pipeline health is team-owned, not only DevOps-owned.

For mobile workflows specifically, the same principle applies with mobile tooling: build/test automation, staged distribution (for example internal testers before store release), protected secrets for signing keys, and optimized build times.

## Conclusion

Good CI/CD is not only about tooling choices. It is about setting a structured baseline, adding safeguards for reliability, and giving teams the support to operate the pipeline consistently. With this approach, the organization can ship faster while controlling risk.

## Sources

1. Nixys, From 2024 to 2025: Reflecting on CI/CD best practices*  
   https://medium.com/@nixys_io/from-2024-to-2025-reflecting-on-ci-cd-best-practices-030efa6d58d9
2. Dhruvin Soni, CI/CD Best Practices*  
   https://medium.com/@dksoni4530/ci-cd-best-practices-c288f6846346
3. David Onuche, *Best Practices for CI/CD Pipelines in Mobile Apps*  
   https://medium.com/@davidonuche/best-practices-for-ci-cd-pipelines-in-mobile-apps-8ea88df8580e
