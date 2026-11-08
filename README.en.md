**English** | [한국어](README.md)

# AWS Infrastructure Management and Infrastructure as Code (IaC) Workshop with Claude Code

## Workshop Overview

A hands-on workshop in which you design, deploy, and optimize Terraform-based container infrastructure from start to finish, using Claude Code, an agentic AI coding tool, together with Amazon Bedrock. Participants generate production-grade IaC code from natural language alone, refer to the latest official documentation in real time through MCP (Model Context Protocol), and experience a workflow in which repetitive infrastructure tasks are delegated to AI.

## Workshop Objectives

- Build an AI-powered infrastructure automation environment by integrating Claude Code with Amazon Bedrock
- Build AWS container infrastructure following Terraform module design best practices
- Deploy and operate a multi-service application (Cats & Dogs) on ECS Fargate
- Experience a cost analysis and architecture improvement process powered by AI

## Target Audience

- Beginner to intermediate engineers with AWS experience
- DevOps/SRE engineers interested in infrastructure automation with AI tools
- Cloud engineers who want to improve their Terraform-based IaC workflow

## Prerequisites

- Experience with basic AWS services (VPC, EC2, IAM level)
- Basic terminal/CLI usage
- Basic container (Docker) concepts
- Terraform basics (optional — you can complete the lab without prior experience)

## Skills You Will Gain

- A workflow for generating and validating Terraform code with Claude Code
- How to configure an AI agent environment on Amazon Bedrock
- How to customize an AI agent with SKILL.md
- Integrating external tools through the MCP protocol (Terraform Registry, AWS services)
- Understanding the core Terraform concepts (Provider, State, Plan/Apply, Module, HCL)
- Terraform module design best practices (separating infrastructure and application, the DRY principle)
- Designing and deploying a multi-service architecture on ECS Fargate
- Configuring ALB path-based routing and Step Scaling Auto Scaling
- A process for analyzing infrastructure cost and improving the architecture with AI

## Workshop Lab Outline

> **How to follow the lab:** Open [`workshop-claude-code-iac.en.md`](workshop-claude-code-iac.en.md) and follow the text, commands, and example code of each step in the order of the outline below.

| Step | Lab | Description |
|------|-----|-------------|
| 1 | [Install Claude Code](workshop-claude-code-iac.en.md#1-install-claude-code) | Introduction to Claude Code, installation, and basic usage |
| 2 | [Configure AWS Authentication](workshop-claude-code-iac.en.md#2-configure-aws-authentication) | Set up AWS credentials and integrate with Terraform |
| 3 | [Configure the Bedrock LLM](workshop-claude-code-iac.en.md#3-configure-the-bedrock-llm) | Connect Amazon Bedrock models and verify the connection |
| 4 | [Create SKILL.md](workshop-claude-code-iac.en.md#4-create-skillmd--aws--terraform--container) | Give the AI agent your project rules and best practices |
| 5 | [Connect MCP Servers](workshop-claude-code-iac.en.md#5-connect-mcp-servers) | Set up the Terraform Registry, AWS ECS, and AWS Documentation MCP servers |
| 6 | [Create and Deploy the Infrastructure with Terraform](workshop-claude-code-iac.en.md#6-create-and-deploy-the-infrastructure-with-terraform) | Design the VPC and ECS Cluster as Terraform modules and deploy them |
| 7 | [Create and Deploy the Container Application with Terraform](workshop-claude-code-iac.en.md#7-create-and-deploy-the-container-application-with-terraform) | Build and push ECR images, and deploy the ECS Fargate multi-service (Cats & Dogs) application |
| 8 | [Cost Optimization and Architecture Improvements](workshop-claude-code-iac.en.md#8-cost-optimization-and-architecture-improvements) | AI-based cost analysis, Fargate Spot, and suggestions for production readiness |

## Duration

About **3 hours**

## References

| Topic | Link |
|-------|------|
| Claude Code official documentation | https://docs.anthropic.com/en/docs/claude-code/overview |
| Terraform AWS Provider best practices | https://docs.aws.amazon.com/prescriptive-guidance/latest/terraform-aws-provider-best-practices/introduction.html |
| Terraform code structure best practices | https://docs.aws.amazon.com/prescriptive-guidance/latest/terraform-aws-provider-best-practices/structure.html |
| Amazon ECS best practices | https://docs.aws.amazon.com/AmazonECS/latest/bestpracticesguide/intro.html |
| AWS VPC security best practices | https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-best-practices.html |
| HashiCorp Terraform MCP Server (official, container image) | https://github.com/hashicorp/terraform-mcp-server |
| Terraform MCP Server (third-party, npx package) | https://github.com/thrashr888/terraform-mcp-server |
| AWS MCP Servers | https://awslabs.github.io/mcp/ |
| ECS Cats & Dogs sample app | https://github.com/solminkim/ecs-cats-dogs |

---

## License

This workshop material is released under the [MIT License](LICENSE). You are free to use, modify, and redistribute it.

---

## Built With

This workshop material was written with <img src="assets/kiro-color.png" alt="Kiro" width="20" style="vertical-align: middle;" /> [Kiro](https://kiro.dev) and validated with a HITL (Human-in-the-Loop) approach.
