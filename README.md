# 🚀 Snyk SCA GitHub Actions Demo

> **Lightning-fast dependency scanning integrated seamlessly into your CI/CD pipeline**

Transform your development workflow with **Snyk SCA** - the industry's leading Software Composition Analysis solution. This demo showcases how to integrate Snyk SCA into GitHub Actions for comprehensive open source vulnerability detection.

## ✨ Key Features

- ⚡ **Lightning Performance**: Sub-10 second dependency scans with real-time timing metrics
- 📊 **Beautiful Reports**: Stunning HTML reports with vulnerability details and remediation guidance
- 🛡️ **Enterprise Ready**: Configurable failure thresholds and regional API support
- 📱 **Developer Friendly**: Seamless integration with your existing workflow
- 🔍 **Comprehensive Coverage**: Scans all open source dependencies for known vulnerabilities

## 🚀 Quick Start

### 1. Get Your Demo Running
```bash
# Fork this repository or clone it
git clone https://github.com/your-username/snyk-sca-githubactions.git
```

### 2. 🔑 Configure Your Snyk Token
- 🌟 Get your free Snyk token from [app.snyk.io](https://app.snyk.io) → Account Settings
- 🔒 Add to GitHub Secrets: `Settings → Secrets → Actions → New repository secret`
  - **Name**: `SNYK_TOKEN`
  - **Value**: Your Snyk API token

### 3. 🌍 Regional Configuration (Critical!)
> ⚠️ **Important**: Set the correct regional API endpoint for your Snyk account

| Region | API Endpoint |
|--------|-------------|
| 🌍 **Global/Default** | `https://api.snyk.io` |
| 🇺🇸 **US** | `https://api.us.snyk.io` |
| 🇪🇺 **EU** | `https://api.eu.snyk.io` |
| 🇦🇺 **AU** | `https://api.au.snyk.io` |

**Configure in `.github/workflows/snyk-sca.yml`:**
```yaml
env:
  SNYK_API: https://api.snyk.io  # Update this!
```

### 4. 🔧 Optional: Enable Strict Mode
Want to fail builds on high/critical issues? Set:
```yaml
SNYK_SCA_FAIL_ON_ISSUES: true
```

### 5. 🎯 Watch the Magic
Push code or create a PR to trigger the workflow and see Snyk SCA in action!

## 🎯 What You'll See

### 📊 Real-Time Performance Metrics
```
🔥 SNYK SCA SCAN COMPLETED IN: 9 SECONDS 🔥
```

### 🐛 Sample Vulnerabilities Detected
This demo includes dependencies with known vulnerabilities for testing:

| Package | Vulnerability | Severity | CVE |
|---------|---------------|----------|-----|
| 🔴 **axios@0.21.0** | Server-Side Request Forgery | High | CVE-2020-28168 |
| 🔴 **lodash@4.17.19** | Prototype Pollution | High | CVE-2020-8203 |
| 🟡 **minimist@1.2.0** | Prototype Pollution | Medium | CVE-2020-7598 |
| 🟡 **tar@4.4.13** | Arbitrary File Overwrite | Medium | CVE-2021-32803 |

### 📱 Beautiful HTML Reports
- 📅 **Timestamped**: `repo-name-snyk-sca-report-20240115-143022.html`
- 🎨 **Interactive**: Click-through vulnerability details
- 🔧 **Actionable**: Clear remediation guidance
- 📥 **Downloadable**: Access from GitHub Actions artifacts

## 🔍 How It Works

1. **⚡ Lightning Setup**: Checkout code, install Snyk CLI, configure Node.js
2. **📦 Dependency Installation**: Install project dependencies
3. **🛡️ Security Scan**: Run Snyk SCA with real-time timing
4. **📊 Report Generation**: Create beautiful HTML reports with findings
5. **📤 Artifact Upload**: Make reports available for download

## 🎉 View Your Results

1. 🏃 **Go to Actions**: Navigate to your repository's Actions tab
2. 🎯 **Select Run**: Click on the latest workflow run
3. 📥 **Download**: Grab the HTML report from the artifacts section (downloads as a zip file)
4. 📂 **Extract**: Unzip the downloaded file to access the HTML report
5. 🔍 **Explore**: Open the HTML file in your browser to see detailed vulnerability analysis

---

## 🎬 **[👀 VIEW LIVE DEMO →](https://github.com/markusweldon/snyk-sca-githubactions/actions)**

See Snyk SCA in action! Check out recent workflow runs and download sample HTML reports.

---

## 🚀 Ready to Get Started?

**[Fork this repository](https://github.com/markusweldon/snyk-sca-githubactions/fork)** and experience the power of Snyk SCA in your CI/CD pipeline today!

> 💡 **Pro Tip**: Star this repository to keep it handy for future reference!