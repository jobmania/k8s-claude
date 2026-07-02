# 📘 AI 시대에 개발자가 알아야 할 인프라 구성 배포 with 클로드 코드

> **학습 기간:** 2026.06.25 ~ 7.26  
> **목표:** Claude Code와 AI 에이전트를 활용한 효율적인 클라우드 인프라 아키텍처 설계 및 배포 프로세스 마스터

---

## 📌 목차 (Chapters)

<details>
<summary><b>Chapter 1. AI 시대의 개발자와 인프라 패러다임의 변화</b></summary>
<div markdown="1">

### 🔑 핵심 요약
* AI 에이전트(Claude Code 등)가 인프라 구축 및 DevOps 환경에 미치는 영향
* 전통적인 인프라 관리와 AI 기반 자동화의 차이점

### 📝 주요 학습 내용
1. **Infrastructure as Code (IaC)와 AI의 시너지**
   * 내용을 적으세요.
2. **AI 도구를 활용한 트러블슈팅 효율화**
   * 내용을 적으세요.

### 💡 나만의 한 줄 노트
* _"AI는 도구일 뿐, 최종 인프라 구조의 무결성을 검증하는 것은 개발자의 몫이다."_

</div>
</details>

<details>
<summary><b>Chapter 2. 컨테이너 기반 인프라의 기초 (Docker & Kubernetes)</b></summary>
<div markdown="1">

### 📦 핵심 개념
* **Docker Compose:** 멀티 컨테이너 환경 격리 및 로컬 테스트 시스템 구축
* **Kubernetes:** 가용성과 확장성을 고려한 Pod, Deployment, Service 설계

### 🛠️ 실습 및 설정 코드
```yaml
# Claude Code가 추천한 로컬 k8s 배포 가계도 예시
apiVersion: apps/v1
kind: Deployment
metadata:
  name: backend-deployment
spec:
  replicas: 3
  template:
    spec:
      containers:
      - name: app
        image: my-backend-app:latest
