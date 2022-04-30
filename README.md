# Cloud Native Courses Roadmap

## Containers - Docker
### [x] Session 01: Containers 101
- https://kube.academy/courses/containers-101
- https://riptutorial.com/Download/docker.pdf

### [x] Session 02: Containers 101 - Docker Workshop
- WorkShop -> Mini Peoject (Deploy MERN App)
  - Container Security Explained
    - https://www.youtube.com/watch?v=b_euX_M82uI&ab_channel=IBMTechnology
  - Cloud Native Container
    - https://www.youtube.com/results?search_query=cloud+native+container
  - Cloud native Container Networking
  - What is a Container?
  - Intro to cloud native: What are containers?
  - Containerization Explained
  - Learn Cloud-Native Week 2: Intro to Containers
  - Cloud Native Container Security

## [!] Container Orchestration - Kubernetes 101
### [ ] Session 03: Container Orchestration - Kubernetes 101
- [!] Kubernetes Crash Course for Absolute Beginners: https://www.youtube.com/watch?v=s_o8dwzRlu4&ab_channel=TechWorldwithNana
- https://kube.academy/courses/kubernetes-101
- Kubernetes architecture explained: https://www.youtube.com/watch?v=HJ6F05Pm5mQ&list=PLpbcUe4chE79sB7Jg7B4z3HytqUUEwcNE&ab_channel=HoussemDellai
- Kubernetes Core Concepts: https://kube.academy/paths/kubernetes-core-concepts

## [!] Build Automation & CI/CD Pipeline - Jenkins
- [!] GitLab CI/CD
  - Mettez en place l'intégration et la livraison continues avec la démarche DevOps: https://openclassrooms.com/fr/courses/2035736-mettez-en-place-lintegration-et-la-livraison-continues-avec-la-demarche-devops
- Jenkins
  - Jenkines Pipeline Tutorials: https://www.youtube.com/playlist?list=PLy7NrYWoggjw_LIiDK1LXdNN82uYuuuiC
- GitHub Actions
  - GitHub Actions - Basic Concepts and CI/CD Pipeline with Docker: https://www.youtube.com/watch?v=R8_veQiYBjI&list=PLy7NrYWoggjzSIlwxeBbcgfAdYoxCIrM2&index=2&ab_channel=TechWorldwithNana
- TeamCity CI/CD
  - JetBrains TeamCity: https://www.youtube.com/watch?v=zqi4fDF-S60&list=PLy7NrYWoggjzSIlwxeBbcgfAdYoxCIrM2&index=2&ab_channel=TechWorldwithNana
- ArgoCD
  - Argo CD | GitOps CD for K8S: https://www.youtube.com/watch?v=MeU5_k9ssrs&list=PLy7NrYWoggjzSIlwxeBbcgfAdYoxCIrM2&index=9&t=2187s&ab_channel=TechWorldwithNana
- Azure DevOps
- AWS CodePipeline
  - https://docs.aws.amazon.com/whitepapers/latest/cicd_for_5g_networks_on_aws/cicd-on-aws.html
  - https://aws.amazon.com/getting-started/hands-on/set-up-ci-cd-pipeline/
  - https://www.youtube.com/watch?v=NwzJCSPSPZs&ab_channel=BlockExplorer

## [!] Infrastructure Provisioning & Configuration Management (IaC)
- [!] Ansible: https://www.youtube.com/watch?v=1id6ERvfozo&ab_channel=TechWorldwithNana
- [!] Terraform: https://www.youtube.com/watch?v=l5k1ai_GBDE&t=76s&ab_channel=TechWorldwithNana

## [!] AWS
- [!] AWS Certified Cloud Practitioner
  - AWS Cloud Practitioner Essentials: https://explore.skillbuilder.aws/
  - AWS Power Hour: Cloud Practitioner: https://pages.awscloud.com/global-traincert-twitch-power-hour-cloud-practitioner.html
  - https://aws.amazon.com/certification/certified-cloud-practitioner/?ch=sec&sec=rmg&d=1
- https://www.youtube.com/c/BeABetterDev
- https://www.youtube.com/channel/UCCYR9GpcE3skVnyMU8Wx1kQ
- https://www.youtube.com/channel/UCwpIueN8B-42Z8vfxVt0yEQ

## Azure

## Cloud Native
- https://www.youtube.com/watch?v=k-NXaFZ5lCU&ab_channel=Cookieconnect%C3%A9
- Understanding Cloud Native: https://kube.academy/paths/understanding-cloud-native
- Introduction to Building Cloud Native Applications: https://kube.academy/paths/introduction-to-building-cloud-native-applications

## Monitoring
- [!] Prometheus Monitoring Full Tutorial: https://www.youtube.com/playlist?list=PLy7NrYWoggjxCF3av5JKwyG7FFF9eLeL4

## Scripting Language
- [!] Golang Tutorial for Beginners | Full Go Course: https://www.youtube.com/watch?v=yyUHQIec83I&t=11154s&ab_channel=TechWorldwithNana

## Helps
sudo docker stop $(docker ps -qa); docker rm $(docker ps -qa); docker rmi -f $(docker images -qa); docker volume rm $(docker volume ls -q); docker network rm $(docker network ls -q) 2>/dev/null

