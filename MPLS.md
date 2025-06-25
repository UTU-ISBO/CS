# 📡 Clase: MPLS en Uruguay y su Aplicación en la Red Nacional de UTU

**Duración:** 1 hora  
**Modalidad:** Teórico-práctica  
**Enfoque:** Ruteo dinámico, garantías de ancho de banda y seguridad

---

## 🎯 Objetivos

- Comprender qué es MPLS y cómo funciona.
- Analizar cómo se implementa MPLS en Uruguay, particularmente en la red de UTU.
- Estudiar el concepto de rutas dinámicas.
- Identificar las ventajas del ancho de banda simétrico garantizado (100 Mbps).
- Reconocer los beneficios de seguridad que ofrece MPLS.

---

## 🧠 Introducción al MPLS (15 min)

### ¿Qué es MPLS?
- **Multiprotocol Label Switching**
- Tecnología que **agrega etiquetas (labels)** a los paquetes IP para que sean reenviados más rápido y de forma eficiente.
- Combina velocidad de **conmutación** y **flexibilidad de ruteo**.

### Características clave:
- Independiente del protocolo de capa 3 (IP, IPv6, etc.)
- Más eficiente que el ruteo tradicional.
- Soporta calidad de servicio (QoS).

---

## 🌐 Caso real: Red Nacional de UTU (15 min)

### Infraestructura MPLS en Uruguay
- **Proveedores principales**: ANTEL (principal backbone MPLS), con presencia en centros educativos.
- La UTU se conecta a través de **enlaces MPLS proporcionados por ANTEL**, en su mayoría con **ancho de banda simétrico garantizado de 100 Mbps**.

### Ventajas para UTU:
- Conectividad de alta disponibilidad entre campus.
- Enlaces simétricos: misma velocidad de subida y bajada, ideal para:
  - Videoconferencias.
  - Transferencias de datos entre servidores.
  - Acceso a servicios en la nube.
- Conexiones directas entre sedes (backbone privado).

> ⚠️ **Nota:** No es Internet, es una **red privada** entre sitios de UTU.

---

## 🔁 Ruteo Dinámico con MPLS (15 min)

### ¿Cómo funciona?
- MPLS utiliza protocolos como **OSPF**, **IS-IS** o **BGP** para aprender rutas.
- Pero en vez de reenviar por IP, **usa etiquetas (labels)** para encaminar el tráfico.

### Ventajas del ruteo dinámico:
- Si un enlace falla, se puede **cambiar automáticamente de ruta** sin perder conectividad.
- Mejora la confiabilidad del servicio educativo digital (clases virtuales, Moodle, etc.).

### Ejemplo:
> Campus A pierde conectividad directa. MPLS enruta automáticamente a través del nodo B sin que el usuario lo note.

---

## 🔐 Seguridad en la Red MPLS (10 min)

### Beneficios:
- MPLS es una red **cerrada**, **no expuesta a Internet directamente**.
- Aislada del tráfico público → menos riesgo de ataques externos.
- Permite políticas por tipo de tráfico y QoS.
- Puede segmentarse con **VRF (VPNs internas)** para separar tráfico de alumnos, administrativos, etc.

---

## 🛠️ Actividad práctica sugerida (fuera de clase)

1. Investigar si el centro educativo del estudiante está conectado por MPLS.
2. Identificar si cuentan con ancho de banda garantizado.
3. ¿Qué aplicaciones usan que se benefician de ancho simétrico?

---

## ✅ Cierre y reflexión (5 min)

- ¿Por qué MPLS es importante para una red educativa?
- ¿Qué diferencia hay entre MPLS y una conexión tradicional por Internet?
- ¿Cómo se garantiza la calidad del servicio?

---

## 📚 Recursos complementarios

- [ANTEL - Servicios empresariales MPLS](https://www.antel.com.uy/)
- [Cisco - Introducción a MPLS](https://www.cisco.com/c/en/us/products/collateral/ios-nx-os-software/multiprotocol-label-switching-mpls/prod_white_paper0900aecd804f1f28.html)
- [RFC 3031 - MPLS Architecture](https://datatracker.ietf.org/doc/html/rfc3031)

---

