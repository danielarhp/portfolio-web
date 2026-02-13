# 🔧 Solución: CSS no se ve

## ✅ Verificación Rápida

Después de descomprimir el ZIP, tu estructura DEBE verse así:

```
📁 portfolio-web/
│
├── 📄 index.html
├── 📄 proyectos.html
├── 📄 sobre-mi.html
├── 📄 contacto.html
├── 📄 experiencia.html
├── 📄 formacion.html
├── 📄 habilidades.html
├── 📄 competiciones.html
├── 📄 tecnologias.html
├── 📄 blog.html
├── 📄 recursos.html
├── 📄 sitemap.xml
├── 📄 README.md
├── 📄 CHECKLIST_REQUISITOS.md
│
└── 📁 css/
    ├── 📄 styles.css
    └── 📄 animations.css
```

## ❌ PROBLEMA COMÚN: Carpeta doble

Si al descomprimir ves esto:

```
📁 portfolio-web/
└── 📁 portfolio-web/     ← CARPETA DUPLICADA
    ├── 📄 index.html
    └── 📁 css/
```

### Solución:
1. Abre la carpeta `portfolio-web` externa
2. Copia TODO el contenido de `portfolio-web` interna
3. Pégalo en la carpeta externa
4. Elimina la carpeta interna vacía

## 🔍 Cómo verificar que está bien

1. **Abre la carpeta `portfolio-web`**
2. Debes ver directamente:
   - ✅ Los archivos `.html`
   - ✅ La carpeta `css`
   - ✅ NO otra carpeta `portfolio-web` dentro

3. **Abre la carpeta `css`**
4. Debes ver:
   - ✅ `styles.css` (archivo de ~150 KB)
   - ✅ `animations.css` (archivo de ~5 KB)

## 🧪 Probar que funciona

1. **Abre `index.html` haciendo doble clic**
2. **¿Se ve bonito con colores y diseño?** ✅ Está bien
3. **¿Solo ves texto sin formato?** ❌ Revisa la estructura de carpetas

## 🌐 Para GitHub Pages

Cuando subas a GitHub, asegúrate de que:

1. **La estructura en GitHub sea:**
   ```
   tu-repositorio/
   ├── index.html
   ├── proyectos.html
   ├── ...
   └── css/
       ├── styles.css
       └── animations.css
   ```

2. **NO debe haber una carpeta extra:**
   ```
   tu-repositorio/
   └── portfolio-web/    ← MAL, esto rompe las rutas
       ├── index.html
       └── css/
   ```

## 💡 Si subes con Git

Cuando uses `git add .`, asegúrate de estar DENTRO de la carpeta que contiene directamente los archivos `.html` y la carpeta `css`.

```bash
# CORRECTO
cd portfolio-web              # Entras a la carpeta
ls                            # Ves: index.html, css/, etc.
git init                      # Inicializas aquí
git add .

# INCORRECTO
cd carpeta-que-contiene-portfolio-web
git init                      # ¡Mal! Demasiado arriba
```

## 🆘 Si el CSS sigue sin funcionar

1. **Opción 1:** Vuelve a descomprimir el ZIP
2. **Opción 2:** Descárgame de nuevo y te creo una versión con rutas absolutas
3. **Opción 3:** Avísame y te ayudo a debuggear

## ✅ Checklist Final

- [ ] Carpeta `css` está al mismo nivel que `index.html`
- [ ] Dentro de `css` están `styles.css` y `animations.css`
- [ ] Al abrir `index.html` en navegador se ve con diseño
- [ ] En GitHub, los archivos están en la raíz del repositorio (no en una subcarpeta)
- [ ] GitHub Pages está activado en Settings → Pages
- [ ] URL de GitHub Pages: `https://TU-USUARIO.github.io/NOMBRE-REPO/`

## 📞 Contacto

Si necesitas ayuda, avísame con:
- Captura de pantalla de la estructura de carpetas
- Captura de cómo se ve en el navegador
- URL de tu repositorio de GitHub
