## 1. Scope of the Business Process

This business process describes how collateral submitted by a loan applicant is validated, appraised, evaluated, and approved within a Loan Management Information System (MIS).
The process begins when a customer submits collateral documents and ends when a secured loan is either approved or rejected. The MIS supports validation, appraisal workflows, eligibility rule processing, audit logging, and reporting for compliance and management dashboards.

Objectives

Ensure collateral is authentic, complete, and accurately valued.

Automate eligibility and coverage checks using system rules.

Improve decision-making for risk officers through structured evaluation data.

Maintain audit trails for regulatory and compliance reporting.

Provide MIS insights for operational analytics and monitoring.

Expected Outcomes

Reliable appraisal results

Faster loan decision-making

Reduced manual errors

Improved transparency through audit logs

Data available for MIS dashboards

## 2. Key Entities and Actors
Users

Customer – Submits collateral documents.

Loan Officer – Validates customer submissions and forwards approved applications.

Appraiser – Conducts field/desk asset verification and appraisal confirmation.

Risk Officer – Reviews evaluation and makes final loan approval or rejection decision.

MIS/Compliance Team – Uses system logs for auditing, monitoring, and reporting.

System (MIS) – Automates valuation, depreciation, eligibility checks, and audit logging.

Departments/Systems

Loan Origination Department

Appraisal Unit

Risk Management

MIS/Compliance

Automated PL/SQL-based Collateral Evaluation Engine

Roles & Responsibilities

Customer: Provides required documents

Loan Officer: Screens for completeness and correctness

Appraiser: Conducts asset verification and confirms valuation

System: Runs rules, stores data, logs actions

Risk Officer: Final eligibility decision

MIS: Extracts audit logs for dashboards and compliance reports

## 3. Swimlane Modeling Approach

The swimlane diagram separates responsibilities clearly across:

Customer

Loan Officer

Appraiser

System

Risk Officer

MIS/Compliance

This helps visualize how the workflow transitions between different actors and identifies accountability at each stage.

Key handoff points include:

Customer → Loan Officer: submission

Loan Officer → Appraiser and System

Appraiser → System

System → Risk Officer

Risk Officer → MIS

## 4. Use of BPMN/UML Notations

Start/End points define the process boundary.

Tasks represent human or system activities.

Decision diamonds show branching points (e.g., "Verified?" or "Sufficient Coverage?").

Arrows/flows show the logical sequence and dependencies.

Swimlanes map accountability.

## 5. Logical Flow Summary

Customer submits collateral form and documents.

Loan Officer validates submission:

If incomplete → returned to customer.

If complete → forwarded to Appraiser and System.

Appraiser verifies asset (field/desk).

If verification fails → inspection requested or rejection.

If verified → appraisal confirmed.

System ingests request, runs valuation & depreciation, checks eligibility rules, computes coverage ratio, and logs evaluation.

Risk Officer reviews evaluation:

If insufficient coverage → request additional collateral or reject.

If sufficient → approve secured loan.

MIS/Compliance consumes audit logs for dashboards and reporting.

## 6. MIS & Organizational Impact

Supports accurate loan pricing and risk management

Enables data-driven decisions through automated evaluations

Ensures regulatory compliance via audit logs

Improves transparency and accountability

Enhances processing speed increasing customer satisfaction

Provides analytics opportunities (coverage trends, asset types, risk scoring)

## 7. Analytics Opportunities

Tracking collateral performance trends

Identifying high-risk collateral types

Automating early-warning indicators

Monitoring appraiser efficiency

Real-time loan approval metrics for management dashboards
