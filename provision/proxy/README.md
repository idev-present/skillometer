# Proxy

## Dependencies
- [flannel](https://github.com/flannel-io/flannel) - интерфейс сети контейнеров, назначает Pod-ам IP-адреса для их взаимодействия между друг другом.
- [MetalLB](https://metallb.universe.tf/) — LoadBalancer, который будет использоваться для выдачи внешних IP-адресов из заданного нами пула.
- [cert-manager](https://cert-manager.io/docs/installation/helm/) - менеджер сертификатов

## Install
1. [metallb](https://metallb.universe.tf/installation/#installation-with-helm) by helm official chart
2. `kubectl apply -f clusters/skillometer/proxy/ip-loadbalancer.yaml` - setup ip load balancer
3. `kubectl apply -f clusters/skillometer/proxy/ssl/secret.yaml` - dns resolver secrets for traefik
4. `kubectl apply -f clusters/skillometer/proxy/ssl/ssl-issuer.yaml` - cert issuer
5. `kubectl apply -f clusters/skillometer/proxy/ssl/ssl-cert.yaml` - ssl cert
6. `helm upgrade --install --namespace skillometer --values=clusters/skillometer/proxy/values.yaml traefik traefik/traefik`