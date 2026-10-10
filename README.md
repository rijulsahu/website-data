# 🚀 Rijul Sahu - Lead Data Engineer & Cloud Solutions Architect

[![AWS Certified](https://img.shields.io/badge/AWS-Certified%20Solutions%20Architect-orange?style=for-the-badge&logo=amazon-aws)](https://www.credly.com/badges/517e7ddb-d863-4751-af60-fd476dd92cb6/public_url)
[![Databricks Certified](https://img.shields.io/badge/Databricks-Certified%20Data%20Engineer%20Associate-red?style=for-the-badge&logo=databricks)](https://credentials.databricks.com/159633769)
[![Live Portfolio](https://img.shields.io/badge/Live-Portfolio-brightgreen?style=for-the-badge&logo=amazonaws)](https://rijul.cloud)

> **Lead Data Engineer at Mars Snacking with 15+ years of experience and a focus on Cloud Solutions Architecture.**

## 🌟 Overview

This repository contains the static source for [rijul.cloud](https://rijul.cloud), a professional portfolio covering data engineering, cloud architecture, analytics platforms, and infrastructure automation. The site includes a homepage, resume, contact form, and eight detailed project case studies.

### 🎯 Key Highlights
- Lead Data Engineer at Mars Snacking with 15+ years of experience
- AWS Certified Solutions Architect and Databricks Certified Data Engineer Associate
- Eight case studies spanning big data, retail analytics, machine learning, AWS, and IaC
- Project examples include processing 6B+ pricing records and a text-classification solution with 85% accuracy

## 🛠️ Tech Stack

### Frontend
- HTML5, CSS3, and JavaScript
- Bootstrap, jQuery, and AOS for responsive layout and interactions
- Boxicons and IcoFont icons; locally bundled vendor assets

### Infrastructure & Deployment
- AWS Amplify Hosting with an Amplify-managed CloudFront distribution
- Route 53 DNS delegation and AWS Certificate Manager TLS
- GitHub-connected deployment from the `main` branch
- Web app manifest, sitemap, and `robots.txt`
- Formspree contact form protected by Cloudflare Turnstile

### Tools & Technologies Featured
- **Cloud**: AWS (Amplify, CloudFront, Route 53, Lambda, S3, VPC, EC2, RDS)
- **Data platforms**: Databricks, Snowflake, dbt, Hadoop, Hive, Exasol
- **Engineering**: Python, SQL, Apache Spark/PySpark, Apache Pig, Alteryx, Lua
- **Delivery**: Terraform, CloudFormation, GitHub Actions, CI/CD
- **Analytics**: Retail media bidding, retail execution reporting, CRM analytics, NLP

## 📁 Project Structure

```
website-data/
├── index.html                 # Home, about, resume, projects, contact
├── 404.html                   # Custom not-found page
├── customHttp.yml              # Amplify security response headers
├── manifest.json               # Installable web app metadata
├── robots.txt
├── sitemap.xml
├── favicon.ico
├── .github/workflows/
│   └── update-resume-date.yml  # Updates the resume date on the qa branch
├── assets/
│   ├── css/                    # Site styles
│   ├── fonts/                  # Local fonts
│   ├── img/                    # Site and project images
│   ├── js/                     # Site behavior
│   ├── thumbnails/             # Project thumbnails
│   ├── vendor/                 # Frontend libraries
│   └── Rijul_Sahu.pdf          # Resume
└── projects/                  # Eight project case studies
```

## 🚀 Featured Projects

1. [**Big Data Analytics with Hadoop**](projects/Hadoop.html) — Built a six-node Hadoop analytics platform processing 6B+ pricing records; reduced turnaround time by 83% and reported $150K in annual savings.
2. [**Data Integration using Python & Alteryx**](projects/DI.html) — Replaced a Syntasa-based Adobe Analytics integration with Python, Alteryx, and Exasol; automated daily delivery with no manual steps.
3. [**Exasol CRM Analytics Automation**](projects/Exasol.html) — Automated CRM retention reporting with Lua and Exasol, reducing report time from 45 minutes to 4 minutes and manual effort by up to 98%.
4. [**Topic Modelling & Text Classification**](projects/Topic_Modeling.html) — Built a distributed PySpark text pipeline achieving 85% classification accuracy, with processing in about three minutes.
5. [**Terraform AWS Infrastructure**](projects/Terraform.html) — Created reusable Terraform templates for a VPC, two subnets, EC2, and RDS, integrated with CI/CD. [Source repository](https://github.com/rijulsahu/vpc-2subnets-ec2-rds).
6. [**Retail Media Bid Optimization**](projects/Bid_Optimization.html) — Orchestrated nine AWS Lambda functions across SKAI, Snowflake, and Databricks for a weekly keyword-level ROAS optimization workflow, including manual retailer uploads.
7. [**Retail Execution Data Mart for SAAG Reporting**](projects/Retail_Store_POS.html) — Consolidated reporting into a dbt/Snowflake mart with 14 KPIs, three timeframes, and Kroger and Walmart fiscal calendars.
8. [**AWS Amplify Website Hosting**](projects/My_Static_Website.html) — This portfolio’s hosting design: Amplify, Route 53 DNS delegation, CloudFront, ACM-managed TLS, and GitHub deployment.

## 🔗 Related Repositories

These are separate projects in addition to this website repository:

- [SKAI API Code Base](https://github.com/rijulsahu/skai-api-code-base) — Python tooling for SKAI OAuth2, reports, and bulk updates; related to the retail media case study.
- [AWS VPC & EC2 Deployments](https://github.com/rijulsahu/vpc-2subnets-ec2-rds) — Terraform/OpenTofu examples for EC2 deployment and VPC best practices.

## 🌐 AWS Amplify Deployment Guide

The site is a static HTML/CSS/JavaScript project and does not require a framework build. Its current hosting configuration is:

- Amplify Hosting is connected to this GitHub repository and deploys the `main` branch.
- The domain is registered with Hostinger; DNS is delegated to an Amplify-managed Route 53 hosted zone.
- Amplify provisions the CloudFront distribution and ACM certificate for HTTPS.
- [customHttp.yml](customHttp.yml) configures response security headers.
- No application environment variables are required. The contact form uses Formspree and Cloudflare Turnstile.

To deploy a fork, connect its repository and production branch in AWS Amplify, set the app root to the repository root, and attach a domain through Amplify's domain management. For a custom domain registered elsewhere, follow the DNS delegation/validation values shown in the Amplify console rather than reusing this site's DNS records.

The workflow at `.github/workflows/update-resume-date.yml` is separate from production hosting: when the resume PDF changes on `qa`, it updates the date displayed in `index.html` and commits that change to `qa`.

## 🔧 Local Development

### Setup
```bash
# Clone the repository and enter its directory
git clone https://github.com/rijulsahu/website-data.git
cd website-data

# Start a local static web server
python -m http.server 8000
```

Open <http://localhost:8000>. Project pages and assets use relative paths, so serve the repository root rather than opening individual HTML files directly.

## 📈 Performance Optimizations

- Static files are delivered through Amplify Hosting and its CloudFront distribution.
- Project thumbnails use lazy loading on the homepage.
- The repository includes a web app manifest for supported install experiences; it does not include a service worker or offline caching.

### 🎯 SEO Features
- Page titles and descriptions are defined in the HTML pages.
- `sitemap.xml` and `robots.txt` are included.

## 🔒 Security Features

- HTTPS is provided by Amplify-managed TLS.
- [customHttp.yml](customHttp.yml) sets HSTS, Content Security Policy, frame/content-type protections, Referrer-Policy, Cross-Origin-Opener-Policy, and Permissions-Policy headers.
- Contact submissions are sent to Formspree; Cloudflare Turnstile is used for bot protection.
- Do not add private credentials or API tokens to this static repository.

## 🤝 Contributing

This is a personal portfolio. Suggestions and corrections are welcome through GitHub issues or pull requests. Keep project content consistent with the linked case studies and avoid committing credentials, generated deployment state, or private documents.

## 💼 Current Role & Certifications

**Lead Data Engineer at Mars Snacking** with 14+ years of experience. Current focus areas include data and analytics platform architecture, high-volume ingestion and transformation, performance and cost optimization, infrastructure as code, and technical leadership.

**Certifications:**
- [AWS Certified Solutions Architect](https://www.credly.com/badges/517e7ddb-d863-4751-af60-fd476dd92cb6/public_url)
- [Databricks Certified Data Engineer Associate](https://credentials.databricks.com/159633769)

## 📞 Contact

**Rijul Sahu**  
🏢 **Current Role**: Lead Data Engineer at Mars Snacking  
🌐 **Website**: [rijul.cloud](https://rijul.cloud)  
💼 **LinkedIn**: [rijul-sahu](https://www.linkedin.com/in/rijul-sahu-242b59129)  
📧 **Email**: [rijulsahu@duck.com](mailto:rijulsahu@duck.com) *(Business inquiries only)*  
🔗 **Stack Overflow**: [rijul-sahu](https://stackoverflow.com/users/2831370/rijul-sahu)  
💻 **GitHub**: [rijulsahu](https://github.com/rijulsahu)

---

*Portfolio source: [github.com/rijulsahu/website-data](https://github.com/rijulsahu/website-data) · Hosted on AWS Amplify.*