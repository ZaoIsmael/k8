# K8
Proyecto para crear un cluster de kubernetes en local con minikube.

Requisitos:
 * Linux
 * Docker

# Instalación
Ejecutamos install-minikube.sh, para instalar minikube y kubectl.
```bash
./scripts/install-minikube.sh
```

Una vez finalizado podremos arrancar el cluster.
```bash
sudo minikube start --disk-size "10g" --vm-driver "none"
```

Podemos comprobar que todo a ido bien con:
```bash
sudo kubectl get services -n kube-system
```
si el cluster esta operativo podemos abrir el dashboard
```bash
sudo minikube dashboard 
```
[![dashboard](https://i.imgur.com/pD1F0yH.png)](https://i.imgur.com/pD1F0yH.png)