# 📦 Sistema de Pendientes de Compra

Sistema web para gestión y control de pendientes de compra con sincronización en tiempo real.

## ✨ Características

- 🔐 Sistema de login con 8 usuarios (4 compras + 4 facturación)
- 📝 Creación de pendientes de compra
- 🎨 Código de colores automático según días pendientes
- 🔍 Filtros por cliente, empresa y fecha
- 📊 Exportación a Excel/CSV
- 👥 Gestión de usuarios (solo equipo de compras)
- 🗑️ Eliminación de pendientes (solo equipo de compras)
- 💾 Guardado automático en tiempo real
- 📱 Responsive - funciona en móviles y tablets

## 👥 Usuarios del Sistema

### Equipo de Compras (Acceso Total)
- **CCOMETA** - Carlos Hernán Cometa Osso (Contraseña: CC123)
- **JKTRUJILLO** - Jean Karlo Trujillo (Contraseña: JK.2026)
- **JSTERLING** - Javier Sterling Bermúdez (Contraseña: JS.2026)
- **AMSANCHEZ** - Ana María Sánchez (Contraseña: AN.2026)

### Auxiliares de Facturación (Solo Crear y Ver)
- **DAYANNA.V1** - Dayanna - Ventas 1 (Contraseña: DV1.123)
- **KATALINA.V2** - Katalina - Ventas 2 (Contraseña: KV2.123)
- **JULIETH.V3** - Julieth - Ventas 3 (Contraseña: JV3.123)
- **MARICELA.V4** - Maricela - Ventas 4 (Contraseña: MV4.123)

## 🚀 Despliegue en Vercel

### Opción 1: Deploy desde GitHub (Recomendado)

1. **Sube este repositorio a GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/sistema-pendientes-compra.git
   git push -u origin main
   ```

2. **Ve a Vercel:**
   - Visita: https://vercel.com/new
   - Conecta con GitHub
   - Selecciona este repositorio
   - Framework Preset: **Vite**
   - Click en "Deploy"

3. **¡Listo!** Tu app estará disponible en:
   ```
   https://sistema-pendientes-compra.vercel.app
   ```

### Opción 2: Deploy directo con Vercel CLI

```bash
npm install -g vercel
vercel
```

## 💻 Desarrollo Local

### Requisitos
- Node.js 16+ (Descargar de https://nodejs.org)
- npm o yarn

### Instalación

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/TU-USUARIO/sistema-pendientes-compra.git
   cd sistema-pendientes-compra
   ```

2. **Instalar dependencias:**
   ```bash
   npm install
   ```

3. **Ejecutar en modo desarrollo:**
   ```bash
   npm run dev
   ```

4. **Abrir en el navegador:**
   ```
   http://localhost:5173
   ```

### Build para producción

```bash
npm run build
```

Los archivos compilados estarán en la carpeta `dist/`

## 📁 Estructura del Proyecto

```
sistema-pendientes-compra/
├── index.html              # HTML principal
├── package.json            # Dependencias del proyecto
├── vite.config.js          # Configuración de Vite
├── README.md               # Este archivo
└── src/
    ├── main.jsx            # Punto de entrada de React
    └── App.jsx             # Componente principal del sistema
```

## 🔧 Tecnologías Utilizadas

- **React 18** - Framework de interfaz
- **Vite** - Build tool y dev server
- **Tailwind CSS** - Estilos (vía CDN)
- **Lucide React** - Iconos
- **Vercel** - Hosting y deployment

## 📝 Funcionalidades por Rol

### Equipo de Compras puede:
- ✅ Crear pendientes
- ✅ Ver todos los pendientes
- ✅ Marcar pendientes como OK
- ✅ Agregar/editar observaciones
- ✅ Eliminar pendientes
- ✅ Exportar a Excel
- ✅ Agregar nuevos usuarios
- ✅ Usar todos los filtros

### Auxiliares de Facturación pueden:
- ✅ Crear pendientes
- ✅ Ver todos los pendientes
- ✅ Usar filtros de búsqueda
- ❌ No pueden editar
- ❌ No pueden eliminar
- ❌ No pueden marcar como OK
- ❌ No pueden exportar
- ❌ No pueden agregar usuarios

## 🎨 Código de Colores

- 🟢 **Verde** - Pendiente marcado como OK
- 🟡 **Amarillo** - Pendiente de 0-1 días
- 🔴 **Rojo** - Pendiente de más de 1 día (URGENTE)

## 🔍 Filtros Disponibles

1. **Por Cliente** - Búsqueda por nombre
2. **Por Empresa** - IMPSURMEDICALS / HABILITEMOS / TODAS
3. **Por Fecha** - Rango desde-hasta

## 📊 Exportación a Excel

El botón de exportación genera un archivo CSV con:
- Fecha
- Producto, Marca, Cantidad
- Cliente y Empresa
- Solicitado por
- Días pendiente
- Estado actual
- Observaciones
- Datos de gestión

Compatible con Excel, Google Sheets, LibreOffice, etc.

## 🐛 Solución de Problemas

### La aplicación no carga
- Verifica que todas las dependencias estén instaladas: `npm install`
- Limpia la caché: `npm run build -- --force`

### Los datos no se guardan
- Asegúrate de tener conexión a internet
- Verifica la consola del navegador (F12) para ver errores
- Los datos se guardan usando `window.storage` (requiere Claude.ai)

### Error al desplegar en Vercel
- Verifica que el Framework Preset sea **Vite**
- Revisa los logs de build en Vercel
- Asegúrate que `package.json` tenga todas las dependencias

## 📞 Soporte

Para reportar problemas o sugerencias, contacta al equipo de desarrollo.

## 📄 Licencia

Este proyecto es de uso interno para la gestión de compras.

---

**Desarrollado para optimizar el proceso de gestión de pendientes de compra** 🚀
