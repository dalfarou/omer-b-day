# Feliz Cumpleaños Omer 🎂

Página interactiva de cumpleaños con pastel animado, velitas que se soplan, confeti, globos y Las Mañanitas como música de fondo.

## Archivos

- `index.html` — la página completa (sin dependencias externas)
- `las-mananitas.mp3` — música de fondo (Alejandro Fernández — Las Mañanitas)

Los dos archivos deben subirse juntos al mismo directorio.

## Probar localmente

Solo abre `index.html` en tu navegador haciendo doble clic. También puedes servirla:

```bash
python3 -m http.server 8080
```

y luego abrir http://localhost:8080

## Desplegar en Vercel (recomendado — más rápido)

**Opción A: arrastrar y soltar**

1. Entra a https://vercel.com y crea una cuenta gratis
2. Clic en "Add New..." → "Project"
3. Arrastra la carpeta que contiene `index.html` al área de carga
4. Clic en "Deploy" — listo en ~30 segundos
5. Recibirás una URL tipo `https://feliz-cumpleanos-omer.vercel.app`

**Opción B: Vercel CLI**

```bash
npm i -g vercel
cd carpeta-del-proyecto
vercel
```

## Desplegar en GitHub Pages

1. Crea un repo nuevo en GitHub (ej. `cumpleanos-omer`)
2. Sube el archivo `index.html`:
   ```bash
   git init
   git add index.html
   git commit -m "Feliz cumpleaños Omer"
   git branch -M main
   git remote add origin https://github.com/tu-usuario/cumpleanos-omer.git
   git push -u origin main
   ```
3. En el repo: Settings → Pages → Source: `main` branch, carpeta `/ (root)` → Save
4. Espera 1–2 minutos y accede a `https://tu-usuario.github.io/cumpleanos-omer/`

## Notas

- La música se reproduce al tocar **"Toca para comenzar"** (los navegadores bloquean autoplay hasta que hay interacción del usuario)
- El audio es `las-mananitas.mp3` (Alejandro Fernández) reproducido en loop automático
- Hay un botón 🔊 en la esquina superior derecha para silenciar/activar
- Haz clic en cada vela para apagarla, o usa el botón "Soplar las velitas" para todas
