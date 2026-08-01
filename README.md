# 🧩 Sistema de Gestión Empresarial — Power Apps + SharePoint

Aplicación de gestión empresarial desarrollada con **Microsoft Power Apps** (Canvas App) y **SharePoint** como fuente de datos, creada como proyecto práctico durante un curso de formación en desarrollo low-code.

La app centraliza la administración de **empleados, ventas, contactos y productos** de una organización, permitiendo registrar, consultar y editar información desde una interfaz visual e intuitiva.

---

## 📌 Descripción general

El objetivo del proyecto fue construir una solución funcional de extremo a extremo dentro del ecosistema de **Microsoft Power Platform**, cubriendo todo el flujo de trabajo típico de una aplicación empresarial: alta de registros, listados, edición y navegación entre módulos, conectada a listas de SharePoint como backend.

**Stack utilizado:**
- Microsoft **Power Apps** (Canvas App)
- **SharePoint Online** (fuentes de datos / listas)
- Fórmulas de Power Fx para lógica de negocio y validaciones

---

## 🗂️ Fuentes de datos

La aplicación se conecta a cuatro listas de SharePoint, cada una representando una entidad clave del negocio:

| Fuente de datos | Descripción |
|---|---|
| **Empleados** | Información del personal registrado (nombre, correo, departamento, salario, fecha de ingreso) |
| **Ventas** | Registro de transacciones/ventas realizadas |
| **Contactos** | Directorio de contactos asociados a la organización |
| **Productos** | Catálogo de productos disponibles |

---

## 🖥️ Estructura de pantallas

La app está organizada en pantallas independientes, siguiendo buenas prácticas de navegación en Power Apps:

- **`pantalla_inicio`** — Pantalla de bienvenida y punto de entrada a la aplicación
- **`pantalla_editar`** — Formulario de registro/edición de empleados
- **`pantalla_lista_empleados`** — Listado general de empleados registrados
- **`pantalla_lista_ventas`** — Listado de ventas realizadas
- **`pantalla_nueva_venta`** — Formulario para registrar una nueva venta

![Estructura de pantallas](Vista-de-arbol.jpeg)
*Vista de árbol con la organización de pantallas de la aplicación.*

---

## 📝 Funcionalidad destacada: Registro de Empleados

Uno de los módulos principales permite dar de alta nuevos empleados capturando:

- **Nombre del empleado**
- **Correo electrónico**
- **Departamento** (selector desplegable)
- **Salario** (con validación de formato, dos decimales)
- **Fecha de ingreso** (selector de calendario, con valor por defecto la fecha actual)

El formulario incluye **validaciones en tiempo real**: los campos obligatorios se resaltan y se muestran advertencias cuando falta completar información (por ejemplo, el selector de departamento sin seleccionar).

![Pantalla de registro de empleados](Registro-de-empleado.jpeg)
*Formulario "Registrar Empleado" con validaciones visuales de campos obligatorios.*

---

## ✅ Aspectos técnicos aplicados

- Conexión y consumo de **múltiples listas de SharePoint** como fuentes de datos.
- Uso de **controles de formulario** (Edit Form / controles de entrada) con reglas de validación.
- **Navegación entre pantallas** mediante `Navigate()` y organización modular por funcionalidad.
- Fórmulas de **Power Fx** para lógica condicional y control de errores de entrada.
- Diseño de interfaz con **menú lateral de navegación** (Empleados, Contactos, Productos, Usuarios, Ventas).

---

## 📎 Nota

Este proyecto fue desarrollado con fines de aprendizaje como parte de un curso de capacitación en Power Apps. El archivo `.zip` con la solución exportada está disponible bajo solicitud.

---

### 👩‍💻 Autora
**Blanca Avalos Durand**
