# 도커를 활용하는 클라우드 서비스에 대해 알아보자!

## 컨테이너 오케스트레이션 기능

- 컨테이너 클러스터링(Container Clustering)
- 서비스 디스커버리(Service Discovery)
- 자동 스케일링(Autoscaling)
- 로드 밸런싱(Load Balancing)
- 롤아웃과 롤백(Rollout and Rollback)
- 자동 복구(Automatic Recovery)
- 모니터링과 로깅(Monitoring and Logging)
- 보안과 네트워크 관리(Security and Network Management)

## 대표적인 컨테이너 오케스트레이션 툴/서비스

### Docker Swarm

- 쿠버네티스가 등장하기 전까지 가장 대중적인 컨테이너 오케스트레이션 도구 중 하나
- 간단하게 작동하며 설정이 쉬움

### Kubernetes

- 구글에서 대용량 트래픽을 감당하기 위해 개발
- 대규모에 적합 (스케일링 기능 강화, 서비스 디스커버리 기능 강화)
- 가장 기능이 많음
- 다양한 환경에서 작동 가능

### GKE(Google Kubernetes Engine)

- GCP에서 제공하는 Kubernetes기반의 관리형 오케스트레이션 서비스
- Kubernetes의 기능을 모두 제공

### EKS (Amazon Elastic Kubernetes Service)

- AWS에서 제공하는 관리형 Kubernetes 서비스
- Kubernetes API를 통해 EKS 클러스터 관리 가능

### ECS (Amazon Elastic Container Service)

- AWS에서 제공하는 관리형 컨테이너 오케스트레이션 서비스
- Docker 컨테이너를 실행하기 위한 기능 제공

## ECS 서비스 종류(호스트 유형)

### EC2

- 컨테이너가 운영되는 자원이 EC2
- Capacity Providers를 통해 EC2 Auto-ScalingGroup을 연결

### Fargate (편리함)

- 서버리스 유형
- EC2 배포 및 관리가 필요없음
- 컨테이너도 어디서 운영되는지 관리할 필요없음

### External

- AWS 인프라가 아닌 자원의 호스트를 붙이는 서비스
- 실제 서비스는 AWS 밖에서 동작하며, 모니터링만 AWS 콘솔에서 관리
  EC2가 더 저렴할까?
