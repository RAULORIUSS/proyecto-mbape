# Proyecto: SIEM con ELK para Monitorización de Seguridad

Este proyecto tiene como objetivo la implantación de un SIEM (Security Information and Event Management) utilizando la suite ELK (Elasticsearch, Logstash y Kibana) para centralizar la recolección, almacenamiento y análisis de logs de servidores y dispositivos de red.

---

## Objetivos del Proyecto

- Implantar un entorno ELK en una infraestructura basada en máquinas virtuales o contenedores Docker.
- Configurar Logstash y Filebeat para recopilar logs de sistemas Unix .
- Incorporar reglas de detección de eventos sospechosos, como intentos de acceso fallidos o escaneos de puertos.
- Configurar Dashboards en Kibana para visualizar eventos de seguridad.
- Crear un entorno de pruebas con ataques simulados para verificar el funcionamiento del SIEM (DoS, DDoS, escaneo de puertos, EICAR, etc.).

---

## Estructura del Repositorio

```bash
proyecto-mbape/
├── memoria.md                    # Documentación principal del proyecto
├── compose.yaml          # Configuración de servicios ELK en contenedores
├── maquinas/                   # Archivos y configuraciones de máquinas virtuales o entornos
│   └── (configuraciones específicas de cada máquina)
├── siem-elk/                   # Archivos específicos del stack ELK
│   ├── elasticsearch/          # Configuración de Elasticsearch
│   ├── logstash/               # Configuración de Logstash y sus pipelines
│   ├── kibana/                 # Configuración de Kibana
│   └── filebeat/               # Configuración de Filebeat
├── pruebas/                    # Scripts y logs de pruebas de seguridad simuladas
│   └── ( DDoS, escaneos, EICAR, etc.)
```


### Pruebas

- Añadir scripts de pruebas simuladas de seguridad (ataques DoS, escaneo, etc.).

### Visualización

-  Incluir capturas o enlaces a Dashboards de Kibana funcionales.
-  Añadir interpretación de resultados de pruebas.


## 🗓️ Planificación 

| Fecha       | Actividad                                      |
|-------------|------------------------------------------------|
| 15/04/2024  | Instalación de entornos virtuales y Docker     |
| 20/04/2024  | Configuración de ELK y recolección de logs     |
| //2024  | Desarrollo de reglas de detección y dashboards |
| //2024  | Pruebas de ataques y validación                |
| //2024  | Documentación y entrega final                  |

---

**Autor**: Raúl Méndez García  
**Centro**: IES San Andrés  
**Fecha**: marzo de 2024
