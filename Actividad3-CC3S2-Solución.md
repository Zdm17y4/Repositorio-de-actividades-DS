

---
## A. Cuestionario

### 1. Motivaciones para la nube  
**1.a. ¿Qué problemas o limitaciones existían antes del surgimiento de la computación en la nube y cómo los solucionó la centralización de servidores en data centers?**

Antes de la nube, las empresas dependían de hardware propio y centros de datos aislados, lo que generaba altos costos, baja escalabilidad y dificultad para responder a picos de demanda. La centralización en data centers permitió consolidar recursos, optimizar el uso de la infraestructura y ofrecer un modelo de pago por uso que reduce gastos operativos.

**1.b. ¿Por qué se habla de “The Power Wall” y cómo influyó la aparición de procesadores multi-core en la evolución hacia la nube?**  
El “Power Wall” se refiere al límite físico en el aumento de la frecuencia de los procesadores debido a problemas de disipación térmica y consumo energético. La aparición de procesadores multi-core permitió paralelizar tareas, lo que facilitó la distribución de cargas de trabajo en entornos virtualizados y escalables, impulsando así la evolución hacia la nube.

### 2. Clusters y load balancing  
**2.a. Explica cómo la necesidad de atender grandes volúmenes de tráfico en sitios web condujo a la adopción de clústeres y balanceadores de carga.**  
El incremento del tráfico web llevó a distribuir las solicitudes entre varios servidores para evitar sobrecargas. Se implementaron clústeres y balanceadores de carga que reparten las peticiones, garantizando alta disponibilidad y respuestas rápidas a los usuarios.

**2.b. Describe un ejemplo práctico de cómo un desarrollador de software puede beneficiarse del uso de load balancers para una aplicación web.**  
Un desarrollador de un e-commerce puede utilizar un load balancer para distribuir las solicitudes de los clientes entre múltiples servidores, mejorando la experiencia del usuario durante picos de tráfico, evitando cuellos de botella y asegurando la continuidad del servicio en caso de fallos de alguno de los servidores.

### 3. Elastic computing  
**3.a. Define con tus propias palabras el concepto de Elastic Computing.**  
Elastic Computing es la capacidad de ajustar dinámicamente la cantidad de recursos de cómputo según la demanda, permitiendo escalar hacia arriba o hacia abajo sin interrupciones.

**3.b. ¿Por qué la virtualización es una pieza clave para la elasticidad en la nube?**  
La virtualización abstrae el hardware físico, permitiendo crear y gestionar múltiples máquinas virtuales de forma rápida y eficiente. Esto facilita la asignación de recursos según las necesidades y permite ajustar la capacidad sin depender del hardware físico.

**3.c. Menciona un escenario donde, desde la perspectiva de desarrollo, sería muy difícil escalar la infraestructura sin un entorno elástico.**  
En una aplicación de streaming en vivo con picos imprevistos de audiencia, sin un entorno elástico habría que adquirir y configurar hardware adicional de forma manual, lo que retrasaría la respuesta a la demanda y aumentaría los costos.

### 4. Modelos de servicio (IaaS, PaaS, SaaS, DaaS)  
**4.a. Diferencia cada uno de estos modelos. ¿En qué casos un desarrollador optaría por PaaS en lugar de IaaS?**  
- **IaaS (Infraestructura como Servicio):** Ofrece recursos virtualizados (servidores, almacenamiento) y requiere gestionar el sistema operativo y las aplicaciones.  
- **PaaS (Plataforma como Servicio):** Proporciona un entorno gestionado para desarrollar y desplegar aplicaciones sin preocuparse por la infraestructura subyacente.  
- **SaaS (Software como Servicio):** Entrega aplicaciones listas para usar, sin necesidad de gestionar infraestructura o desarrollo.  
- **DaaS (Desktop as a Service):** Ofrece escritorios virtuales accesibles desde cualquier dispositivo.

Se opta por PaaS cuando el objetivo es centrarse en el desarrollo del código y la lógica de negocio sin tener que administrar el sistema operativo o la infraestructura.

**4.b. Enumera tres ejemplos concretos de proveedores o herramientas que correspondan a cada tipo de servicio.**  
- **IaaS:** AWS EC2, Azure Virtual Machines, Google Compute Engine.  
- **PaaS:** AWS Elastic Beanstalk, Azure App Service, Google App Engine.  
- **SaaS:** Microsoft Office 365, Google Workspace, Salesforce.  
- **DaaS:** Amazon WorkSpaces, Citrix Virtual Apps and Desktops, VMware Horizon Cloud.

### 5. Tipos de nubes (Pública, Privada, Híbrida, Multi-Cloud)  
**5.a. ¿Cuáles son las ventajas de implementar una nube privada para una organización grande?**  
Una nube privada ofrece mayor control, seguridad y personalización, permitiendo cumplir requisitos regulatorios y gestionar datos sensibles de manera interna.

**5.b. ¿Por qué una empresa podría verse afectada por el “provider lock-in”?**  
El “provider lock-in” ocurre cuando una empresa se vuelve dependiente de un único proveedor por el uso de servicios y APIs propietarias, lo que dificulta y encarece la migración a otros proveedores en el futuro.

**5.c. ¿Qué rol juegan los “hyperscalers” en el ecosistema de la nube?**  
Los hyperscalers (como AWS, Azure y Google Cloud) son proveedores de infraestructura masiva que ofrecen escalabilidad global y servicios avanzados, impulsando la innovación y la capacidad de gestionar grandes volúmenes de datos y recursos.

---

## B. Actividades de investigación y aplicación

### 1. Estudio de casos  
**Caso 1:**  
- **Motivación:** Una startup de tecnología migró a la nube para reducir costos iniciales y acelerar el lanzamiento de su producto.  
- **Beneficios:** Alcanzó escalabilidad rápida, mayor flexibilidad y reducción de gastos operativos mediante un modelo de pago por uso.  
- **Desafíos:** Se enfrentó a retos de seguridad y a la integración de sistemas legados con la nueva infraestructura.

**Caso 2:**  
- **Motivación:** Una gran empresa del sector financiero trasladó parte de su infraestructura a la nube para mejorar la resiliencia y el acceso a datos en tiempo real.  
- **Beneficios:** Obtuvo alta disponibilidad, agilidad en el despliegue de actualizaciones y mejor capacidad de análisis de datos.  
- **Desafíos:** Tuvo que cumplir estrictas normativas de seguridad y gestionar la complejidad de integrar sistemas críticos con la nube.

### 2. Comparativa de modelos de servicio  
**Cuadro Comparativo de Responsabilidades:**

| Modelo | Desarrollador                      | Proveedor                        | Equipo de Operaciones                     |
|--------|------------------------------------|----------------------------------|-------------------------------------------|
| IaaS   | Configuración y despliegue de apps | Gestión de hardware y red        | Administración de sistemas y parches       |
| PaaS   | Desarrollo y código de la app      | Gestión de la plataforma y middleware | Supervisión del entorno y escalabilidad      |
| SaaS   | Uso y configuración mínima         | Mantenimiento y actualizaciones completas | Gestión de usuarios y configuración básica   |

### 3. Estrategia multi-cloud o híbrida  
**Estrategia teórica para migrar el 50% de cargas a un segundo proveedor:**  
- **Base de datos:** Ubicarla en un servicio gestionado que ofrezca replicación entre nubes, asegurando alta disponibilidad.  
- **Configuración de red:** Implementar VPNs o conexiones dedicadas para integrar ambos entornos, utilizando balanceadores de carga para distribuir el tráfico entre el data center propio y la nube pública.  
- **Plan de contingencia:** Redirigir automáticamente el tráfico al entorno alternativo en caso de fallo, mediante monitoreo activo y pruebas de failover.

### 4. Debate sobre costos  
**Análisis breve de pros y contras de cada tipo de nube:**

- **Nube Pública:**  
  - *Pros:* Bajo CAPEX, alta escalabilidad y flexibilidad, rápido despliegue.  
  - *Contras:* Riesgo de provider lock-in y posibles desafíos en cumplimiento normativo.

- **Nube Privada:**  
  - *Pros:* Mayor control, seguridad personalizada y cumplimiento específico.  
  - *Contras:* Altos costos iniciales (CAPEX) y menor flexibilidad para escalar rápidamente.

- **Nube Híbrida:**  
  - *Pros:* Combina control y escalabilidad, permitiendo balancear cargas y gestionar datos sensibles de forma segura.  
  - *Contras:* Mayor complejidad en la integración y gestión de dos entornos.

- **Multi-Cloud:**  
  - *Pros:* Evita dependencia de un único proveedor, mayor resiliencia y optimización de costos mediante la elección de servicios.  
  - *Contras:* Requiere mayor coordinación y puede incrementar la complejidad de gestión y el cumplimiento normativo.

---

## C. Ejercicio de presentación de "Mini-proyecto"

### 1. Objetivo del sistema  
Desarrollar una plataforma de e-commerce que permita a los usuarios comprar productos en línea, integrando pasarelas de pago y gestión de inventario.

### 2. Selección de modelo de servicio  
Se utilizará **PaaS** para el despliegue de la aplicación, permitiendo centrarse en el desarrollo y la lógica de negocio sin preocuparse por la administración de la infraestructura.

### 3. Tipo de nube  
La solución se desplegará en un entorno **híbrido**: se utilizará una nube pública para el front-end y servicios escalables, mientras que la información sensible y las bases de datos se alojarán en una nube privada para mayor control y seguridad.

### 4. Esquema de escalabilidad  
La aplicación se escalará mediante balanceadores de carga que distribuyen el tráfico entre múltiples instancias en la nube pública, con autoescalado basado en la demanda para gestionar picos de visitas.

### 5. Costos y riesgos  
- **Costos:** Gastos operativos (OPEX) por el uso de servicios en la nube, inversión en seguridad y mantenimiento de la nube privada.  
- **Riesgos:** Dependencia del proveedor (lock-in), desafíos en la gestión de la seguridad en entornos duales y complejidad en la integración.

### 6. Presentación final  
**Diagrama de infraestructura (descripción):**  
- **Capa de presentación:** Servidores web en la nube pública detrás de un balanceador de carga.  
- **Capa de aplicación:** Microservicios desplegados en contenedores orquestados con Kubernetes.  
- **Capa de datos:** Base de datos gestionada en la nube privada, conectada de forma segura (VPN) con la nube pública.  
- **Monitoreo y seguridad:** Implementación de herramientas de observabilidad (Prometheus, Grafana) y gestión de identidades (IAM).

---

Cada sección ha sido resuelta de forma ordenada y concisa, siguiendo tanto la lectura como conceptos actualizados en el ámbito de la computación en la nube.
