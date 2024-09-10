![Badge IBM](assets/cke_badge.png)
## Archivo creado por Ignacio Suárez

#### Curso: [Introduction to Containers, Kubernetes, and OpenShift V3](https://cognitiveclass.ai/courses/kubernetes-course)
#### Badge IBM: [Containers & Kubernetes Essentials](https://yourlearning.ibm.com/credential/CREDLY-5eef1a66-1a37-42cc-940a-e7160661810a)

##### Comienzo: 10/09/24
##### Finalizado: ---

![Docker](assets/Docker-Logo.png)

**Docker** es un proyecto de código abierto que automatiza el despliegue de aplicaciones dentro de contenedores de software, proporcionando una capa adicional de abstracción y automatización de virtualización de aplicaciones en múltiples sistemas operativos. 
Se encarga de crear y manejar los contenedores a niveles individuales.

> Ciertos conceptos!

##### *Imágenes / Image*
Son plantillas que solo se pueden leer, contienen las instrucciones para la creación de un contenedor. Estás plantillas son las que contienen las librerías y dependencias requeridas por una aplicación para poder correr. Son básicamente una snapshot de un contenedor.

##### *Contenedores / Container*
Un contenedor es un entorno de ejecución que contiene todos los componentes necesarios para que una aplicación pueda correr, sin necesidad de utilizar dependencias de la máquina host.
Básicamente empaqueta una aplicación para que se ejecute en cualquier sistema destino.
Los contenedores son altamente portables y muy ligeros, debido a que no requieren empaquetar todo un sistema operativo dentro, como en el caso de las VM.

##### *Contenedorización / Containerization*
La contenedorización permite que una aplicación de software se ejecute como microservicio en arquitecturas de hardware distribuidas y multiplataformas.

###### Sources:
- [Image, container and containerization](https://aws.amazon.com/es/compare/the-difference-between-docker-images-and-containers/?nc1=h_ls)






![Kubernetes](assets/kubernetes.png)

**Kubernetes** es un orquestador de contenedores, se encarga de automatizar la implementación, escalado y administración de contenedores.

**Arquitectura de Kubernetes.**
![Kubernetes Arch](assets/Kubernetes_architecture.webp)

> Ciertos conceptos!

##### *Clústers*
Un clústers es lo que se puede ver en la arquitectura de arriba. Consiste en un plano de control, y uno, o varios, nodos de trabajo.
También posee una interfaz de usuario (que comparada con la de OpenShift, es más primitiva (dato no checkeado)) y una CLI llamada Kubectl (se pronuncia kube control)

##### *Plano de control*
Controla el estado en general del clúster. Tiene varios componentes:
- **Kube-apiserver**: El componente núcleo, este expone la API de Kubernetes. Se trata del frontend de Kubernetes, recibe las peticiones y actualiza acordemente el estado en etcd.
- **Kube-scheduler**: Se encarga de ejecutar los controladores de Kubernetes (los controladores son bucles de control que observan el estado del clúster, y ejecutan o solicitan los cambios que sean necesarios para alcanzar el estado deseado). Existen varios tipos de controladores, más info en el link de info.
- **To-Do**





![alt text](assets/OpenShift.webp)

**Red Hat OpenShift** es una extensión de Kubernetes, permite funciones adicionales (tales como una GUI) que permiten el build, deploy and run secure cloud-native applications en cualquier lado.Tiene a Kubernetes como parte interior.
Es un producto open-source que se encuentra comercializado por la empresa creadora: Red Hat.