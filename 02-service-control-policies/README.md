AWS SCP lab restricting EC2 instance types in sandbox

This lab demonstrates enforcing cost and governance guardrails with an AWS Service Control Policy (SCP) that denies launching EC2 instances unless the instance type is in an approved micro list. It’s built for a sandbox account inside an AWS Organization and presented CLI-first with curated console visuals.
Objective and scope

 Goal: Prevent oversized or costly EC2 launches by allowing only approved micro instance types in the sandbox.
 
 Scope: Attach SCP to the sandbox account (or Sandbox OU). Applies to all IAM principals in that account.
 
 Guardrail model: SCP defines the maximum permissions; IAM policies can’t grant what SCP denies.

Architecture overview

Management account: Owns AWS Organizations and creates/attaches SCPs.

Sandbox account: Target account where EC2 launches are constrained.

Policy placement: SCP attached to Sandbox account or OU; evaluated alongside IAM policies.

Coverage: Blocks ec2:RunInstances and ec2:CreateFleet unless instance type is in the allowlist.

Tip: Keep this SCP scoped to sandbox until validated. Promote to broader OUs only after blast‑radius testing.
