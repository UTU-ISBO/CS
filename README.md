1. Plantilla en Formato Markdown para subir al repositorio del estudiante
Guárdalo como README.md en el repositorio de cada estudiante:

markdown
Copy
Edit
# Evaluación Práctica - Diseño de Red Completa

**Alumno:**  
**Curso:**  
**Fecha:**  

---

## 📌 Objetivo

Diseñar un esquema completo de red que integre conectividad WAN, LAN cableada, WLAN con WiFi 6 y una DMZ con servicios esenciales (Web, SMTP y Base de Datos).

---

## 📐 Diagrama de Red

Adjuntar el archivo del diagrama (en formato `.drawio`, `.png` o `.svg`).

> 📝 *Puedes usar [https://app.diagrams.net](https://app.diagrams.net) (Draw.io) para realizar el diagrama.*

---

## 🌐 Configuración WAN

| Parámetro           | Valor                           |
|---------------------|---------------------------------|
| Medio físico        | Fibra óptica                    |
| IP pública          |                                 |
| Máscara de subred   |                                 |
| Gateway (GW)        |                                 |
| DNS externos        |                                 |
| Router (marca/modelo) |                              |

---

## 🖧 Configuración LAN

| Dispositivo         | IP Privada     | Máscara | GW         | Hostname | MAC Address       | Sistema Operativo     |
|---------------------|----------------|---------|------------|----------|--------------------|------------------------|
| PC Oficina 1        |                |         |            |          |                    |                        |
| PC Oficina 2        |                |         |            |          |                    |                        |
| Servidor DHCP       |                |         |            |          |                    |                        |

- Rango DHCP: `192.168.X.X - X.X`
- Gateway LAN: 
- Equipamiento utilizado (switches, categoría de cable, racks):

---

## 📶 Configuración WLAN (WiFi 6)

| Parámetro           | Valor                         |
|---------------------|-------------------------------|
| SSID                |                               |
| Seguridad           | WPA3                          |
| Frecuencia          | 2.4 GHz / 5 GHz / 6 GHz        |
| DHCP                | Sí / No (indicar)             |
| MAC address ejemplo |                               |
| Equipamiento        | Marca/modelo del AP           |

---

## 🔐 DMZ - Zona Desmilitarizada

| Servicio           | IP Interna     | Puerto | Hostname        | Sistema Operativo | Observaciones                |
|--------------------|----------------|--------|------------------|--------------------|------------------------------|
| Servidor Web       |                | 80/443 |                  |                    |                              |
| Servidor SMTP      |                | 25     |                  |                    | Postfix                      |
| Servidor Base Datos|                | 3306/5432 |              |                    | MariaDB / PostgreSQL         |

- Firewall/ACL: Indicar puertos abiertos hacia/desde la DMZ
- VLANs o interfaces separadas (explicar cómo se aísla la DMZ de la LAN)

---

## 🔎 Seguridad y Escalabilidad

- ¿Qué medidas de seguridad aplicaste?
- ¿Cómo se podría escalar esta red a más usuarios o servicios?

---

## 📎 Archivos Adjuntos

- `diagrama.drawio` o `diagrama.png`
- Capturas de configuración si aplica
- Este archivo `README.md` completo

---

## ✅ Checklist

- [ ] Diagrama completo
- [ ] WAN configurada
- [ ] LAN con DHCP y datos
- [ ] WLAN con parámetros de WiFi 6
- [ ] DMZ con servicios y puertos
- [ ] Documentación clara

🧰 2. Bosquejo del Diagrama de Red en Draw.io
Te dejo una idea textual para que puedas replicarla fácilmente en draw.io:

🖼 Estructura del diagrama:
less
Copy
Edit
[INTERNET]
     |
[Router de borde] ————→ [Switch DMZ]
     |                            |——→ [Servidor Web (80/443)]
     |                            |——→ [Servidor SMTP (25)]
     |                            |——→ [Servidor BD (3306)]
     |
[Switch principal] ————→ [AP WiFi 6] → Clientes inalámbricos
     |
     |——→ [PC 1]
     |——→ [PC 2]
     |——→ [Servidor DHCP]
🔧 Detalles sugeridos a incluir visualmente:
Flechas con etiquetas de puertos abiertos.

Cajas con las IP, máscara, hostname.

Colores para separar LAN, WLAN, DMZ, y WAN.

Notas al margen indicando DNS, rango DHCP, gateway.
