# `컨테이너 인프라 환경 구축을 위한 쿠버네티스/도커` 헬름 차트 저장소

![img1](https://img.shields.io/badge/helm-3.x+%20-blue)
![img3](https://img.shields.io/badge/license-Apache%202-blue)

이 헬름 차트 저장소는 컨테이너 인프라 환경 구축을 위한 쿠버네티스/도커 책 실습에 사용되는 차트를 제공합니다.

🧰 제공하는 차트는 다음과 같습니다.


- MetalLB
- Jenkins
- Dashboard (블루그린)
- Prometheus
- Grafana

## 헬름 설치하기
헬름 설치는 [공식 문서](https://helm.sh/docs/intro/install/)를 참조하여 설치합니다.


## 헬름 차트 저장소 등록하기

```bash
$ helm repo add edu https://iac-source.github.io/helm-charts
$ helm repo update
```