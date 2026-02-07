# Minecraft-Bedrock-Version

> **2026-W Project**
> 박혜수(PM), 양유상, 윤주혁, 이제혁, 이제희, 정재성

---

## 프로젝트 개요

본 프로젝트는 클라우드 환경에서 생성 예정인 인프라에 대해 CLI 기반으로 **사전에 공격 경로를 예측**하고, 이를 구축하는 데 필요한 **최소 권한 IAM 정책을 AI가 자동 제안**함으로써 보안 중심의 인프라 변경 통제를 구현하는 시스템입니다.

<img width="1372" height="498" alt="image" src="https://github.com/user-attachments/assets/7c7fa375-c473-43de-96d8-dc2fd3cc2a81" />
<br>

**공격 경로 예측** : 기존 인프라를 그래프 형태로 모델링한 후, 생성 예정인 인프라를 가상 노드로 추가하여 연결 관계를 확장합니다. 이후 새롭게 도출된 인프라 노드의 접근 경로를 임베딩하여, 공격 시나리오가 저장된 벡터 DB와 RAG 방식으로 비교·분석하여 수행됩니다.

**최소 권한 IAM 정책** : AI가 제안한 정책은 사용자의 최종 승인 절차를 거칩니다. 이후 자격 증명 생성 → 인프라 생성 → 사용된 자격 증명 삭제로 이어지는 보안 중심의 Workflow를 구현합니다.

<img width="1372" alt="image" src="https://github.com/user-attachments/assets/714ebd4c-4709-4091-b030-198f6975ba42" />


---

## 프로젝트 목표

- 생성 예정 인프라에 대한 공격 경로 사전 예측 (Attack Graph)
- 인프라 생성을 위한 AWS CLI 명령어 자동 생성
- CLI 실행에 필요한 최소 권한 IAM 정책(JSON) 자동 생성
- 사용자 승인 기반의 인프라 변경 통제 프로세스 구현
- 자격 증명 및 CLI 사용 로그를 기반으로 한 비정상 행위 탐지

---

## WBS (수정 및 진행 중)

<img width="1308" height="705" alt="image" src="https://github.com/user-attachments/assets/47384559-15c9-4b26-ba20-50b7f5d03fa3" />

