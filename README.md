# 🏠 Anfitrio — Gestión de Cambio para Alquiler Vacacional

App web multi-empresa para gestionar el cambio de inquilinos en apartamentos de alquiler vacacional. Funciona como PWA instalable en móvil y tablet (Android 16 / iOS).

## 📁 Archivos

| Archivo | Descripción |
|---|---|
| `index.html` | App principal — checklist, suministros, fotos, late check-out |
| `login.html` | Pantalla de acceso con Firebase Authentication |
| `admin.html` | Panel de administración — empresas, usuarios, historial |
| `firestore.rules` | Reglas de seguridad Firestore (aisla empresas entre sí) |

## ✨ Funcionalidades

- ✅ **Multi-empresa** — cada empresa ve solo sus datos
- 👥 **Roles** — admin y empleado con permisos diferenciados
- 📋 **Checklist** de tareas de limpieza con progreso
- ⚡ **Control de suministros** (luz y agua) con cálculo de consumo
- 🔑 **Inventario y llaves**
- ⚠️ **Incidencias** con notas libres
- 📸 **Fotos de desperfectos**
- 🕐 **Late check-out** con cálculo de retraso y cargo
- 📄 **Exportar PDF** profesional
- 💬 **Enviar por WhatsApp** con resumen completo
- ☁️ **Sincronización automática** con Firebase Firestore
- 📱 **PWA instalable** en pantalla de inicio (Android / iOS)
- 🌙 **Dark mode** automático
- 📐 **Responsive** — móvil, tablet, plegables, landscape

## 🔧 Tecnologías

- HTML + CSS + JavaScript vanilla (sin frameworks)
- Firebase Authentication (email/password)
- Cloud Firestore (base de datos en tiempo real)
- jsPDF (generación de PDF)
- CSS custom properties + media queries para responsive

## 🚀 Instalación

### 1. Clonar el repositorio
```bash
git clone https://github.com/TU_USUARIO/anfitrio-app.git
cd anfitrio-app
```

### 2. Configurar Firebase
Las claves ya están incluidas en los archivos. Si clonas para otro proyecto, edita el bloque `firebaseConfig` en los 3 archivos HTML.

### 3. Aplicar las Security Rules
En Firebase Console → Firestore → Reglas → pega el contenido de `firestore.rules` → Publicar.

### 4. Abrir la app
Abre `login.html` en el navegador o súbela a Firebase Hosting / cualquier servidor web estático.

### 5. Crear el primer admin
Ver guía completa en la documentación del proyecto.

## 🔐 Seguridad

Las Security Rules de Firestore garantizan que:
- Una empresa **nunca** puede acceder a datos de otra
- Los empleados solo pueden crear y leer checkouts de su empresa
- Solo los admins pueden gestionar usuarios y empresas
- Todo acceso requiere autenticación

## 📱 Instalar en móvil

**Android:** Chrome → tres puntos → "Añadir a pantalla de inicio"  
**iOS:** Safari → Compartir → "Añadir a pantalla de inicio"

---

Desarrollado con ❤️ para propietarios de alquiler vacacional
