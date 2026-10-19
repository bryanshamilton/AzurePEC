---
name: Azure PEC AOBO Tool
tagline: Bulk-assign Partner Earned Credit RBAC roles across customer tenants in minutes
category: Automation
status: ga
# TODO (repo owner): confirm the executive sponsor accountable for this solution
# exec_sponsor:
# TODO (repo owner): confirm stakeholder teams/functions
# stakeholders:
#   -
audience: MSPs and Arrow CSP partners managing RBAC across customer Azure tenants
problem: >
  Partner Earned Credit requires PEC-eligible RBAC role assignments across every managed
  customer subscription. Doing this by hand, subscription by subscription, is slow and
  error-prone — and every missed assignment quietly erodes PEC margin.
solution: >
  An interactive PowerShell tool that bulk-assigns PEC-eligible RBAC roles to your partner
  Foreign Group across selected customer subscriptions via Admin On Behalf Of (AOBO). A
  built-in dry-run previews changes and a per-subscription summary confirms exactly what
  succeeded, already existed, or failed.
highlights:
  - Guided ANSI TUI with banners, dividers, and prompts
  - Multi-select subscription picker (with select-all) and filterable multi-role menu
  - Validates required Az modules and forces a fresh login before running
  - "-DryRun switch previews assignments without touching resources"
  - Per-subscription, per-role success/existing/failure summary
tech:
  - PowerShell 7+
  - Az.Accounts
  - Az.Resources
  - Partner Center AOBO
links:
  repo: https://github.com/naccoe-docsNtools/AzurePEC
---

# Azure PEC AOBO Tool

Bulk-assign Partner Earned Credit RBAC roles across customer tenants in minutes.
