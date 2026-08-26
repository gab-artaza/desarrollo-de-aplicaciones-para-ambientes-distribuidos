> Repositorio oficial de la asignatura **Desarrollo de Aplicaciones para Ambientes Distribuidos**, impartida por el **Lic. Gabriel Artaza**.

Este espacio contiene el material práctico, demostraciones de código (*live coding*), guías de laboratorio y proyectos desarrollados durante el cursado.

---

## 📌 Información de la Cátedra

* **Docente:** Lic. Gabriel Artaza
* **Materia:** Desarrollo de Aplicaciones para Ambientes Distribuidos
* **Modalidad:** Teórico-Práctica (60% de instancia práctica)

---

## 🎯 Objetivos de la Asignatura

El objetivo principal es capacitar al estudiante en el diseño, implementación y evaluación de aplicaciones en entornos distribuidos, abordando los desafíos de concurrencia, tolerancia a fallos, comunicación en red y seguridad mediante tecnologías modernas en **Java** y **Node.js/Python**.

---

## 🛠️ Tecnologías y Herramientas Utilizadas

* **Lenguajes:** Java (JDK 17+) / Python / JavaScript (Node.js)
* **Comunicación y Redes:** Sockets (TCP/UDP), REST APIs, gRPC, Java RMI
* **Resiliencia:** Retry Pattern, Exponential Backoff, Timeouts
* **Persistencia Distribuidas:** PostgreSQL, MongoDB (Replicación y Sharding)
* **Seguridad & Monitoreo:** JWT, TLS/SSL, JMeter / Locust
* **Control de Versiones:** Git & GitHub

---

## 📅 Estructura del Cursado y Contenidos

| Unidad | Tema Principal | Práctica / Entregable |
| :---: | :--- | :--- |
| **U1** | Introducción a Sistemas Distribuidos y Evolución Arquitectónica | TP1: Cliente-Servidor simple |
| **U1** | Modelos Fundamentales (Comunicación, Fallo y Seguridad) | TP2: Resiliencia (Retry Pattern y Timeouts) |
| **U2** | Programación con Sockets TCP y UDP | TP3: Servicio de mensajería/archivos con Sockets |
| **U2** | Representación de Datos y Paso de Mensajes | TP4: Parser de JSON / Protocol Buffers |
| **U2** | Modelo de Actores y Sincronización | TP5: Concurrencia sin estado compartido |
| **U3** | Middleware y Objetos Remotos (RMI / gRPC) | TP6: Invocación remota distribuida |
| **U3** | APIs y Servicios Web (REST / Microservicios) | **Hito 1:** Avance del Proyecto Integrador |
| **U4** | Bases de Datos Distribuidas | TP7: Persistencia distribuida y ORM |
| **U4** | Seguridad en Aplicaciones Distribuidas | TP8: Autenticación con JWT y TLS |
| **U4** | Monitoreo y Evaluación de Desempeño | TP9: Pruebas de carga y cuellos de botella |
| **Taller** | Integración y Puesta a Punto | Trabajo en Laboratorio |
| **Final** | Presentación y Defensa Oral del Sistema Distribuido | Demo en Vivo y Evaluación de Arquitectura |

---

## 🚨 Las 8 Falacias de la Computación Distribuida

Durante la cursada se analizan los errores comunes al asumir que la red se comporta como un entorno local:

1. **La red es confiable:** Los mensajes pueden perderse o demorarse.
2. **La latencia es cero:** Toda llamada a través de la red toma tiempo.
3. **El ancho de banda es infinito:** La capacidad de transferencia tiene límites físicos.
4. **La red es segura:** Los datos en tránsito requieren encriptación y autenticación.
5. **La topología no cambia:** Los nodos entran, salen y cambian de dirección IP.
6. **Hay un único administrador:** Múltiples entidades gestionan las partes de la infraestructura.
7. **El costo de transporte es cero:** Enviar y serializar datos insume cómputo y dinero.
8. **La red es homogénea:** Coexisten distintos sistemas operativos, hardware y protocolos.

---
