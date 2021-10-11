# POC ArgoCD
Example aplication for Argo CD

# GitOps 

La clave de GitOps es la idea de la infraestructura como código, que adopta el mismo enfoque de aprovisionamiento de la infraestructura que utiliza devops para aprovisionar las aplicaciones. 
Así, no solo la aplicación, sino también las máquinas y redes anfitrionas subyacentes, son descritas en archivos que pueden ser tratados como cualquier otro código dentro de un sistema de control de versiones, con procesos automatizados que trabajan para hacer converger la aplicación del mundo real con la descrita en esos archivos.


**WeaveWorks**: GitOps fue desarrollado por WeaveWorks, con el objetivo de crear una “fuente única” relacionada con la infraestructura y las aplicaciones.
Para ello se colocó a Git en el centro de su canal de entrega para que los desarrolladores puedan hacer uso de las solicitudes de extracción y así simplificar las operaciones y la implementación de software en Kubernetes.

## Pilares de GitOps

 - Infraestructura como código **(IaaC)**
 - Control de versiones **(Git)**
 - Colaboración **(Merge/Pull Request)**
 - Automatización **(CI/CD)**

## Beneficios y porque GitOps ?

* Unica fuente de la verdad (Estado deseado de la infraestructura en Git)
* Versionamiento de la infraestructura
* Rollback (Git revert)
* Colaboración entre equipos
* Mejora la seguridad - Solo el proceso de CD deberia tener permisos de modificación sobre los recursos del cluster
* Autodocumentación de Git

## Requisitos para implementar GitOps

* Herramienta de control de codigo fuente (Gitlab, Github, etc)
* Herramienta u operador de GitOps definido
* Flujo de proceso definido con actores


## Argo CD


* Diseñado para Kubernetes
* Solo se debe realizar push al repo y Argo  realiza el resto de la tarea
* Argo CD trabaja con la mayoria de herramientas de DevOps (Github, Gitlab, S3 Buckets, CI providers, All major container registries )
* Argo CD funciona con cualquier cluster de K8S y todas las herramientas de K8S (Kustomize, Helm, RBAC, and policy-driven validation)

## Flujo de Proceso (Modelo)

![Argo CD Design](./images/design-argocd.png)

## Referencias:
GitOps Definition: 
Flux CD Documentation