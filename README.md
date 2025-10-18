# 🚀 Agentum Landing Page

Landing page para capturar leads y solicitudes de demo de Agentum.

**Esta landing está diseñada para ser hosteada en un repositorio separado** (GitHub Pages, Vercel, Netlify, etc.) independiente del backend principal de Agentum.

## 📁 Estructura de Archivos

```
landing_page/
├── index.html          # Landing page principal
├── favicon.png         # Icono del sitio
├── images/
│   └── agentum-logo.png   # Logo de Agentum
├── README.md           # Este archivo
└── .gitignore          # Archivos a ignorar en git
```

## 🚀 Despliegue

Esta landing page está diseñada para ser hosteada en:
- **GitHub Pages** (recomendado para estático)
- **Vercel**
- **Netlify**
- Cualquier servidor web estático

## 📧 Captura de Leads

✅ **Formspree configurado** - Los leads se envían automáticamente a Formspree cuando alguien llena el formulario.

### Funcionamiento:

- Los leads se envían directamente a Formspree: https://formspree.io/f/xjkazbod
- Recibirás notificaciones por email en la cuenta de Formspree
- Puedes exportar los leads desde el panel de Formspree

### Ver Leads:

**Panel de Formspree**: https://formspree.io/forms/xjkazbod/submissions

Desde ahí puedes:
- Ver todos los leads capturados
- Exportar a CSV, Google Sheets, etc.
- Configurar webhooks
- Integrar con tu CRM

## 🛠️ Configuración

### Para hostear en GitHub Pages:

1. Crea un nuevo repositorio en GitHub
2. Sube los archivos de la carpeta `landing_page`
3. Ve a Settings → Pages
4. Selecciona la rama `main` y carpeta `/ (root)`
5. Guarda y espera unos minutos

Tu landing estará en: `https://tu-usuario.github.io/nombre-repo/`

### Para usar dominio personalizado:

1. En GitHub Pages settings, agrega tu dominio custom
2. Crea un archivo `CNAME` con tu dominio:
```
landing.agentum.com
```
3. Configura DNS:
```
Type: CNAME
Name: landing
Value: tu-usuario.github.io
```

## 📊 Ver Leads Capturados

**Opción 1: Desde el navegador**
```javascript
// En la consola del navegador
localStorage.getItem('agentum_leads')
```

**Opción 2: Exportar a CSV**
```javascript
// En la consola del navegador
exportLeads()
```

**Opción 3: Desde tu backend**
Consulta tu base de datos o endpoint `/api/leads/`

## 🎨 Personalización

Los colores están definidos en las variables CSS al inicio del archivo:
```css
:root {
    --color-primary: #1b9ca7;
    --color-primary-hover: #16828c;
    ...
}
```

## 📝 Slogan

**"Tu empresa, Tu agente, Tu manera"**

## 🔔 Notificaciones

Una vez configurado Formspree o tu backend, puedes recibir notificaciones automáticas por email cuando llegue un nuevo lead.

## 🌐 SEO

La landing incluye:
- Meta description optimizado
- Títulos semánticos (H1, H2, H3)
- Alt texts para accesibilidad
- Responsive design
- Performance optimizado

## 📱 Responsive

La landing es completamente responsive y se adapta a:
- Desktop (1280px+)
- Tablet (768px - 1024px)
- Mobile (< 768px)

## 🎯 Métricas Recomendadas

Para trackear conversiones, puedes integrar:
- Google Analytics
- Facebook Pixel
- LinkedIn Insight Tag
- Hotjar (para heatmaps)

Agrega los scripts antes de `</body>`.

