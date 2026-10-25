# Portfolio Evidence: AWS Three-Tier Lab

## Scope

This repository preserves a personal learning case study. Its inspectable contents are the README, one architecture image and four lab PDFs. It is suitable for discussing service selection and tier boundaries; it is not an executable application package.

## Evidence and Design Decisions

| Source | Supported discussion | Limitation |
|---|---|---|
| [Architecture image](../AWS%20three%20tier.png) | Static web files feeding S3/CloudFront; API Gateway/Lambda logic tier; DynamoDB data tier | Conceptual diagram; does not show all application/data connections, identity controls or failure paths |
| [CloudFront PDF](../legendary-aws-networks-cloudfront.pdf) | Retained presentation-tier learning artifact | No independently executed content-delivery benchmark supplied |
| [API PDF](../legendary-aws-compute-api.pdf) and [Lambda PDF](../legendary-aws-compute-lambda.pdf) | Retained API/compute learning artifacts | Runtime configuration and behavior were not independently verified |
| [Integration PDF](../legendary-aws-compute-threetier.pdf) | Retained three-tier learning artifact | No reproducible environment or current deployment receipt supplied |

The original README describes S3/CloudFront for presentation, API Gateway/Lambda for request processing and DynamoDB for user records. It also mentions OAC, custom IAM policies, CORS and response handling. These are the decisions reported in the exercise, not a claim that the repository implements or validates those controls.

## What a Reviewer Can Assess

The case study introduces separation of presentation, request logic and persistence. A reviewer can question why each service was selected, where access is enforced and how data travels between tiers. The high-level diagram does not establish a full Well-Architected review.

## Missing Verification

- Frontend and Lambda source, infrastructure as code and dependency/runtime versions.
- Repeatable deployment and cleanup instructions.
- Authorization, IAM/OAC policy evidence and negative-access tests.
- API contracts, data schema, failure tests and observability evidence.
- Workload assumptions, availability/recovery targets, measured performance and dated cost estimates.

These are future evidence requirements. No new AWS resources were created, and no live tests, deployments or billable operations were performed for this documentation update.
