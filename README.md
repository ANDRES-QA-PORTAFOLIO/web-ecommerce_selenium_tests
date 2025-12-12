# 🏦 ecommerce_selenium_tests: Suite de Automatización de Pruebas de Comportamiento (BDD)

Suite de pruebas automatizadas diseñada para validar las funcionalidades clave de una aplicación de demostración bancaria. Este proyecto implementa el patrón de diseño Page Object Model (POM) y utiliza la metodología de Desarrollo Guiado por Comportamiento (BDD) con Gherkin.

---

## 🚀 Tecnologías y Herramientas de Automatización

Este proyecto utiliza un conjunto de herramientas modernas para garantizar la eficiencia, mantenibilidad y reportabilidad de las pruebas automatizadas.

| Categoría | Tecnología/Herramienta | Descripción y Uso |
| :--- | :--- | :--- |
| **Lenguaje** | **Java** (JDK 17) | Lenguaje principal de desarrollo y ejecución de la suite. |
| **Automatización Web** | **Selenium WebDriver** (4.21.0) | Motor para la interacción con el navegador y la ejecución de acciones en la web. |
| **BDD** | **Cucumber-JVM** (7.3.0) y **Gherkin** | Framework de BDD para la definición de escenarios de prueba en un lenguaje natural y legible, separando las especificaciones del código. |
| **Gestión de Dependencias** | **Maven** | Herramienta de automatización de compilación y gestión de dependencias del proyecto. |
| **Configuración de Drivers** | **WebDriverManager** (5.8.0) | Simplifica la gestión automática de los *drivers* de los navegadores (Chrome, Firefox, etc.). |
| **Reporting Avanzado** | **Allure Reporting** (2.31.0) | Generación de informes de pruebas interactivos y detallados, incluyendo capturas de pantalla y pasos de ejecución. |
| **Reporting Alternativo** | **ExtentReports** (5.0.6) | Una herramienta adicional para la generación de informes detallados de la ejecución de las pruebas. |
| **Utilidades** | **Lombok** (1.18.24) | Biblioteca de apoyo para reducir el código *boilerplate* en clases Java (ej. *getters*, *setters*, constructores). |
| **Logging** | **SLF4J API** (2.0.13) | Interfaz de *logging* utilizada para una gestión de registros flexible y desacoplada. |

---

## 🎯 Alcance de la Automatización

La suite se enfoca en la validación del comportamiento de las siguientes funcionalidades críticas de la aplicación bancaria de demostración:

* **Registro de Clientes:** Verificación del flujo de alta de nuevos usuarios.
* **Apertura de Cuentas:** Validación de la creación exitosa de cuentas para un cliente.
* **Gestión de Cuentas:** Pruebas relacionadas con la consulta y administración de las cuentas de un cliente.
* **Pagos de Servicios/Transferencias:** Validación del proceso de transferencia de fondos entre cuentas.

---

## 📐 Estructura y Patrones de Diseño

El proyecto está estructurado para maximizar la **reusabilidad** y la **mantenibilidad** del código de prueba:

* **Page Object Model (POM):** Cada página o componente significativo de la interfaz de usuario está representado por una clase Java dedicada, encapsulando sus *localizadores* y la lógica de interacción.
* **Estructura de Directorios:**
    * `src/main/java`: Pages Objects
    * `src/test/java`: Step Definitions, runners.
    * `src/test/resources`: Archivos `.feature` de Cucumber escritos en Gherkin.

---

## ⚙️ Integración Continua (CI)

La ejecución de las pruebas está diseñada para ser integrada en pipelines de **Integración Continua** (CI), siendo **Jenkins** la herramienta preferida para la compilación, prueba y despliegue continuo del proyecto. Esto asegura que cualquier cambio en el código sea validado automáticamente contra la suite de pruebas.

---

## 📖 Configuración y Ejecución Local

Sigue estos pasos para poner en marcha y ejecutar las pruebas en tu entorno local:

1.  **Clonar el Repositorio:**
    ```bash
    git clone https://github.com/ANDRES-QA-PORTAFOLIO/web-ecommerce_selenium_tests.git
    ```
2.  **Prerrequisitos:** Asegúrate de tener **Java JDK 17** y **Apache Maven** instalados y configurados.
3.  **Ejecución de Pruebas:** Ejecuta la suite completa utilizando Maven:
    ```bash
    mvn clean test
    ```
4.  **Generación de Reportes Allure:** Para visualizar el informe detallado, ejecuta (después de `mvn test`):
    ```bash
    mvn allure:serve
    ```

---

## 📸 Evidencia de Ejecución (Allure Reports)

Los reportes de Allure ofrecen una vista clara del estado de las pruebas.

| Estado | Última Versión |
| :--- | :--- |
| **Release** | ![GitHub Release](https://img.shields.io/github/v/release/ANDRES-QA-PORTAFOLIO/web-ecommerce_selenium_tests) |

![Screenshot de un reporte Allure - Evidencia 1](https://github.com/ANDRES-QA-PORTAFOLIO/web-ecommerce_selenium_tests/releases/download/V1.0.0/evidencia_1765559136790.png)

![Screenshot de un reporte Allure - Evidencia 2](https://github.com/ANDRES-QA-PORTAFOLIO/web-ecommerce_selenium_tests/releases/download/V1.0.0/evidencia_1765559142499.png)
