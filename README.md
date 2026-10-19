## 📌 Descripción del Proyecto

El objetivo de este proyecto es realizar la validación y pruebas de la API del backend de **Urban Grocers** para verificar las nuevas actualizaciones relacionadas con:
1. **Trabajar con los Kits** (creación, edición y validación de nombres/parámetros en kits).
2. **Trabajar con los Servicios de Entrega** (cálculo de tarifas, horarios, disponibilidad y productos permitidos).

Se diseñaron e integraron casos de prueba funcionales, positivos y negativos en **Postman**, analizando las respuestas HTTP (`200 OK`, `201 Created`, `400 Bad Request`, `404 Not Found`, etc.) y la estructura de los JSON devueltos.

---

## 🛠️ Herramientas Utilizadas

* **Postman**: Ejecución de solicitudes HTTP (`GET`, `POST`, `PUT`, `DELETE`).
* **Apidoc**: Documentación oficial de la API de Urban Grocers (`base_url/docs/`).
* **Jira**: Registro y gestión de informes de errores (Bug Reports).
* **GitHub**: Control de versiones y almacenamiento de la documentación del proyecto.

---

## 📑 Resumen de la Documentación y Cobertura

### 1. Requisito 1: Trabajar con los Kits
- [x] **Creación de kits:** Validación de nombre con límites de caracteres (mínimos, máximos, caracteres especiales, números y espacios).
- [x] **Códigos de Estado:** Verificación de respuestas `201 Created` para solicitudes válidas y `400 Bad Request` para entradas inválidas.
- [x] **Estructura del JSON:** Comprobación de que la respuesta contiene el ID, nombre y productos del kit creado.

### 2. Requisito 2: Trabajar con los Servicios de Entrega
- [x] **Cálculo de costos y tiempos:** Comprobación de precios según distancia, velocidad de entrega y peso.
- [x] **Disponibilidad de entregas:** Pruebas en diferentes franjas horarias y días de operación.
- [x] **Validación de respuestas:** Verificación de esquemas de respuesta JSON y códigos HTTP correspondientes.

---

## 🐞 Reportes de Errores (Jira)

Cualquier discrepancia entre la documentación en **Apidoc / Requisitos de Backend** y la respuesta obtenida en **Postman** fue registrada en Jira con la siguiente estructura:
- **Resumen del error / Endpoint afectado**
- **Método HTTP y URL**
- **Body de la solicitud (Request Body)**
- **Resultado Esperado vs. Resultado Obtenido (Response Status & Body)**
- **Severidad y Prioridad**
