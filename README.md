# 개요
blog 프로젝트에서 사용하는 K8S iac 프로젝트 입니다.

## 앱 레포지토리
* [blog-api](https://github.com/narumir/blog-api)
* [blog-web](https://github.com/narumir/blog-web)

## 설치된 도구 목록
* [ingress-nginx](https://kubernetes.github.io/ingress-nginx/)
* [cert-manager](https://cert-manager.io/)
* [grafana](https://grafana.com/) (link: [grafana.narumir.io](https://grafana.narumir.io))
* [prometheus](https://prometheus.io/)
* [argocd](https://argoproj.github.io/cd/) (link: [argocd.narumir.io](https://argocd.narumir.io))

## 서버 구조
![server-structure](./docs/resources/server-structure.png)

### IP 주소

name              | ip address     | description
------------------|----------------|----------------------
router            | 192.168.50.1   | NAT Router
HAProy            | 192.168.50.102 | external loadbalancer
K8S Control Plane | 192.168.50.120 | control plance
K8S Node 1        | 192.168.50.121 | node 1
K8S Node 2        | 192.168.50.122 | node 2
K8S Node 3        | 192.168.50.123 | node 3

