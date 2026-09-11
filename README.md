# Control de Reactivos y Consumibles - Hematología

Sistema interactivo de gestión de inventario de reactivos para el **Servicio de Hematología del Hospital Universitario "Dr. José Eleuterio González"**.

## ✨ Características

- 📥 **Registro de entrada** - Captura automática de lotes, fechas y datos
- ⚙️ **Seguimiento de uso** - Registra cuándo se usa cada reactivo
- 🗑️ **Control de baja** - Documenta el retiro del inventario
- 🔐 **Seguridad con contraseña** - `hemato2026` para desbloquear registros
- 📊 **Exportar a Excel** - Descarga los datos en formato CSV
- 💾 **Almacenamiento local** - Los datos se guardan en tu navegador
- 📱 **Responsive** - Funciona en computadoras, tablets y celulares

## 🚀 Instalación rápida

### Opción 1: GitHub Pages (Recomendado)

1. **Sube el archivo `index.html`** a tu repositorio:
   - Ve a: https://github.com/yairchaveze/control-de-reactivo-hemato-hu
   - Click en "Add file" → "Upload files"
   - Selecciona `index.html`
   - Commit

2. **Activa GitHub Pages:**
   - Ve a Settings del repositorio
   - Busca "GitHub Pages"
   - Selecciona `main` branch
   - Guarda

3. **Tu app estará en:**
   ```
   https://yairchaveze.github.io/control-de-reactivo-hemato-hu/
   ```

### Opción 2: Local (Desarrollo)

Solo abre el archivo `index.html` en tu navegador. ¡Funciona sin conexión!

---

## 🖼️ Configurar logo

El sistema incluye un banner con los logos del UANL, Hospital Universitario y Centro Universitario Contra el Cáncer.

### Pasos para subir tu logo:

1. **Crea una carpeta `logos`** en tu repositorio
   - Ve a tu repositorio en GitHub
   - Click en "Add file" → "Create new file"
   - Escribe: `logos/.gitkeep`
   - Commit

2. **Sube la imagen:**
   - Desde GitHub web: "Add file" → "Upload files"
   - Sube tu imagen PNG o JPG:
     - `inicio-logo01.png` (o cámbialo a otro nombre)

3. **La URL se forma automáticamente:**
   ```
   https://raw.githubusercontent.com/yairchaveze/control-de-reactivo-hemato-hu/main/logos/inicio-logo01.png
   ```

4. **Si cambias el nombre del archivo**, edita el `index.html`:
   - Busca: `inicio-logo01.png`
   - Reemplaza con tu nombre de archivo

---

## 📖 Cómo usar

### Flujo típico:

1. **Selecciona modo:**
   - 📥 **Entrada** - Reactivo llega al laboratorio
   - ⚙️ **Uso** - Se utiliza el reactivo
   - 🗑️ **Baja** - Se retira del inventario

2. **Escanea o escribe el código de lote**
   - Si es nuevo: Completa datos (Producto, Fabricante, etc.)
   - Si existe: Llena los datos faltantes

3. **Los datos se guardan automáticamente**
   - Bloqueados después de completar cada etapa
   - Para editar: ingresa contraseña `hemato2026`

4. **Exporta cuando necesites:**
   - Click en "Exportar a Excel"
   - Se descarga en formato CSV

---

## 🔒 Seguridad

- **Contraseña:** `hemato2026`
- Los registros se **bloquean automáticamente** después de completarse
- Para modificar un registro bloqueado, debes ingresar la contraseña
- Esto crea un **historial de auditoría** (registro de cambios)

---

## 💾 Datos

- Se guardan **localmente en tu navegador** (localStorage)
- **No se envían a servidores** - privacidad garantizada
- Borrar datos del navegador = borrar los registros
- Recomendación: **Exporta regularmente a Excel** como respaldo

---

## 🎨 Personalización

Puedes editar el archivo `index.html` para:
- Cambiar colores: Busca `#0C447C` (azul principal)
- Cambiar contraseña: Busca `const CONTRASEÑA = 'hemato2026'`
- Cambiar nombre del hospital
- Agregar más campos al registro

---

## 📱 Acceso desde móvil

La app es **totalmente responsive**. Accede desde:
- Computadora de escritorio
- Tablet
- Celular (recomendado para escanear códigos con cámara)

---

## 🐛 Soporte

Si encuentras problemas:

1. Verifica que el logo esté en la carpeta `logos/inicio-logo01.png`
2. Limpia el cache del navegador (Ctrl+Shift+Del)
3. Prueba en otro navegador
4. Revisa la consola (F12 → Console)

---

## 📄 Versión

**Control de Reactivos v1.0**

Desarrollado para el Servicio de Hematología - UANL

---

## 📚 Especificaciones técnicas

- **Lenguaje:** HTML5, CSS3, JavaScript vanilla
- **Almacenamiento:** localStorage del navegador
- **Exportación:** CSV (compatible con Excel)
- **Sin dependencias externas:** Funciona offline
- **Compatible:** Chrome, Firefox, Safari, Edge

---

¿Necesitas ayuda? Abre un issue en el repositorio 🚀
