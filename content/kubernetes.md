# Desafio Kubernetes

[`Kubernetes`](https://kubernetes.io/) atualmente é a principal ferramenta de orquestração e deployment de containers utilizado no mundo, praticamente tornando-se um padrão para abstração de recursos de infraestrutura.

Na maioria das empresas os serviços são containerizados e distribuídos em clusters para cada ambiente, sendo assim é importante que as aplicações sejam adaptáveis para cada ambiente e haja controle via código dos recursos kubernetes através de seus manifestos.

Aqui neste desafio trabalharemos com a aplicação [`PetClinic`](https://github.com/spring-projects/spring-petclinic). Essa aplicação é escrita em [`Spring Boot`](https://spring.io/projects/spring-boot), um framework open source.

### Objetivos

**Aplicação:**

* Criar uma pipeline de CI/CD contemplando `build` e `delivery` da aplicação. Fique à vontade para escolher a ferramenta de CI/CD;
* Criar os manifestos de recursos kubernetes para implantar a aplicação (deployment, service, ingress, configmap e/ou qualquer outro recurso que você considerar necessário);
* A aplicação precisa responder numa URL específicada no `Ingress`;

**Infraestrutura:**

* Fique à vontade para escolher como provisionar o cluster Kubernetes, pode utilizar small clusters como KinD, Minikube, K3D e afins;
* Para o DNS utilize o `/etc/hosts` do seu computador mesmo ou o serviço https://nip.io/.

### Extras

* Implante e instrumente observabilidade para as aplicações e para o seu cluster kubernetes, e.g. Prometheus, Grafana, Loki.
* Para o Load Balancing utilize soluções como o [`MetalLB`](https://metallb.universe.tf/), por exemplo.

Boa Implementação!
