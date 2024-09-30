# AWS VPC 및 EKS 클러스터 템플릿

## 📋 개요
본 프로젝트는 AWS 인프라에서 VPC 및 EKS 클러스터를 구축하기 위한 CloudFormation 템플릿을 제공합니다. 아래와 같은 구성 요소를 포함합니다:

### 📌 VPC 및 네트워크 구성 (`cf_basic_infra.yaml`)
- **VPC**: 1개
- **Public 서브넷**: 2개
- **Private 서브넷**: 6개 (Frontend 2개, Backend 2개, Database 2개)
- **Internet Gateway**: 1개
- **NAT Gateway**: 1개

### 📌 EKS 클러스터 생성 (`create-ekcluster.yaml`)
- EKS 클러스터 배포를 위한 템플릿
- `cf_basic_infra.yaml` 템플릿을 사전 배포하고 필요한 ID 값을 추가하여 1개의 EKS 클러스터를 구성

### 📌 IP 구성
- **Public 서브넷**: 8,192 IP 주소
- **Private 서브넷**:
  - Frontend: 8,192 IP 주소
  - Backend: 8,192 IP 주소
  - Database: 2,048 IP 주소

## ⚠️ 참고 사항
- **ETEVERS-IDE**: 사전 생성된 IAM을 구성하고 코드 서버로 활용합니다.

