# Páginas de cumpleaños interactivas 🎂⚾⚽🏀

Tres páginas independientes con pastel animado, confeti, música de fondo (Las Mañanitas) y velitas que se apagan al tocarlas.

## Archivos

- `index.html` — versión clásica para **Omer** (paleta morado/rosa, globos, cielo estrellado)
- `sandy.html` — versión beisbol para **Sandy** (Dodger blue, jersey #17 de Ohtani, scoreboard, ¡HOME RUN!)
- `niv.html` — versión doble para **Niv** (Manchester United ✕ Miami Heat, jerseys #7 y #3, estadio genérico, ¡GOOOOL Y SWISH!)
- `las-mananitas.mp3` — música compartida por las tres páginas

Todos los archivos deben subirse al mismo directorio.

## Probar localmente

```bash
python3 -m http.server 8080
```

- Página de Omer: http://localhost:8080/index.html
- Página de Sandy: http://localhost:8080/sandy.html
- Página de Niv:   http://localhost:8080/niv.html

## Desplegar en Vercel (recomendado — más rápido)

1. Entra a https://vercel.com y crea una cuenta gratis
2. Clic en "Add New..." → "Project"
3. Arrastra la carpeta `outputs` completa al área de carga
4. Clic en "Deploy" — listo en ~30 segundos
5. Recibirás una URL tipo `https://cumpleanos.vercel.app`. Las páginas estarán en:
   - `https://cumpleanos.vercel.app/` (Omer, por defecto)
   - `https://cumpleanos.vercel.app/sandy.html` (Sandy)
   - `https://cumpleanos.vercel.app/niv.html` (Niv)

**Opción CLI:**

```bash
npm i -g vercel
cd carpeta-del-proyecto
vercel
```

## Desplegar en GitHub Pages

1. Crea un repo nuevo en GitHub (ej. `cumpleanos`)
2. Sube los archivos:
   ```bash
   git init
   git add index.html sandy.html niv.html las-mananitas.mp3
   git commit -m "Páginas de cumpleaños"
   git branch -M main
   git remote add origin https://github.com/tu-usuario/cumpleanos.git
   git push -u origin main
   ```
3. En el repo: Settings → Pages → Source: `main` branch, carpeta `/ (root)` → Save
4. Espera 1–2 minutos y entra a:
   - `https://tu-usuario.github.io/cumpleanos/` (Omer)
   - `https://tu-usuario.github.io/cumpleanos/sandy.html` (Sandy)
   - `https://tu-usuario.github.io/cumpleanos/niv.html` (Niv)

## Notas

- La música se reproduce al tocar el botón inicial (los navegadores bloquean autoplay hasta que hay interacción del usuario)
- El audio es `las-mananitas.mp3` (Alejandro Fernández) reproducido en loop
- Hay un botón 🔊 en la esquina superior derecha para silenciar/activar
- Haz clic en cada vela para apagarla, o usa el botón principal para apagarlas todas
- En la página de Sandy, cada vela apagada lanza una pelota de beisbol al cielo y al final aparece "¡HOME RUN!" con confeti en colores de los Dodgers
- En la página de Niv, cada vela alterna lanzando ⚽ y 🏀 al cielo, con confeti en rojo MUFC + negro/dorado Heat y final "¡GOOOOL Y SWISH!"
