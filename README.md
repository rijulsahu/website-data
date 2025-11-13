# 🚀 Rijul Sahu - Lead Data Engineer & Aspiring Cloud Solutions Architect

[![AWS Certified](https://img.shields.io/badge/AWS-Certified%20Solutions%20Architect-orange?style=for-the-badge&logo=amazon-aws)](https://www.youracclaim.com/badges/8a29b89e-c32b-44f7-94be-800f7412c16d/linked_in)
[![Databricks Certified](https://img.shields.io/badge/Databricks-Certified%20Data%20Engineer%20Associate-red?style=for-the-badge&logo=databricks)](https://credentials.databricks.com/159633769)
[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=for-the-badge&logo=vercel)](https://rijul.cloud)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

> **Lead Data Engineer at Kellanova with 14+ years of experience, transitioning to Cloud Solutions Architect role**

## 🌟 Overview

This repository contains the source code for my professional portfolio website, highlighting my experience as a **Lead Data Engineer** and **aspiring Cloud Solutions Architect**. The site showcases real-world projects involving modern data platforms like Databricks, Snowflake, AWS cloud infrastructure, and enterprise-scale analytics solutions.

### 🎯 Key Highlights
- **Lead Data Engineer at Kellanova** with 14+ years of experience
- **Dual Certifications**: AWS Solutions Architect + Databricks Data Engineer Associate
- **Modern Data Stack**: Databricks, Snowflake, dbt, GitHub CI/CD workflows
- **Big Data Engineering** experience processing 6+ billion records
- **5 Major Projects** with detailed case studies and measurable business impact
- **DevOps & Infrastructure as Code** using Terraform and CI/CD pipelines
- **Machine Learning & Analytics** solutions with 85%+ accuracy rates

## 🛠️ Tech Stack

### Frontend
- **HTML5** - Semantic markup and accessibility
- **CSS3** - Responsive design with Bootstrap framework
- **JavaScript** - Interactive elements and animations
- **AOS Library** - Smooth scroll animations

### Infrastructure & Deployment
- **AWS Amplify** - Static website hosting and CI/CD
- **Progressive Web App (PWA)** - Installable web application
- **SEO Optimized** - Meta tags, sitemap, and structured data

### Tools & Technologies Featured
- **Cloud Platforms**: AWS (VPC, EC2, RDS, S3), Databricks
- **Modern Data Stack**: Databricks, Snowflake, dbt (data build tool)
- **Big Data**: Hadoop, Apache Spark, Apache Pig, Hive
- **Databases**: Snowflake, Exasol (In-Memory MPP), Traditional RDBMS
- **Programming**: Python, SQL, Lua Scripts
- **Data Integration**: Alteryx, Adobe APIs, ETL Pipelines
- **DevOps**: Terraform, GitHub CI/CD Workflows, Infrastructure as Code
- **Machine Learning**: PySpark, Topic Modeling, Text Classification
- **Current Role**: Lead Data Engineer at Kellanova (Fortune 500)

## 📁 Project Structure

```
rijul-portfolio/
├── 📄 index.html              # Main landing page
├── ☎️ contact                 #contact section
├── 📄 404.html                # Custom error page
├── 📄 manifest.json           # PWA configuration
├── 📄 sitemap.xml             # SEO sitemap
├── 📄 robots.txt              # Search engine directives
├── 📁 assets/
│   ├── 🎨 css/                # Stylesheets
│   ├── 🖼️ img/                # Images and icons
│   ├── ⚡ js/                 # JavaScript files
│   ├── 📚 vendor/             # Third-party libraries
│   └── 📋 Rijul_Sahu.pdf      # Resume/CV
└── 📁 projects/
    ├── 📊 Hadoop.html         # Big Data Analytics Project
    ├── 🔄 DI.html             # Data Integration Solution
    ├── 💾 Exasol.html         # CRM Analytics Automation
    ├── 🤖 Topic_Modeling.html # ML Text Classification
    └── 🏗️ Terraform.html      # Infrastructure as Code
```

## 🚀 Featured Projects

### 1. 📊 Big Data Analytics with Hadoop
**Challenge**: Process 6+ billion competitor pricing records for global analytics  
**Solution**: 6-node Hadoop cluster with Spark, Pig, and Hive  
**Impact**: 83% reduction in processing time, $150K annual savings

### 2. 🔄 Data Integration using Python & Alteryx
**Challenge**: Replace legacy Syntasa platform for Adidas/Reebok analytics  
**Solution**: Python + Alteryx pipeline with Adobe API integration  
**Impact**: Eliminated vendor dependency, 98% less manual intervention

### 3. 💾 Exasol CRM Analytics Automation
**Challenge**: Manual CRM reporting across multiple brands and regions  
**Solution**: Automated Lua scripts in Exasol in-memory database  
**Impact**: 91% time reduction (45 min → 4 min), 98% less manual work

### 4. 🤖 Topic Modeling & Text Classification
**Challenge**: Categorize large volumes of customer chat data  
**Solution**: PySpark-based ML pipeline with 85%+ accuracy  
**Impact**: 3-minute processing time, automated topic categorization

### 5. 🏗️ Terraform Infrastructure Automation
**Challenge**: Manual AWS resource deployment for European food delivery company  
**Solution**: Reusable Terraform templates for VPC, EC2, RDS deployment  
**Impact**: Full CI/CD DevOps implementation, eliminated manual errors

## 🌐 AWS Amplify Deployment Guide

### Prerequisites
- AWS Account with appropriate permissions
- Git repository (GitHub, GitLab, or Bitbucket)
- Domain name (optional, for custom domain)

### Step 1: Prepare Your Repository
```bash
# Clone the repository
git clone https://github.com/yourusername/rijul-portfolio.git
cd rijul-portfolio

# Ensure all files are committed
git add .
git commit -m "Ready for AWS Amplify deployment"
git push origin main
```

### Step 2: Create Amplify App
1. **Login to AWS Console**
   - Navigate to AWS Amplify service
   - Click "Get Started" under "Host your web app"

2. **Connect Repository**
   - Select your Git provider (GitHub/GitLab/Bitbucket)
   - Authorize AWS Amplify to access your repositories
   - Select your portfolio repository
   - Choose the `main` branch

### Step 3: Configure Build Settings
```yaml
# amplify.yml (auto-generated, but you can customize)
version: 1
frontend:
  phases:
    build:
      commands:
        - echo "No build process required for static site"
  artifacts:
    baseDirectory: /
    files:
      - '**/*'
  cache:
    paths: []
```

### Step 4: Deploy Configuration
1. **App Name**: `rijul-portfolio` (or your preferred name)
2. **Environment**: `production`
3. **Build Settings**: Use default (no build process needed)
4. **Advanced Settings**:
   - **Root Directory**: Leave empty (deploy from root)
   - **Build Command**: Not required
   - **Output Directory**: Not required

### Step 5: Custom Domain Setup (Optional)
1. **Add Domain**
   - Go to "Domain Management" in Amplify console
   - Click "Add domain"
   - Enter your domain (e.g., `rijul.cloud`)

2. **DNS Configuration**
   - Add CNAME record pointing to Amplify domain
   - Or use Route 53 for automatic DNS management

3. **SSL Certificate**
   - Amplify automatically provisions SSL certificates
   - HTTPS will be enabled by default

### Step 6: Environment Variables (If Needed)
```bash
# In Amplify Console > App Settings > Environment Variables
# Add any required environment variables
# (None required for this static site)
```

### Step 7: Monitoring & Analytics
1. **Enable Monitoring**
   - CloudWatch metrics automatically enabled
   - Monitor page views, performance, and errors

2. **Custom Headers** (Optional)
   ```json
   {
     "/**": {
       "headers": {
         "X-Frame-Options": "DENY",
         "X-Content-Type-Options": "nosniff",
         "Referrer-Policy": "strict-origin-when-cross-origin"
       }
     }
   }
   ```

## 🔧 Local Development

### Setup
```bash
# Clone the repository
git clone https://github.com/yourusername/rijul-portfolio.git
cd rijul-portfolio

# Serve locally (using Python)
python -m http.server 8000

# Or using Node.js
npx serve .

# Or using PHP
php -S localhost:8000
```

### File Structure Guidelines
- Keep all assets in the `assets/` directory
- Project pages go in the `projects/` directory
- Use relative paths for all internal links
- Optimize images for web (WebP format recommended)

## 📈 Performance Optimizations

### ✅ Implemented
- **Minified CSS/JS** - Reduced file sizes
- **Optimized Images** - Compressed project images
- **CDN Delivery** - AWS CloudFront integration via Amplify
- **Gzip Compression** - Automatic compression
- **Browser Caching** - Optimized cache headers
- **Progressive Web App** - Installable, offline-capable

### 🎯 SEO Features
- **Meta Tags** - Comprehensive SEO metadata
- **Structured Data** - Schema.org markup
- **Sitemap** - XML sitemap for search engines
- **Robots.txt** - Search engine directives
- **Open Graph** - Social media sharing optimization

## 🔒 Security Features

- **HTTPS Enforced** - SSL/TLS encryption
- **Security Headers** - XSS protection, content type validation
- **No Sensitive Data** - Client-side only, no backend secrets
- **Input Validation** - Sanitized contact forms

## 📊 Analytics & Monitoring

### AWS CloudWatch Metrics
- Page views and unique visitors
- Geographic distribution
- Device and browser analytics
- Performance metrics (load times)
- Error tracking and 404 monitoring

### Performance Benchmarks
- **Lighthouse Score**: 95+ (Performance, Accessibility, SEO)
- **Page Load Time**: < 2 seconds
- **First Contentful Paint**: < 1.5 seconds
- **Mobile Responsive**: 100% compatible

## 🤝 Contributing

While this is a personal portfolio, suggestions and improvements are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 💼 Current Role & Certifications

**Lead Data Engineer at Kellanova** (Fortune 500 Company)
- Leading data transformation initiatives and analytics platform development
- Architecting cloud-based data ecosystems using modern data stack
- Managing cross-functional teams and driving digital transformation projects

**Professional Certifications:**
- 🏆 **Databricks Certified Data Engineer Associate** (Expires September 1, 2027)
- 🏆 **AWS Certified Solutions Architect** (Expired, Preparing for Exam)

## 📞 Contact

**Rijul Sahu**  
🏢 **Current Role**: Lead Data Engineer at Kellanova  
🌐 **Website**: [rijul.cloud](https://rijul.cloud)  
💼 **LinkedIn**: [rijul-sahu](https://www.linkedin.com/in/rijul-sahu-242b59129/)  
📧 **Email**: [rijulsahu@duck.com](mailto:rijulsahu@duck.com) *(Business inquiries only)*  
🔗 **Stack Overflow**: [rijul-sahu](https://stackoverflow.com/users/2831370/rijul-sahu)  
🎯 **Career Goal**: Transitioning to Cloud Solutions Architect role

---

⭐ **Star this repository if you found it helpful!**

*Built with ❤️ using modern web technologies and deployed on AWS Amplify*