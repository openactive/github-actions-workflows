# github-actions-workflows
A repository that contains reusable GitHub Actions Workflows that are referenced throughout the OpenActive GitHub organisation

## dependabot-auto-approve

Ensures that dependencies stay updated automatically, with maintainers only intervening by exception (i.e. when an automatic update fails).

Note that [security concerns](https://github.com/dependabot/dependabot-core/issues/2243) are mitigated as (i) the GitHub actions that test PRs [do not have access to any secrets](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions#accessing-secrets), and (ii) approval of dependabot PRs is delayed for 20 days, to allow time for vulnerabilities to be discovered and the offending version removed from npm (and allow time for dependabot to close the associated PR).
