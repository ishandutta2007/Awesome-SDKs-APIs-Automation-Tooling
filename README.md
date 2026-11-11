# Awesome-SDKs-APIs-Automation-Tooling

# Awesome SDKs, APIs & Automation Tooling

> A curated list of top SDK, API, and Automation Tooling platforms — both SaaS/Hosted commercial developer platforms and open-source alternatives for building, testing, and automating software delivery and infrastructure.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Druva Developer Portal](#druva-developer-portal)
  - [GitHub Developer Platform](#github-developer-platform)
  - [GitLab Developer Platform](#gitlab-developer-platform)
  - [Postman](#postman)
  - [AWS Developer Tools](#aws-developer-tools)
  - [Azure DevOps](#azure-devops)
  - [CircleCI](#circleci)
- [Open-Source Software](#-open-source-software)
  - [HashiCorp Terraform](#hashicorp-terraform)
  - [OpenTofu](#opentofu)
  - [Pulumi](#pulumi)
  - [Jenkins](#jenkins)
  - [Hoppscotch](#hoppscotch)
  - [API Dash](#api-dash)
  - [Oriel](#oriel)
  - [Pipewright](#pipewright)
  - [Microcks](#microcks)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted SDK, API, and Automation Tooling platforms. These are not open-source but are included as reference points for feature comparison.

### Druva Developer Portal
**Type:** Data protection API and integration ecosystem
Druva's Developer Portal provides comprehensive REST API documentation for all Druva products, webhook configurations for event-driven notifications, and developer guides covering authentication, rate limits, and building best practices [citation:1]. A **Developer Sandbox** allows risk-free testing and validation of scripts before going live, simulating complete data protection workflows without affecting production data [citation:1]. The Marketplace serves as the integration hub, bridging Druva with Splunk, Microsoft Sentinel, Okta, ServiceNow, and other IT stack tools through pre-integrated apps and custom API solutions [citation:1].
**Best for:** Druva customers wanting to build custom integrations or automate data protection workflows via REST API and webhooks.

### GitHub Developer Platform
**Type:** Code hosting, CI/CD, and extensive API ecosystem
GitHub provides the most widely adopted developer platform, with REST and GraphQL APIs, GitHub Apps for granular integrations, Actions for CI/CD automation, and a massive marketplace of third-party tools. The platform is the de facto standard for open-source collaboration and source control, with native integration into virtually every development tool.

### GitLab Developer Platform
**Type:** Integrated DevSecOps with built-in CI/CD
GitLab provides a complete DevSecOps platform with built-in CI/CD, container registry, security scanning, and issue tracking. Its API-first design and self-managed option make it a strong choice for organizations wanting an integrated platform without stitching together multiple vendors.

### Postman
**Type:** API development and testing platform
Postman is the most widely adopted API client, offering request building, collection management, environment variables, mock servers, and automated testing via Newman CLI. It has evolved into a full API lifecycle platform with documentation, monitoring, and team collaboration features [citation:2].
**Best for:** Teams wanting a comprehensive, established API development platform with broad ecosystem support.

### AWS Developer Tools
**Type:** Integrated CI/CD and infrastructure tooling
AWS provides a suite of developer tools including CodeCommit (Git hosting), CodeBuild (CI), CodeDeploy (CD), CodePipeline (orchestration), and CloudFormation (IaC). Deeply integrated with AWS services and IAM, it is the natural choice for AWS-centric organizations.

### Azure DevOps
**Type:** Integrated DevOps platform
Azure DevOps provides Azure Repos (Git/TFVC), Azure Pipelines (CI/CD), Azure Boards (work tracking), and Azure Artifacts (package management). It integrates natively with the Microsoft ecosystem and supports both cloud and on-premises deployment.

### CircleCI
**Type:** Cloud-native CI/CD with Docker support
CircleCI is a cloud-native CI/CD platform known for its Docker layer caching and parallelism capabilities [citation:25]. It supports GitHub and Bitbucket integration, with configuration via YAML and extensive orbs for reusable pipeline components.

---

## 🟩 Open-Source Software

Self-hosted, community-driven SDK, API, and Automation Tooling. The open-source ecosystem spans **Infrastructure as Code engines**, **CI/CD platforms**, **API clients**, and **specialized automation tools**.

### HashiCorp Terraform
**Stack:** Go / HCL | **License:** Business Source License (BSL) 1.1
Terraform is the de facto standard for Infrastructure as Code, enabling declarative provisioning across any cloud provider with 3,000+ providers [citation:25]. It uses HashiCorp Configuration Language (HCL) to define infrastructure, with state management, planning, and apply workflows [citation:3]. **Important licensing note:** Terraform changed to the Business Source License in 2023, which is not OSI-approved open source and restricts certain commercial uses [citation:18]. The open-source edition is free for most internal use cases [citation:3].
**Best for:** Teams wanting the largest ecosystem and community support for IaC, accepting the BSL licensing terms.

### OpenTofu
**Stack:** Go / HCL | **License:** MPL 2.0
OpenTofu is the open-source fork of Terraform created after Terraform's license change, now under the Linux Foundation and CNCF Sandbox [citation:18][citation:25]. It maintains compatibility with Terraform's HCL configuration and provider ecosystem while remaining genuinely open source under MPL 2.0. For organizations where license matters, OpenTofu is the direct replacement.
**Best for:** Teams wanting Terraform-compatible IaC under a permissive open-source license with community governance.

### Pulumi
**Stack:** Go / TypeScript / Python / C# / Java | **License:** Apache 2.0
Pulumi enables Infrastructure as Code using real programming languages (TypeScript, Python, Go, C#, Java) instead of a domain-specific configuration language [citation:25]. It supports all major cloud providers and can even run HCL programs via a language plugin [citation:18]. Teams already comfortable with general-purpose languages can write reusable abstractions, unit tests, and leverage existing tooling (autocomplete, debugging, linting) [citation:18]. `pulumi convert --from terraform` enables migration from existing Terraform configurations [citation:18].
**Best for:** Software engineering teams wanting IaC in their primary language with strong testing and abstraction capabilities.

### Jenkins
**Stack:** Java | **License:** MIT
Jenkins is the long-standing open-source automation server with 1,800+ plugins for building, testing, and deploying code [citation:25]. It supports Pipeline as Code (Jenkinsfile), distributed builds, and extensive integrations [citation:19]. While newer platforms offer more modern UX, Jenkins remains the most extensible and widely deployed CI/CD server, particularly in enterprise environments [citation:27].
**Best for:** Organizations wanting maximum extensibility and a proven, community-driven CI/CD server.

### Hoppscotch
**Stack:** TypeScript / Vue | **License:** MIT
Hoppscotch is a lightweight, open-source API development ecosystem positioned as a Postman alternative. It supports REST, GraphQL, WebSocket, SSE, and MQTT, with a web app, desktop app (Tauri), and PWA. Features include collections, environments, pre-request scripts, and self-hosting options [citation:2]. The free tier remains available, and self-hosting is supported.
**Best for:** Teams wanting a fast, open-source API client with broad protocol support and no vendor lock-in.

### API Dash
**Stack:** Flutter | **License:** Open Source
API Dash is a beautiful AI-powered open-source cross-platform (Desktop & Mobile) API client for testing, visualizing, and integrating APIs. It supports HTTP and GraphQL requests, visual response inspection, and API integration code generation. Positioned as a lightweight alternative to Postman and Insomnia, with 2,900+ GitHub stars [citation:26].
**Best for:** Developers wanting a modern, cross-platform API client with AI-assisted code generation and a lightweight footprint.

### Oriel
**Stack:** Go | **License:** Apache 2.0
Oriel is a small, local GUI for Colima and Docker, positioned as an open-source Docker Desktop alternative. It manages containers, images, volumes, networks, and Compose stacks from a browser UI, using only 15-30 MB of RAM with no Electron. It also functions as an **MCP server**, allowing AI clients (Claude, Cursor) to manage Docker through validated, secret-masked tools with destructive actions gated [citation:6].
**Best for:** Developers wanting a lightweight Docker Desktop alternative with AI agent accessibility via MCP.

### Pipewright
**Stack:** Go | **License:** Open Source
Pipewright is a lightweight self-hosted CI/CD, deployment, and ops platform in a single Go binary with zero runtime dependencies [citation:12]. Features include pipeline-as-code via `.pipewright.yml` (GitOps), DORA metrics (deployment frequency, lead time, change failure rate, MTTR), optional AI assist for failure diagnosis, container management, and multi-host ops [citation:5][citation:12]. It requires Docker for isolated builds but degrades gracefully without it [citation:12].
**Best for:** Teams wanting a self-hosted CI/CD platform with built-in ops monitoring and DORA metrics without the complexity of Jenkins or the cost of cloud CI.

### Microcks
**Stack:** Java / Kubernetes | **License:** Apache 2.0
Microcks is a CNCF incubating project for API mocking and testing, supporting OpenAPI, AsyncAPI, gRPC, GraphQL, Postman collections, and SOAP [citation:7]. It turns API contracts into live mock servers and powers contract conformance tests against real implementations. With 2.5M+ container downloads in 2025 and adoption by BNP Paribas, Société Générale, and Deloitte, it is a mature choice for API-first teams [citation:7].
**Best for:** Teams practicing API-first development wanting to mock and test APIs across multiple protocols in Kubernetes-native environments.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Category | Self-Hosted | Best For |
|----------|---------|-------|----------|-------------|----------|
| **Druva Developer Portal** | Proprietary | Cloud | Data protection API | ❌ | Druva integrations |
| **GitHub** | Proprietary | Cloud | Code + CI/CD | ❌ | Universal developer platform |
| **GitLab** | Proprietary | Cloud/on-prem | DevSecOps | (Self-managed) | Integrated DevSecOps |
| **Postman** | Proprietary | Cloud/Desktop | API client | ❌ | Comprehensive API platform |
| **Terraform** | BSL 1.1 | Go/HCL | IaC | ✅ | Largest IaC ecosystem |
| **OpenTofu** | MPL 2.0 | Go/HCL | IaC | ✅ | OSS Terraform fork |
| **Pulumi** | Apache 2.0 | Multi-language | IaC | ✅ | IaC in real languages |
| **Jenkins** | MIT | Java | CI/CD | ✅ | Maximum extensibility |
| **Hoppscotch** | MIT | TypeScript | API client | ✅ | Lightweight Postman alt |
| **API Dash** | Open Source | Flutter | API client | ✅ | Cross-platform + AI |
| **Oriel** | Apache 2.0 | Go | Docker GUI + MCP | ✅ | Lightweight Docker Desktop alt |
| **Pipewright** | Open Source | Go | CI/CD + Ops | ✅ | Self-hosted CI/CD + DORA |
| **Microcks** | Apache 2.0 | Java/K8s | API mocking | ✅ | Multi-protocol API testing |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source SDK, API, or Automation Tooling platform that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source (or clearly note if it is source-available but not OSI-approved, as with Terraform's BSL). Note that the ecosystem **splits** across **Infrastructure as Code** (Terraform, OpenTofu, Pulumi), **CI/CD** (Jenkins, Pipewright), **API clients** (Hoppscotch, API Dash), and **specialized tooling** (Oriel for Docker/MCP, Microcks for API mocking). **OpenTofu** and **Pulumi** are the primary open-source alternatives to Terraform, with OpenTofu offering the most direct migration path and Pulumi offering a fundamentally different approach using general-purpose languages [citation:18][citation:25].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
