[English](README.en.md) | **한국어**

# Claude Code를 활용한 AWS 인프라 관리 및 코드형 인프라(IaC) 워크샵

## 워크샵 개요

AI 에이전틱 코딩 도구인 Claude Code와 Amazon Bedrock을 활용하여, Terraform 기반의 컨테이너 인프라를 설계부터 배포, 최적화까지 전 과정을 실습하는 핸즈온 워크샵입니다. 참가자는 자연어만으로 프로덕션 수준의 IaC 코드를 생성하고, MCP(Model Context Protocol)를 통해 최신 공식 문서를 실시간 참조하며, 반복적인 인프라 작업을 AI에게 위임하는 워크플로우를 체험합니다.

## 워크샵 목표

- Claude Code와 Amazon Bedrock을 연동하여 AI 기반 인프라 자동화 환경을 구축한다
- Terraform 모듈 설계 모범 사례에 따라 AWS 컨테이너 인프라를 구성한다
- ECS Fargate 기반 멀티 서비스 애플리케이션(Cats & Dogs)을 배포하고 운영한다
- AI를 활용한 비용 분석 및 아키텍처 개선 프로세스를 경험한다

## 대상 참가자

- AWS 경험이 있는 초중급 엔지니어
- AI 도구를 활용한 인프라 자동화에 관심 있는 DevOps/SRE 엔지니어
- Terraform 기반 IaC 워크플로우를 개선하고자 하는 클라우드 엔지니어

## 사전 지식

- AWS 기본 서비스 경험 (VPC, EC2, IAM 수준)
- 터미널/CLI 기본 사용법
- 컨테이너(Docker) 기초 개념
- Terraform 기초 (선택 — 경험이 없어도 실습 가능)

## 워크샵 완료 시 습득 역량

- Claude Code를 활용한 Terraform 코드 생성 및 검증 워크플로우
- Amazon Bedrock 기반 AI 에이전트 환경 구성 방법
- SKILL.md를 통한 AI 에이전트 커스터마이징 기법
- MCP 프로토콜을 활용한 외부 도구 연동 (Terraform Registry, AWS 서비스)
- Terraform의 핵심 개념(Provider, State, Plan/Apply, Module, HCL) 이해
- Terraform 모듈 설계 모범 사례 (인프라/애플리케이션 분리, DRY 원칙)
- ECS Fargate 기반 멀티 서비스 아키텍처 설계 및 배포
- ALB 경로 기반 라우팅과 Step Scaling Auto Scaling 구성
- AI를 활용한 인프라 비용 분석 및 아키텍처 개선 프로세스

## 워크샵 실습 목차

> **실습 방법:** [`workshop-claude-code-iac.md`](workshop-claude-code-iac.md) 파일을 열어, 아래 목차 순서에 맞춰 각 단계의 본문·명령어·예제 코드를 그대로 따라 진행하세요.

| 단계 | 실습 내용 | 설명 |
|------|-----------|------|
| 1 | [Claude Code 설치](workshop-claude-code-iac.md#1-claude-code-설치) | Claude Code 소개, 설치 및 기본 사용법 |
| 2 | [AWS 인증 구성](workshop-claude-code-iac.md#2-aws-인증-구성) | AWS 자격 증명 설정 및 Terraform 연동 |
| 3 | [Bedrock LLM 사용 설정](workshop-claude-code-iac.md#3-bedrock-llm-사용-설정) | Amazon Bedrock 모델 연동 및 연결 확인 |
| 4 | [SKILL.md 생성](workshop-claude-code-iac.md#4-skillmd-생성--aws--terraform--container) | AI 에이전트에 프로젝트 규칙과 모범 사례 주입 |
| 5 | [MCP 서버 연결 구성](workshop-claude-code-iac.md#5-mcp-서버-연결-구성) | Terraform Registry, AWS ECS, AWS Documentation MCP 서버 구성 |
| 6 | [인프라 Terraform 템플릿 생성 및 배포](workshop-claude-code-iac.md#6-인프라-terraform-템플릿-생성-및-배포) | VPC, ECS Cluster를 Terraform 모듈로 설계하고 배포 |
| 7 | [Container 기반 애플리케이션 배포](workshop-claude-code-iac.md#7-container-기반-애플리케이션-배포를-위한-terraform-템플릿-생성-및-배포) | ECR 이미지 빌드/푸시, ECS Fargate 멀티 서비스(Cats & Dogs) 배포 |
| 8 | [비용 최적화 및 아키텍처 개선](workshop-claude-code-iac.md#8-비용-최적화-및-아키텍처-개선) | AI 기반 비용 분석, Fargate Spot, 프로덕션 개선 제안 |

## 소요 시간

약 **3시간**

## 참고 자료

| 주제 | 링크 |
|------|------|
| Claude Code 공식 문서 | https://docs.anthropic.com/en/docs/claude-code/overview |
| Terraform AWS Provider 모범 사례 | https://docs.aws.amazon.com/prescriptive-guidance/latest/terraform-aws-provider-best-practices/introduction.html |
| Terraform 코드 구조 모범 사례 | https://docs.aws.amazon.com/prescriptive-guidance/latest/terraform-aws-provider-best-practices/structure.html |
| Amazon ECS 모범 사례 | https://docs.aws.amazon.com/AmazonECS/latest/bestpracticesguide/intro.html |
| AWS VPC 보안 모범 사례 | https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-best-practices.html |
| HashiCorp Terraform MCP Server (공식, 컨테이너 이미지) | https://github.com/hashicorp/terraform-mcp-server |
| Terraform MCP Server (서드파티, npx 패키지) | https://github.com/thrashr888/terraform-mcp-server |
| AWS MCP Servers | https://awslabs.github.io/mcp/ |
| ECS Cats & Dogs 샘플 앱 | https://github.com/solminkim/ecs-cats-dogs |

---

## 라이선스

이 워크샵 교재는 [MIT License](LICENSE)로 배포됩니다. 자유롭게 사용, 수정, 재배포할 수 있습니다.

---

## 제작 도구

본 워크샵 교재는 <img src="assets/kiro-color.png" alt="Kiro" width="20" style="vertical-align: middle;" /> [Kiro](https://kiro.dev)로 작성되었으며, HITL(Human-in-the-Loop) 방식으로 검증되었습니다.
