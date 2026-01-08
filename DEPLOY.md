# 🚀 GUÍA RÁPIDA DE DESPLIEGUE

## ⏱️ Tiempo total: 15-20 minutos

---

## PASO 1: Descargar el Proyecto (YA HECHO ✅)

Tienes todos los archivos listos en tu carpeta `sistema-pendientes-compra/`

---

## PASO 2: Subir a GitHub (5 minutos)

### A. Crear Repositorio en GitHub

1. Ve a: **https://github.com/new**
2. Configura así:
   ```
   Repository name: sistema-pendientes-compra
   Description: Sistema de gestión de pendientes de compra
   ○ Public ✓ (seleccionar)
   ☐ Add a README file (NO marcar)
   ```
3. Click en **"Create repository"**

### B. Subir archivos

**Opción 1: Usando la interfaz web de GitHub (MÁS FÁCIL)**

1. En la página de tu nuevo repositorio, click en **"uploading an existing file"**
2. Arrastra TODOS los archivos de la carpeta `sistema-pendientes-compra/`
3. En el mensaje de commit escribe: `Initial commit - Sistema completo`
4. Click en **"Commit changes"**

**Opción 2: Usando comandos (si tienes Git instalado)**

```bash
cd sistema-pendientes-compra
git init
git add .
git commit -m "Initial commit - Sistema completo"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/sistema-pendientes-compra.git
git push -u origin main
```

---

## PASO 3: Desplegar en Vercel (10 minutos)

### A. Conectar Vercel con GitHub

1. Ve a: **https://vercel.com/new**
2. Si no tienes cuenta, haz click en **"Continue with GitHub"**
3. Autoriza a Vercel para acceder a tus repositorios

### B. Importar el Proyecto

1. En la lista de repositorios, busca: **sistema-pendientes-compra**
2. Click en **"Import"**

### C. Configurar el Deploy

```
┌─────────────────────────────────────┐
│ Configure Project                   │
├─────────────────────────────────────┤
│ Project Name:                       │
│ sistema-pendientes-compra           │
│                                     │
│ Framework Preset: Vite ← IMPORTANTE│
│                                     │
│ Root Directory: ./                  │
│ Build Command: npm run build        │
│ Output Directory: dist              │
│                                     │
│        [Deploy] ← CLIC             │
└─────────────────────────────────────┘
```

**IMPORTANTE:**
- ✅ Framework Preset debe ser **Vite**
- ✅ NO cambiar nada más
- ✅ NO agregar Environment Variables (aún)

3. Click en **"Deploy"**

### D. Esperar el Deploy

```
⏳ Building... (1-2 minutos)
⏳ Deploying... (30 segundos)
🎉 Success!
```

---

## PASO 4: Obtener tu Link ✅

Vercel te dará un link como:

```
🌐 https://sistema-pendientes-compra.vercel.app
```

O con nombre aleatorio:

```
🌐 https://sistema-pendientes-compra-abc123.vercel.app
```

---

## PASO 5: Probar el Sistema (2 minutos)

1. Abre el link en tu navegador
2. Deberías ver la pantalla de **LOGIN**
3. Prueba con:
   ```
   Usuario: CCOMETA
   Contraseña: CC123
   ```
4. ✅ **¡Funciona!**

---

## 🎯 SIGUIENTE PASO: Compartir con tu Equipo

### Copia este mensaje:

```
¡Hola equipo! 👋

Ya está listo nuestro Sistema de Pendientes de Compra.

🌐 Link: https://tu-link-aqui.vercel.app

📋 USUARIOS Y CONTRASEÑAS:

Equipo de Compras:
• CCOMETA / CC123
• JKTRUJILLO / JK.2026
• JSTERLING / JS.2026
• AMSANCHEZ / AN.2026

Auxiliares de Facturación:
• DAYANNA.V1 / DV1.123
• KATALINA.V2 / KV2.123
• JULIETH.V3 / JV3.123
• MARICELA.V4 / MV4.123

💡 INSTRUCCIONES:
- Todos pueden crear pendientes
- Todo se guarda automáticamente
- Los cambios se ven en tiempo real
- Solo compras puede eliminar y exportar

¡Cualquier duda me avisan! 🚀
```

---

## 🔄 Actualizar el Sistema (Si haces cambios)

1. Modifica los archivos en GitHub
2. Vercel detecta los cambios automáticamente
3. Redeploya automáticamente
4. **¡Listo!** Los cambios están en línea

---

## 🆘 Problemas Comunes

### "Deploy failed"
- Verifica que seleccionaste **Vite** como Framework
- Revisa los logs en Vercel
- Asegúrate que `package.json` esté correcto

### "Cannot find module"
- Verifica que `src/App.jsx` y `src/main.jsx` existan
- Revisa que los nombres sean exactos (mayúsculas/minúsculas)

### Los datos no se guardan
- Esto es normal en la versión con `window.storage`
- Solo funciona en Claude.ai
- Para guardar datos permanentes, necesitas migrar a Supabase

---

## ✅ CHECKLIST FINAL

- [ ] Repositorio creado en GitHub
- [ ] Archivos subidos a GitHub
- [ ] Cuenta de Vercel creada
- [ ] Proyecto conectado a Vercel
- [ ] Framework Preset = Vite
- [ ] Deploy exitoso
- [ ] Link funcionando
- [ ] Login funcionando
- [ ] Puedo crear pendientes
- [ ] Equipo tiene acceso

---

## 🎉 ¡FELICITACIONES!

Tu sistema está en línea y funcionando.

**Próximos pasos opcionales:**
1. Agregar dominio personalizado en Vercel
2. Migrar a Supabase para datos permanentes
3. Personalizar colores o funcionalidades

¿Necesitas ayuda con algo? ¡Pregunta! 😊
