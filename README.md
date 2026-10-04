# AWS Cloud Portfolio

A hands-on cloud engineering project where I built and progressively improved a personal portfolio website using AWS.

Rather than treating the project as a single deployment, I am evolving the architecture through multiple versions to explore cloud hosting, security, content delivery, automation, and Infrastructure as Code.

## Current Architecture — Version 2

![CloudFront + Private S3 Architecture](./docs/v2-cloudfront-private-s3/architecture.png)

The current architecture uses **Amazon CloudFront** as the public HTTPS delivery layer with **Amazon S3 configured as a private origin**.

Direct public access to the S3 bucket is blocked.

## Architecture Evolution

### Version 1 — Amazon S3 Static Website Hosting

The first version introduced the fundamentals of static website hosting on AWS.

**Architecture:**

`User → HTTP → Amazon S3 Static Website Endpoint`

Key concepts:

- Amazon S3
- Static Website Hosting
- S3 bucket policies
- Public read access
- HTML/CSS deployment
- Git and GitHub

[View Version 1 Documentation](./docs/v1-s3-static-hosting/README.md)

### Version 2 — CloudFront + Private Amazon S3

Version 2 improves the architecture by introducing a CDN, HTTPS, and a private S3 origin.

**Architecture:**

`User → HTTPS → Amazon CloudFront → Private Amazon S3`

Key concepts:

- Amazon CloudFront
- CDN and edge caching
- HTTPS
- Private S3 origin
- S3 Block Public Access
- CloudFront service principal
- Resource-based bucket policies
- Restricted origin access

[View Version 2 Documentation](./docs/v2-cloudfront-private-s3/README.md)

## Technologies

**Frontend**

- HTML5
- CSS3

**Cloud**

- Amazon S3
- Amazon CloudFront
- AWS Bucket Policy concepts

**Development & Version Control**

- Visual Studio Code
- Git
- GitHub

## Documentation

- [Version 1 — S3 Static Website Hosting](./docs/v1-s3-static-hosting/README.md)
- [Version 2 — CloudFront + Private S3](./docs/v2-cloudfront-private-s3/README.md)
- [Git Commands Reference](./GIT_COMMANDS.md)