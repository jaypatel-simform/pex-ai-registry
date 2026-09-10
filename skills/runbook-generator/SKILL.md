---
name: runbook-generator
description: Generate deployment runbooks with setup, deployment, rollback, and troubleshooting procedures
stage: documentation
triggers:
  - runbook
  - deployment doc
  - operations doc
  - ops doc
  - deploy guide
  - deployment runbook
prerequisites:
  - docx
output_format: docx
version: 0
---

# Runbook Generator Skill

## Overview

Generates a deployment runbook covering environment setup, first-time deployment, ongoing deployments, rollback procedures, monitoring, troubleshooting, incident response, and maintenance tasks.

## Prerequisites

- Read infrastructure and design artifacts if available.
- Apply document formatting guidelines from docx skill.

## Workflow

1. Document environment prerequisites and configuration
2. Define first-time setup procedures step-by-step
3. Document standard deployment procedures
4. Create rollback procedures with verification steps
5. Define monitoring setup and alert thresholds
6. Create troubleshooting guide with at least 5 common issues
7. Document incident response procedures
8. Define at least 4 regular maintenance tasks
9. Include emergency contacts and escalation paths
10. Save as both markdown and docx artifacts

## Quality Gates

- [ ] Environment prerequisites section present
- [ ] First-time setup procedure documented
- [ ] Deployment procedure with numbered steps
- [ ] Rollback procedure with verification checks
- [ ] Monitoring section with alert thresholds
- [ ] At least 5 troubleshooting entries
- [ ] Incident response procedure defined
- [ ] At least 4 maintenance tasks documented
- [ ] Contact/escalation information included

## Output Format

Save as `{ProjectName}_Deployment_Runbook_v{Version}.docx` in the outputs directory.
