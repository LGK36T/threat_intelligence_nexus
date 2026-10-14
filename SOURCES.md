# Fuentes de Inteligencia de Amenazas (Cyber Threat Intelligence - CTI)

Este documento recopila y describe fuentes de información clave, repositorios de código abierto y marcos analíticos fundamentales utilizados en **Threat Intelligence Nexus** para la recolección, correlación, análisis y atribución de ciberamenazas.

---

## Índice de Fuentes

1. [MITRE ATT&CK - Grupos de Amenazas](#1-mitre-attck---groups)
2. [MITRE ATT&CK - Software y Herramientas](#2-mitre-attck---software)
3. [MITRE ATT&CK - Campañas](#3-mitre-attck---campaigns)
4. [Awesome Ransomware (bbbbbrie)](#4-awesome-ransomware)
5. [Ransomchats (Casualtek)](#5-ransomchats)
6. [ThreatLabz (Zscaler)](#6-threatlabz)
7. [TheRavenFile (Rakesh Krishnan)](#7-theravenfile)
8. [DarkWeb Forums Tracker (brunosergi)](#8-darkweb-forums-tracker)
9. [Onions List (nolim1t)](#9-onions-list)
10. [CVE Program (cve.org)](#10-cve-program-cveorg)
11. [CVEList v5 (CVEProject)](#11-cvelist-v5-cveproject)

---

## 1. MITRE ATT&CK - Groups

- **Enlace**: [https://attack.mitre.org/groups/](https://attack.mitre.org/groups/)
- **Categoría**: Base de conocimiento global / Taxonomía y Marco de CTI
- **Descripción**:  
  Es el catálogo oficial del framework MITRE ATT&CK que documenta y estandariza los grupos de amenazas conocidos a nivel mundial, incluyendo Actores de Amenaza Persistente Avanzada (APT), grupos de ciberdelincuencia organizada, operadores de ransomware y grupos patrocinados por estados.
- **Información disponible**:
  - **Identificadores y Nomenclatura**: Identificador único de MITRE (p. ej., `G0007`) y mapeo exhaustivo de alias utilizados por distintos proveedores de seguridad (p. ej., APT28, Fancy Bear, Sofacy, STRONTIUM).
  - **Tácticas, Técnicas y Procedimientos (TTPs)**: Mapeo granular de todas las técnicas de ataque empleadas por cada grupo a lo largo del ciclo de vida del ataque (Enterprise, Cloud, ICS, Mobile).
  - **Software y Herramientas Asociadas**: Inventario de malware, herramientas de doble uso (*dual-use tools*) y utilidades administrativas utilizadas habitualmente por cada actor.
  - **Campañas y Referencias**: Historial de campañas atribuidas y enlaces a informes técnicos y reportes de investigación de la industria de ciberseguridad.

---

## 2. MITRE ATT&CK - Software

- **Enlace**: [https://attack.mitre.org/software/](https://attack.mitre.org/software/)
- **Categoría**: Catálogo y Taxonomía de Malware y Herramientas Adversarias
- **Descripción**:  
  Es un registro analítico y estructurado de todas las piezas de software (código malicioso, utilidades legítimas del sistema y herramientas de pruebas de penetración o de administración) que han sido observadas en intrusiones reales documentadas por la comunidad de seguridad.
- **Información disponible**:
  - **Clasificación del Software**: Distingue entre:
    - **Malware**: Programas diseñados explícitamente con fines hostiles (troyanos, ransomware, wipers, loaders, botnets).
    - **Tools**: Herramientas comerciales, utilidades open source o software de administración legítimo reutilizado por adversarios con fines maliciosos (p. ej., Cobalt Strike, BloodHound, Mimikatz, PsExec, PowerShell).
  - **Metadatos y Plataformas**: Identificador único (p. ej., `S0002`), aliases, plataformas afectadas (Windows, Linux, macOS, AWS, Azure, etc.).
  - **Mapeo de Técnicas**: Detalle de qué técnicas específicas de ATT&CK implementa cada pieza de software.
  - **Trazabilidad de Uso**: Lista de grupos de amenazas y campañas en las que se ha identificado el software.

---

## 3. MITRE ATT&CK - Campaigns

- **Enlace**: [https://attack.mitre.org/campaigns/](https://attack.mitre.org/campaigns/)
- **Categoría**: Inteligencia Operacional y Análisis de Operaciones Maliciosas
- **Descripción**:  
  Registra y describe campañas cibernéticas concretas. A diferencia de un grupo de amenazas (que existe en el tiempo) o del software en sí, una campaña representa un conjunto delimitado de actividad maliciosa que ocurre durante un período determinado de tiempo, con objetivos específicos, vectores concretos y destinatarios dirigidos.
- **Información disponible**:
  - **Identificador y Cronología**: Código de campaña (p. ej., `C0024` para el compromiso de SolarWinds, `C0022` para Operation Dream Job), fechas de inicio, pico de actividad y cierre o detección.
  - **Atribución y Relaciones**: Grupos de amenazas asociados o hipótesis de atribución basadas en evidencia técnica.
  - **Tácticas y Técnicas Operacionales**: Subconjunto exacto de TTPs implementadas en dicha operación en particular.
  - **Software Desplegado**: Malware específico, scripts a medida y herramientas utilizadas en esa ventana temporal.
  - **Fuentes de Investigación**: Citas directas a los análisis técnicos forenses publicados por firmas de CTI y CERTs gubernamentales.

---

## 4. Awesome Ransomware

- **Enlace**: [https://github.com/bbbbbrie/awesome-ransomware](https://github.com/bbbbbrie/awesome-ransomware)
- **Autor / Mantenedor**: `@bbbbbrie`
- **Categoría**: Directorio Curado de Recursos e Investigación de Ransomware
- **Descripción**:  
  Una lista curada orientada a la investigación y análisis del ecosistema de ransomware, priorizando la comprensión técnica de las operaciones de extorsión digital antes que las guías básicas de remediación.
- **Información disponible**:
  - **Literatura y Publicaciones**: Enlaces a libros de referencia (p. ej., *Ransomware Revealed*, *The Ransomware Hunting Team*), artículos de investigación clave y análisis históricos.
  - **Herramientas de Descifrado (Decrypters)**: Compilación de herramientas de descifrado públicas y gratuitas proporcionadas por empresas como Emsisoft, Kaspersky, Trend Micro y la iniciativa *No More Ransom*.
  - **Recursos de Ransom Notes**: Enlaces a colecciones y archivos de notas de rescate dejadas por diferentes familias de ransomware.
  - **Comunicaciones Filtradas**: Enlaces a archivos y filtraciones de chats internos de grupos de cibercrimen (como las comunicaciones internas filtradas de Conti).
  - **Herramientas de Análisis**: Utilidades de búsqueda forense de notas y extensiones cifradas (CryptoSearch, RansomNoteCleaner, simuladores de RaaS).

---

## 5. Ransomchats

- **Enlace**: [https://github.com/Casualtek/Ransomchats](https://github.com/Casualtek/Ransomchats)
- **Autor / Mantenedor**: `@Casualtek` (Valéry Marchive)
- **Categoría**: Dataset de Negociaciones Reales de Ransomware / Telemetría de Extorsión
- **Descripción**:  
  Es un repositorio de inteligencia que compila registros reales de negociaciones entre operadores de ransomware y víctimas o equipos de respuesta a incidentes, normalizados y estructurados en formato JSON. Su objetivo es aportar visibilidad y datos reproducibles sobre cómo operan realmente las bandas de extorsión digital.
- **Información disponible**:
  - **Registros de Conversación en JSON**: Transcripciones mensaje a mensaje de las salas de negociación de portales Tor/onion de grupos como LockBit, Akira, BlackCat/ALPHV, Conti, Hive, Mount Locker, entre otros.
  - **Datos Financieros y de Demanda**: Monto inicial exigido en criptomonedas (Bitcoin, Monero), descuentos concedidos durante la negociación, plazos otorgados y acuerdos finales.
  - **Anonimización y Cumplimiento Ético**: Datos sensibles de las víctimas redactados y anonimizados hasta que el incidente haya sido divulgado públicamente por los propios atacantes o en medios de comunicación.
  - **Aplicaciones y Herramientas**: Parsers para estandarizar chats y soporte de integración con plataformas de telemetría como [ransomware.live](https://www.ransomware.live/#/negotiations) y visores dedicados ([ransomch.at](https://ransomch.at/)).
  - **Material para Análisis Avanzado**: Utilizado en la industria y academia para análisis estilométrico (determinar si un mismo operador humano responde por diferentes grupos), psicología de la negociación y perfiles operativos.

---

## 6. ThreatLabz (Zscaler)

- **Enlace**: [https://github.com/ThreatLabz](https://github.com/ThreatLabz)
- **Organización**: Zscaler ThreatLabz (Equipo de Investigación y CTI)
- **Categoría**: Inteligencia Técnica de Amenazas, IOCs y Herramientas de Ingeniería Inversa
- **Descripción**:  
  Espacio oficial en GitHub del equipo de investigación de amenazas de Zscaler. Proporciona herramientas de análisis forense, ingeniería inversa de malware y feeds de indicadores de compromiso extraídos directamente de sus investigaciones públicas y telemetría de nube.
- **Información disponible**:
  - **Indicadores de Compromiso (`iocs`)**: Hashes de malware (SHA256/MD5), direcciones IP de Comando y Control (C2), URLs y dominios maliciosos publicados en sus reportes de amenazas globales.
  - **Notas de Rescate (`ransomware_notes`)**: Repositorio dedicado que almacena un archivo histórico y actualizado de textos y formatos de notas de rescate dejadas por operadores de ransomware.
  - **Herramientas de Detección y Remediación**: Proyectos de software especializado para analizar y neutralizar familias de malware específicas (p. ej., `danadetector` para DanaBot, `smokebuster` para SmokeLoader).
  - **Deofuscadores y Plugins para Analistas**: Utilidades para decompilación e ingeniería inversa (como `pikabot-deobfuscator` para desofuscar cadenas protegidas con RC4 y AES en IDA Pro).

---

## 7. TheRavenFile

- **Enlace**: [https://github.com/TheRavenFile](https://github.com/TheRavenFile)
- **Autor / Mantenedor**: Rakesh Krishnan
- **Categoría**: Threat Hunting, Feeds de IOCs, Reglas YARA y Perfilado de Amenazas
- **Descripción**:  
  Repositorio y perfil de investigación de ciberamenazas activo centrado en la caza diaria de amenazas (*daily threat hunting*), investigación de actores maliciosos, ingeniería inversa y publicación de telemetría operativa de libre acceso.
- **Información disponible**:
  - **Caza Diaria e Indicadores (`Daily-Hunt`, `IOC`, `HOSTNAMES`)**: Listados continuos de IPs maliciosas, URLs, nombres de host comprometidos e infraestructura maliciosa descubierta durante investigaciones en tiempo real.
  - **Actores de Amenaza (`THREAT-ACTORS`)**: Mapeo técnico de grupos de ciberdelincuencia y estados-nación con artefactos asociados a sus operaciones.
  - **Reglas YARA (`YARA-RULES`)**: Firmas de detección para identificar variantes emergentes de malware, stealers y ransomware.
  - **Filtraciones de Ransomware (`LEAKS`)**: Archivos y datos procedentes de filtraciones internas de grupos de ransomware.
  - **Scripts y Vectores (`Malicious-Powershell`)**: Colección de scripts maliciosos de PowerShell observados en investigaciones forenses para análisis de evasión y técnicas de ejecución.
  - **Contexto e Historias de Inteligencia (`Intel-Stories`, `CVE-Intel`)**: Documentación narrativa sobre cómo se descubrieron ciertos IOCs y análisis profundos de vulnerabilidades explotadas *in-the-wild*.

---

## 8. DarkWeb Forums Tracker

- **Enlace**: [https://github.com/brunosergi/darkweb-forums-tracker](https://github.com/brunosergi/darkweb-forums-tracker)
- **Autor / Mantenedor**: Bruno Sergi (`@brunosergi`)
- **Categoría**: Automatización de Monitoreo de Foros de la Dark Web con IA / Detección Temprana
- **Descripción**:  
  Herramienta de automatización y scraping inteligente que monitoriza de manera periódica foros clandestinos en la Dark Web, utilizando agentes de Inteligencia Artificial para extraer, filtrar y clasificar actividad relevante (ventas de bases de datos, accesos iniciales, credenciales robadas, exploits) y enviar alertas automáticas a canales de Discord.
- **Información disponible y arquitectura**:
  - **Scraping Automatizado y Sigiloso**: Implementación mediante contenedores Docker utilizando Playwright MCP para simular navegación humana en entornos Tor/Dark Web.
  - **Procesamiento y Clasificación con IA**: Utiliza modelos de lenguaje (Google Gemini) para interpretar el contenido de las publicaciones clandestinas, evaluar su criticidad y descartar ruido o publicaciones de bajo valor.
  - **Orquestación de Flujos (n8n)**: Pipelines de trabajo automatizados que coordinan la recolección, el procesamiento y la notificación cada pocas horas.
  - **Persistencia y Alertas**: Almacenamiento estructurado en Supabase y generación de alertas inmediatas en Discord con capturas de pantalla de las publicaciones detectadas.
  - **Mecanismo Human-in-the-Loop**: Soporte para conexión mediante interfaz VNC para permitir que un operador humano resuelva CAPTCHAs complejos o desafíos de inicio de sesión cuando sea necesario.

---

## 9. Onions List

- **Enlace**: [https://github.com/nolim1t/onions-list](https://github.com/nolim1t/onions-list)
- **Autor / Mantenedor**: `@nolim1t`
- **Categoría**: Directorio y Catálogo Curado de Servicios Ocultos Tor (`.onion`)
- **Descripción**:  
  Directorio curado ("Hyper-onion-ization") de direcciones `.onion` activas en la red Tor, diseñado como índice de referencia para la navegación anónima, auditoría de infraestructura y verificación de servicios tanto legítimos como subterráneos.
- **Información disponible**:
  - **Servicios Ocultos de Entidades Legítimas**: Listado verificado de direcciones `.onion` (v3) de medios de comunicación y portales de noticias internacionales (BBC, The New York Times, ProPublica, The Intercept).
  - **Plataformas de Privacidad y Comunicación Segura**: Enlaces a servicios de correo cifrado y mensajería (ProtonMail, Keybase, DuckDuckGo en Tor).
  - **Ecosistema Cripto y Repositorios Espejo**: Espejos en Tor de repositorios Git de Bitcoin, software de billeteras seguras (Wasabi Wallet, Electrum) y exploradores de bloques.
  - **Guía de Configuración de Proxy Tor**: Parámetros de conexión y entorno para interactuar con la red Tor localmente (`127.0.0.1:9050` / `9151`) mediante proxies SOCKS5 para herramientas de inteligencia y scraping.

---

## 10. CVE Program (cve.org)

- **Enlace**: [https://www.cve.org/](https://www.cve.org/)
- **Organización / Mantenedor**: The CVE Program / MITRE / CISA
- **Categoría**: Estándar Internacional de Vulnerabilidades y Exposiciones Comunes (Vulnerability Intelligence)
- **Descripción**:  
  Es el portal oficial del programa CVE (Common Vulnerabilities and Exposures), el estándar de referencia global de la industria para identificar, catalogar y divulgar públicamente vulnerabilidades de seguridad de software y firmware.
- **Información disponible**:
  - **Buscador y Registros Oficiales de CVE**: Acceso directo al catálogo de identificadores CVE (p. ej., `CVE-2024-XXXXX`), estado del registro (*Published*, *Reserved*, *Rejected*), descripción técnica y referencias externas (avisos de seguridad, parches oficiales y reportes de explotación).
  - **Estructura y Gobernanza del Programa**: Información sobre Autoridades de Numeración de CVE (CNAs - *CVE Numbering Authorities*), raíces (Roots) y publicadores de datos autorizados (ADPs - *Authorized Data Publishers*).
  - **Documentación de Esquemas y APIs**: Documentación del esquema JSON 5.0 para registros CVE y especificaciones de la API REST oficial para automatizar la consulta y gestión de vulnerabilidades.
  - **Políticas y Pautas de Divulgación Coordinada**: Reglas formales para la asignación y divulgación coordinada de vulnerabilidades en la industria.

---

## 11. CVEList v5 (CVEProject)

- **Enlace**: [http://github.com/CVEProject/cvelistv5](http://github.com/CVEProject/cvelistv5)
- **Organización / Mantenedor**: CVE Project (`@CVEProject`)
- **Categoría**: Repositorio Masivo de Vulnerabilidades en Formato JSON 5.0 (Machine-Readable CTI Feed)
- **Descripción**:  
  Es el repositorio oficial de GitHub que contiene la lista completa y actualizada de todos los registros CVE en el formato estándar CVE JSON 5.0. Funciona como el canal de sincronización y distribución masiva en tiempo real del CVE Program mediante Git, reemplazando al antiguo repositorio heredado `cvelist`.
- **Información disponible**:
  - **Registros Estructurados en JSON v5**: Cada vulnerabilidad publicada dispone de su archivo individual (`cves/YYYY/XXXXxxx/CVE-YYYY-XXXX.json`), estructurado bajo el esquema oficial CVE JSON 5.0.
  - **Metadatos Técnicos Detallados**:
    - Tipos de problemas y debilidades asociados clasificados con CWE (*Common Weakness Enumeration*).
    - Fabricante (*vendor*), producto y rangos precisos de versiones afectadas y solucionadas.
    - Contenedor CNA con información técnica asignada por el fabricante o investigador original.
    - Contenedores ADP (*Authorized Data Publisher*), como el de CISA, que incorporan evaluaciones de riesgo complementarias (p. ej., banderas de explotación activa en el KEV - *Known Exploited Vulnerabilities*, métricas SSVC y puntuaciones CVSS v3.1 / v4.0).
  - **Historial de Cambios y Diff Trazable**: Al ser un repositorio Git, permite auditar commits, versiones anteriores y diffs para detectar cuándo una vulnerabilidad fue modificada, actualizada con nuevos vectores de ataque o marcada como rechazada.
  - **Sincronización Automatizada (Mirroring)**: Permite que motores de escaneo, herramientas de gestión de parches y plataformas de Threat Intelligence clonen o hagan pull incremental para mantener bases de datos locales siempre al día sin bloqueos por cuotas de API.

---

## Resumen de Aplicabilidad en Threat Intelligence Nexus

| Fuente | Tipo de Información Principal | Fase del Ciclo de Inteligencia | Uso Típico en el Proyecto |
| :--- | :--- | :--- | :--- |
| **MITRE ATT&CK Groups** | Perfiles de actores, alias, TTPs | Procesamiento / Análisis | Atribución y mapeo de adversarios |
| **MITRE ATT&CK Software** | Catálogo de malware y herramientas dual-use | Procesamiento / Análisis | Detección técnica y correlación de utilidades |
| **MITRE ATT&CK Campaigns** | Operaciones acotadas en tiempo y objetivos | Análisis / Producción | Contextualización de incidentes y tendencias |
| **Awesome Ransomware** | Recursos, libros, decrypters, ransom notes | Recolección / Investigación | Base de conocimiento para investigación de ransomware |
| **Ransomchats** | Transcripciones JSON de negociaciones reales | Recolección / Análisis | Modelado de extorsión, stylometry y montos de rescate |
| **ThreatLabz** | IOCs, notas de rescate, deofuscadores | Recolección / Procesamiento | Enriquecimiento de feeds técnicos y análisis de malware |
| **TheRavenFile** | Feeds de IOCs diarios, YARA, leaks | Recolección / Procesamiento | Caza activa de amenazas (*threat hunting*) y reglas de detección |
| **DarkWeb Forums Tracker** | Scraping automatizado de foros con IA | Recolección / Difusión | Monitoreo temprano de filtraciones y ventas de credenciales |
| **Onions List** | Directorio de sitios `.onion` Tor | Recolección / Soporte | Infraestructura para escaneo y navegación en la Dark Web |
| **CVE Program (cve.org)** | Base de datos oficial de vulnerabilidades CVE | Procesamiento / Enriquecimiento | Normalización y referencia universal de fallos de seguridad |
| **CVEList v5** | Registros completos de CVEs en JSON 5.0 | Recolección / Procesamiento | Ingesta masiva, automatización y alertas tempranas de CVEs |

