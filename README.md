# Claude Code를 활용한 AWS 인프라 관리 및 코드형 인프라(IaC) 워크샵

## 워크샵 목적

AI 에이전틱 코딩 도구인 Claude Code와 Amazon Bedrock을 활용하여, Terraform 기반의 컨테이너 인프라를 설계부터 배포, 최적화까지 전 과정을 실습합니다. 참가자는 자연어만으로 프로덕션 수준의 IaC 코드를 생성하고, MCP(Model Context Protocol)를 통해 최신 공식 문서를 실시간 참조하며, 반복적인 인프라 작업을 AI에게 위임하는 워크플로우를 체험합니다.

## 수행 과제

| 단계 | 과제 | 설명 |
|------|------|------|
| 1 | Claude Code 환경 설정 | 설치, AWS 인증, Amazon Bedrock 연동 |
| 2 | SKILL.md 작성 | 프로젝트 규칙과 모범 사례를 AI에게 가르치는 Skill 파일 생성 |
| 3 | MCP 서버 연결 | Terraform Registry, AWS ECS, AWS Documentation MCP 서버 구성 |
| 4 | 인프라 템플릿 생성 및 배포 | VPC, ECS Cluster를 Terraform 모듈로 설계하고 배포 |
| 5 | 컨테이너 애플리케이션 배포 | ECR 이미지 빌드/푸시, ECS Fargate 멀티 서비스(Cats & Dogs) 배포 |
| 6 | 비용 최적화 및 아키텍처 개선 | AI 기반 비용 분석, Fargate Spot, 모니터링 구성 |

## 사전 지식

- AWS 기본 서비스 경험 (VPC, EC2, IAM 수준)
- 터미널/CLI 기본 사용법
- 컨테이너(Docker) 기초 개념
- Terraform 기초 (선택 — 경험이 없어도 실습 가능)

## 소요 시간

약 **3시간**

## 습득 역량

워크샵을 완료하면 다음 역량을 습득합니다:

- Claude Code를 활용한 Terraform 코드 생성 및 검증 워크플로우
- Amazon Bedrock 기반 AI 에이전트 환경 구성 방법
- SKILL.md를 통한 AI 에이전트 커스터마이징 기법
- MCP 프로토콜을 활용한 외부 도구 연동 (Terraform Registry, AWS 서비스)
- Terraform 모듈 설계 모범 사례 (인프라/애플리케이션 분리, DRY 원칙)
- ECS Fargate 기반 멀티 서비스 아키텍처 설계 및 배포
- ALB 경로 기반 라우팅과 Step Scaling Auto Scaling 구성
- AI를 활용한 인프라 비용 분석 및 아키텍처 개선 프로세스

## 교재

- [workshop-claude-code-iac.md](workshop-claude-code-iac.md) — 워크샵 본문

## 참고 리소스

- [Claude Code 공식 문서](https://docs.anthropic.com/en/docs/claude-code/overview)
- [Terraform AWS Provider 모범 사례](https://docs.aws.amazon.com/prescriptive-guidance/latest/terraform-aws-provider-best-practices/introduction.html)
- [Amazon ECS 모범 사례](https://docs.aws.amazon.com/AmazonECS/latest/bestpracticesguide/intro.html)
- [HashiCorp Terraform MCP Server](https://github.com/hashicorp/terraform-mcp-server)
- [AWS MCP Servers](https://awslabs.github.io/mcp/)
- [ECS Cats & Dogs 샘플 앱](https://github.com/solminkim/ecs-cats-dogs)


## 제작 도구

<img src="assets/kiro-color.png" alt="Kiro" width="120" />

본 워크샵 교재는 [Kiro](https://kiro.dev)로 작성되었으며, HITL(Human-in-the-Loop) 방식으로 검증되었습니다.
