# Como nació Proyecto Yungas
Proyecto Yungas, es un PWA tipo proyecto/prototipo experimental nacido como idea para un proyecto de tesis para el final de cursado de la Licenciatura en Gestión Universitaria, para demostrar el impacto de la tecnología en cuanto a medir el impacto del software libre en la vinculación territorial. Pensado para senderistas y turistas para explorar cómo la tecnología libre, los mapas offline y las redes comunitarias pueden aportar a la seguridad de las yungas tucumanas.  Todo el sistema fue diseñado como una prueba de concepto abierta y gratuita de codigo abierto.
# Proyecto Yungas 🍃 (Horco Molle)
Es el primer lugar donde se prueba con usuarios reales, y esta en etapa de testing. Tiene la potencialidad de escalarse hasta cubrir mas senderos de la reserva, funiculares, cuesta del cielo, etc. Aspiramos a poder colaborar para el desarrollo de sendas de mas alta complejidad donde el tracking es fundamental en situaciones de emergencias y rescates como ser nunorco, los alisos, y otros. Todo esto puede hacerse mediante triangulación de posiciones al haber multiples usuarios usando la pwa y con la posibilidad( probandola actualmente) de integrar Esp32/Lora , LoRa APRS , para brindar la posibilidad de enviar corrdenadas incluso sin necesidad de conexión 4G/LTE. Dada la necesidad de cuidadr nuestros senderos, la misma tecnologia que se prueba para rescate puede usarse para medir el estado de la naturaleza y tomar decisiones sobre cuales senderos habilitar y cuales dejar descansar o si alguna zona tiene la potencialidad de incendio y avisar a las personas. Todo lo anterior para tomar decisiones en base a datos y sobre todo para prevenir.


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
