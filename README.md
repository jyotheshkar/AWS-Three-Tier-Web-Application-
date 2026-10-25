# AWS Three-Tier Web Application Lab

A personal AWS learning case study documenting a static frontend, serverless API and DynamoDB data tier. The original write-up records a March 2025 exercise.

**Maturity:** Documentation and architecture lab. This repository contains an architecture image and four PDFs; it does not contain the frontend files, Lambda source, infrastructure as code or automated tests. A current deployment, reproducible build and performance benchmark have not been established.

## Documented Architecture

![Presentation, logic and data tiers](AWS%20three%20tier.png)

| Tier | Services described in the lab | Purpose |
|---|---|---|
| Presentation | Amazon S3 and Amazon CloudFront | Store and deliver static web content |
| Logic | Amazon API Gateway and AWS Lambda | Expose an API and process retrieval requests |
| Data | Amazon DynamoDB | Store the user records described in the exercise |

The original notes discuss CloudFront Origin Access Control, Lambda IAM permissions, CORS, response handling and a DynamoDB `userId` partition key. These are documented lab topics, not independently verified current security or runtime properties.

## Lab Artifacts

- [Architecture image](AWS%20three%20tier.png)
- [CloudFront lab PDF](legendary-aws-networks-cloudfront.pdf)
- [API Gateway lab PDF](legendary-aws-compute-api.pdf)
- [Lambda lab PDF](legendary-aws-compute-lambda.pdf)
- [Three-tier integration lab PDF](legendary-aws-compute-threetier.pdf)
- [Evidence, design decisions and limitations](docs/PORTFOLIO_EVIDENCE.md)

The PDFs are supporting learning artifacts. No live preview URL or repeatable deployment procedure is supplied here. Claims about security, scalability, latency and cost require additional configuration and measurement evidence.

Prepared by [Jyothesh Karnam](https://github.com/jyotheshkar).
