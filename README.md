# FinOps-Case-Study
AWS FinOps Case Study: May 2025 Free Tier Usage Report
AWS FinOps Case Study: May 2025 Free Tier Usage Report
This case study showcases my hands-on experience with FinOps (Cloud Financial Operations) principles using a Free Tier AWS account. I analyzed real usage data from May 2025, explored cost patterns, and made actionable recommendations for optimizing cloud expenses — a foundational exercise in aligning financial accountability with cloud resource management.
Overview
Objective: Analyze AWS Free Tier usage for May and identify ways to optimize costs.
Tools Used: AWS Cost Explorer, Budgets, S3, EC2, RDS, WAF, Route 53
Total Spend: $16.52
  (All services stayed within Free Tier or low-cost usage — no overages.)
Service Breakdown

Observations
AWS Virtual Private Cloud (VPC) was the largest contributor, likely due to a constantly running NAT Gateway, which can incur charges even in the Free Tier.
WAF had steady, low-level usage costs, suggesting it was enabled daily, and worth evaluating the necessity.
All compute and storage resources like EC2 and S3 remained well within the Free Tier, indicating efficient resource use.
1. Replace NAT Gateway with NAT Instance  
   NAT instance is cheaper for development/testing workloads with limited traffic.  
   [→ AWS Docs: Comparing NAT Gateway and NAT Instance](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-comparison.html)
2. Review and Pause WAF When Idle
   Consider disabling WAF rules during off-hours or when not testing endpoints.
3. Enable Consistent Resource Tagging
   Use tags like `Project=Demo`, `Owner=Awwal`, or `Environment=Test` to track costs more easily.
4. Set Service-Specific Budgets
   Extend beyond a general budget by configuring budgets for key services (like VPC or WAF).

Visuals
Monthly cost trend line

Outcomes and Next Steps

- Demonstrated cloud cost awareness by analyzing actual usage data.
- Reinforced FinOps practices around monitoring, budgeting, and accountability.
- Planning to deepen skills through further FinOps Foundation learning paths and real-world scenario builds.

I’m Awwal — an Accounting & Finance graduate with a growing focus on cloud financial management. This project is part of my FinOps learning journey, blending my finance background with my AWS cloud training.

