# Control de Reactivos y Consumibles - Hematología

Sistema interactivo de gestión de inventario de reactivos para el **Servicio de Hematología del Hospital Universitario "Dr. José Eleuterio González"**.

## ✨ Características v2.0

- 📥 **Registro de entrada** - Captura lote, producto, fabricante, fecha de caducidad y cantidad de piezas
- ⚙️ **Seguimiento de uso** - Registra cuándo se utiliza cada pieza
- 🗑️ **Control de baja** - Documenta el retiro de inventario (por pieza)
- 📦 **Control por piezas** - Si recibes 6 piezas, crea 6 registros independientes
- 🔐 **Seguridad con contraseña** - `hemato2026` para desbloquear registros
- 📊 **Exportar a Excel** - CSV compatible con Excel
- 🖨️ **Imprimir reportes** - Genera reportes formateados para imprimir
- 💾 **Historial permanente** - Los datos NUNCA se borran (auditoría)
- 📱 **Responsive** - Funciona en computadoras, tablets y celulares
- ✅ **Múltiples lotes iguales** - Permite registrar el mismo lote en diferentes fechas

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

El sistema ya incluye la referencia al logo que subiste: `inicio-logo01.png`

### Si el logo no aparece:

1. Verifica que subiste la imagen directamente en la raíz del repositorio (no en carpeta)
   - ✅ Correcto: `https://github.com/yairchaveze/control-de-reactivo-hemato-hu/blob/main/inicio-logo01.png`
   - ❌ Incorrecto: `logos/inicio-logo01.png`

2. Si lo subiste en carpeta, ajusta la URL en `index.html`:
   - Busca: `inicio-logo01.png`
   - Reemplaza por: `logos/inicio-logo01.png`

---

## 📖 Cómo usar

### Flujo de entrada:

1. **Selecciona modo: ENTRADA**
   - 📥 Entrada (para reactivos nuevos)

2. **Escanea o escribe el código de lote**
   - Pega el código en la caja
   - Click en "Aceptar" (o presiona Enter)

3. **Si es la primera vez del lote:**
   - Se abre un formulario
   - Completa: Producto, Fabricante, Fecha de caducidad, Número de piezas
   - Si recibiste 6 piezas → escribe `6`
   - El sistema crea automáticamente 6 registros (1, 2, 3, 4, 5, 6)

4. **Si es el mismo lote 2 meses después:**
   - El sistema lo reconoce como NUEVO ingreso (diferente fecha)
   - Crea nuevos registros para esas piezas

### Flujo de uso:

1. **Selecciona modo: USO**
2. **Escanea el código de lote**
3. **Si hay múltiples piezas:**
   - El sistema muestra: "Hay 6 piezas de este lote"
   - Pide que escanees de nuevo para cada pieza que uses
4. **Registra la verificación del desempeño** (Ej: VISUAL OK)
5. **La pieza se marca como usada** ✅

### Flujo de baja:

1. **Selecciona modo: BAJA**
2. **Escanea el código de lote**
3. **Confirma la baja de la pieza específica**
4. **La pieza se marca como dada de baja** ✅

### Acciones principales:

- **Imprimir**: Abre una vista de impresión del inventario actual
- **Exportar Excel**: Descarga un archivo CSV con todos los datos (histórico completo)

**⚠️ IMPORTANTE:** Los datos NUNCA se borran. Siempre tendrás el histórico completo.

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
