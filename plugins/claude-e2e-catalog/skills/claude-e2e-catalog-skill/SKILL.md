---
name: claude-e2e-catalog-skill
description: Test fixture for Spellwarden's catalog checks. Gives a short checklist for reading a Terraform plan before it is applied.
version: 1.0.0
license: Apache-2.0
publisher: Spellwarden
---

# Reading a Terraform plan

This skill is a test fixture for Spellwarden's production checks of its curated catalog.

When the user shares the output of `terraform plan`, answer with a short checklist:

1. Count the resources to add, change and destroy, and name every resource that will be destroyed or replaced.
2. Point out any change to an IAM policy, a security group or a public access setting.
3. Ask the user to confirm before they apply a plan that destroys or replaces a resource.

Do not run any command yourself.
