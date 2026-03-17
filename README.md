# Water Transfer Track - Sistema de Control de Activos

Sistema de gestión de activos para empresa de water transfer en Río Limay. Permite controlar bombas, carretes layflat, derivadores, mangueras y más.

## Archivos del Proyecto

Este proyecto tiene solo **3 archivos**:

```
water-transfer-github/
├── index.html    → Aplicación completa (HTML + CSS + JS)
├── data.json    → Datos precargados de ejemplo
└── README.md    → Este archivo
```

## Características

- **Gestión de Activos**: Alta, baja y modificación
- **Tipos de Equipos**: Bombas, Carretes Layflat 10"/12", Derivadores, Mangueras Bauer, Acoples Vitáulic, Caudalímetros, Accesorios de Succión, Tanks Australianos
- **Código QR**: Generación automática de códigos para cada activo
- **Operaciones**: Seguimiento por operación
- **Ubicaciones**: Control de bodega y acopio
- **Reportes**: Resúmenes por tipo, estado y operación
- **Exportar PDF**: Generación de reportes en PDF
- **Datos Precargados**: 20 activos de ejemplo listos para usar

## Despliegue en Vercel (3 pasos)

### Paso 1: Subir a GitHub

1. Ve a [github.com](https://github.com) e inicia sesión
2. Click en **"New repository"**
3. Nombre: `water-transfer-track`
4. **NO** marques "Initialize with README"
5. En tu computadora, crea una carpeta y coloca los 3 archivos
6. Sube los 3 archivos desde GitHub (Add file → Upload files)

### Paso 2: Conectar a Vercel

1. Ve a [vercel.com](https://vercel.com) e inicia sesión con GitHub
2. Click en **"Add New"** → **"Project"**
3. Selecciona tu repositorio `water-transfer-track`
4. Vercel detecta automáticamente que es un sitio estático
5. Click en **"Deploy"**

### Paso 3: ¡Listo!

Vercel genera una URL como: `https://water-transfer-track.vercel.app`

## Uso de Datos Precargados

La aplicación viene con **20 activos de ejemplo**:

- 3 Bombas (1 en operación, 1 en bodega, 1 en reparación)
- 5 Carretes Layflat (3 de 12", 2 de 10")
- 2 Derivadores
- 3 Juegos de Mangueras Bauer
- 2 Acoples Vitáulic
- 2 Caudalímetros
- 2 Accesorios de Succión
- 3 Tanks Australianos (5400L)

### Cargar Datos de Ejemplo

Al abrir la aplicación por primera vez:

1. Ve a **Configuración** (ícono de engranaje)
2. Click en **"Importar Datos"**
3. Selecciona el archivo `data.json` incluido
4. Los datos de ejemplo se cargan automáticamente

## Funcionalidades Principales

### Dashboard
- Resumen de activos por estado
- Activos en operación vs en bodega
- Equipos en reparación
- Filtros por tipo y estado

### Gestión de Activos
- Agregar nuevo activo
- Editar información
- Cambiar estado (Bodega → Operación → Reparación → Baja)
- Asignar a operación
- Notas y especificaciones

### Consultas
- Filtrar por tipo de equipo
- Filtrar por operación
- Filtrar por estado
- Búsqueda por código/nombre

### Reportes
- Exportar lista de activos a PDF
- Reporte por operación
- Reporte de inventario

## Tecnologías

- HTML5, CSS3, JavaScript vanilla
- LocalStorage para persistencia
- jsPDF para generación de PDFs
- QRCode.js para códigos QR
- PWA Ready (manifest incluido)

## Nota sobre Datos

La aplicación usa **LocalStorage** del navegador para guardar datos. Esto significa:

✅ Los datos persisten entre sesiones
✅ Funciona offline después de cargar
✅ No requiere servidor ni base de datos
⚠️ Los datos están solo en ese navegador
⚠️ Para respaldar, usa la función exportar en la app

## Licencia

Uso interno - Empresa de Water Transfer Río Limay
