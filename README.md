# Como nació Proyecto Yungas(Origen y propósito)
Proyecto Yungas es una Progressive Web App (PWA) de carácter experimental, concebida como prototipo de investigación para el trabajo de tesis de la Licenciatura en Gestión Universitaria. Su objetivo es analizar el impacto del software libre en la vinculación territorial y la seguridad preventiva de senderistas en las Yungas tucumanas mediante mapas offline y herramientas comunitarias. El sistema se distribuye estrictamente como una prueba de concepto abierta y gratuita.
# Escala y Desarrollo Técnico (Horco Molle)
La Reserva Experimental Horco Molle funciona como el campo de pruebas inicial con usuarios reales en entorno de testing. Su arquitectura es escalable para replicarse en otros circuitos de la región (Funiculares, Cuesta del Cielo) y, a futuro, colaborar en zonas de alta complejidad donde la geolocalización es crítica (Ñuñorco, Los Alisos).

Para superar las limitaciones de conectividad en zonas de montaña, el proyecto investiga la triangulación de posiciones entre usuarios y la integración experimental de hardware de radiofrecuencia (nodos ESP32/LoRa y LoRa APRS) para la transmisión de coordenadas sin dependencia de redes 4G/LTE. Asimismo, la infraestructura de datos se proyecta hacia la gestión ambiental y la permacomputing, permitiendo monitorear variables ecológicas para la toma de decisiones preventivas, tales como la rotación de senderos en descanso o la alerta temprana en zonas de riesgo.

## ⚠️ Aviso Legal y de Seguridad Importante
**Este software es una prueba de concepto experimental de código abierto.**
* **No** es un servicio oficial de emergencias, ni reemplaza al 911, a Defensa Civil, a los guardaparques ni a los cuerpos de rescate oficiales.
* Los autores y colaboradores no asumen responsabilidad civil ni penal por el uso de la herramienta, fallas técnicas, interrupciones de conectividad GPS/red en el cerro, demoras en la respuesta ante incidentes o el uso indebido de la plataforma. 
* Ante una urgencia real, comuníquese siempre con los organismos de emergencia competentes o utilice los números de contacto oficiales provistos en la app.

## 🚀 Características Técnicas
* **Funcionamiento Híbrido / Offline-First:** Diseñada para entornos de baja cobertura. Utiliza mapas interactivos mediante Leaflet y almacenamiento local (`localStorage`) para registrar incidencias y mantener la operatividad básica sin señal.
* **Geolocalización en Vivo:** Seguimiento de posición del usuario, cálculo de distancias aproximadas a puntos de salida clave (Jardín Botánico, Reserva, Finca de limones, etc.) y cálculo automático de hora de ocaso según la época del año.
* **Botón de Pánico (SOS) con Cuenta Regresiva:** Sistema de alerta de emergencia con margen de cancelación voluntaria para evitar activaciones accidentales.
* **Reportes Comunitarios y Analítica en Lote (Batch Sync):** Sistema de reportes de senderos sincronizados de forma optimizada mediante beacons/lotes para minimizar el consumo de datos y batería en el monte.
* **Soporte de Recorridos (GeoJSON):** Visualización modular de traza de senderos y rutas propuestas.

## 🛠️ Stack Tecnológico
* **Frontend:** HTML5, CSS3, JavaScript (Vanilla).
* **Mapas:** Leaflet.js (OpenStreetMap).
* **Procesamiento de Datos:** SheetJS (XLSX) para gestión analítica y Google Apps Script como backend ligero.
* **PWA:** Service Workers para soporte offline.

## 📄 Licencia
Este proyecto se distribuye bajo los términos de la **MIT License**. Eres libre de usar, clonar, auditar y modificar este software, bajo la condición de que se provee "tal cual es", sin garantía de ningún tipo. Consulta el archivo `LICENSE` para más detalles.
