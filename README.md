# Terraform-EKS
## 특징
* IRSA를 이용하여 클러스터 내부에서 AWS의 오토 스케일링을 사용할 수 있게 했습니다.
* 아직 Ingress Controller를 구현하지는 못했지만, AWS의 ALB가 아닌 NLB를 이용하여 아키텍처를 구성했습니다.
* 보안을 위해 private 서브넷에서의 요청과 응답을 NAT gateway를 통해서만 주고 받을 수 있도록 했습니다. 
* 가용 영역 분산으로 가용성을 확보하도록 구성했습니다.

## 아키텍처
![Terraform-EKS 아키텍처](https://user-images.githubusercontent.com/47857304/212636826-dd2126ad-49a6-4f01-a3a4-0387ffd67928.png)

