# Automatización de Pruebas: Solicitud de Taxi en Urban Routes

## 📝 Descripción del Proyecto
Este proyecto implementa un conjunto de pruebas de automatización web con Python y Selenium WebDriver para verificar el flujo completo de solicitud de un servicio de taxi en la aplicación web de Urban Routes. Utiliza pruebas atómicas estructuradas bajo el patrón Page Object Model (POM), garantizando que cada interacción del usuario sea validada de forma independiente y eficiente.

## 🎯 Objetivo
Automatizar y verificar el flujo completo de solicitud de taxi en Urban Routes, asegurando que cada escenario cumpla con los requisitos funcionales establecidos, desde la configuración de la ruta hasta la asignación del conductor.

## 🔍 Alcance
- ✅ Incluido: flujo completo de solicitud de taxi (ruta, tarifa, pago, conductor)
- ❌ Excluido: pruebas de rendimiento y pruebas en dispositivos móviles

## 🛠️ Tecnologías y Técnicas Utilizadas
- **Python**: Lenguaje de programación principal
- **Selenium WebDriver**: Herramienta de automatización
- **Pytest**: Framework para ejecución y estructuración de tests
- **Page Object Model (POM)**: Patrón de diseño para modularizar el código
- **Manejo de IFrames**: Para interactuar con campos de tarjeta de crédito y CVV
- **Sincronización**: Esperas implícitas y explícitas con WebDriverWait
- **Localizadores variados**: By.ID, By.XPATH, By.CSS_SELECTOR, By.CLASS_NAME

## 🧪 Escenarios de Prueba Cubiertos
1. `test_set_route`: Configuración y verificación de direcciones
2. `test_select_rate`: Selección de tarifa Comfort
3. `test_get_tel_code`: Ingreso y confirmación del código de teléfono
4. `test_add_creditcard`: Agrega tarjeta de crédito (manejando iframes)
5. `test_send_message`: Escribe mensaje para el conductor
6. `test_add_blanket_and_tissues`: Habilita manta y pañuelos
7. `test_add_two_icecream`: Agrega 2 helados al pedido
8. `test_order_modal`: Inicia pedido y verifica modal de búsqueda
9. `test_driver_modal`: Espera y verifica asignación del conductor

## ⚙️ Decisiones Clave
- **POM**: Elegido para separar la lógica de pruebas de la interacción con la UI, facilitando el mantenimiento del código
- **Pruebas atómicas**: Cada prueba valida una sola acción, lo que facilita identificar exactamente dónde falla el flujo
- **Esperas explícitas + implícitas**: Combinadas para manejar elementos dinámicos sin hacer el código frágil

## 📊 Resultados
- 9 escenarios de prueba automatizados cubriendo el flujo completo end-to-end
- Flujo validado exitosamente desde configuración de ruta hasta asignación de conductor

## 🔄 ¿Qué mejoraría después?
- Integrar las pruebas en un pipeline de CI/CD con GitHub Actions
- Agregar pruebas de regresión para escenarios alternativos

## 🚀 Cómo Ejecutar las Pruebas
1. Crear entorno virtual: `python -m venv .venv`
2. Activar entorno virtual:
   - macOS/Linux: `source .venv/bin/activate`
   - Windows: `.venv\Scripts\Activate.ps1`
3. Instalar dependencias: `pip install -r requirements.txt`
4. Ejecutar pruebas: `pytest main.py`

## 👩‍💻 Autora
Mónica Vasco | QA Analyst
