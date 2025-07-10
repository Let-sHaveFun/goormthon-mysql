# goormthon-mysql
이 디렉토리는 Kubernetes 환경에서 MySQL 데이터베이스를 배포하기 위한 Kustomize 구성을 포함합니다.

## 구조
- `base/`: 기본 Kubernetes 리소스 정의
- `overlays/`: 환경별 설정 오버레이

## 배포 방법
```bash
# Base 배포
kubectl apply -k database/mysql/base

# Overlay 배포
kubectl apply -k database/mysql/overlays
```