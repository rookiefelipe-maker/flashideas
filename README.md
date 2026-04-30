# FlashIdeas ⚡

> Captura ideas accionables. Actúa o las pierdes.

## ¿Qué hace?

- **Modal inmediato** al abrir la app — cero fricción para capturar
- **24h de vida** por idea con barra de progreso en tiempo real
- **✓ Trabajé en esto** — marca la idea como accionada y desaparece
- **Auto-eliminación** a las 24h si no la checas
- **Etiquetas** — Idea, Proyecto, Personal, Trabajo, Otro
- **Backlinks `[[`** — enlaza notas entre sí, ve conexiones en panel lateral
- **Buscador** tipo Spotlight en la barra inferior
- **Exportar `.md`** por nota
- **PWA** — instálala en tu móvil desde el navegador

---

## Deploy en GitHub Pages

### 1. Crea el repositorio

```bash
git init
git add .
git commit -m "feat: FlashIdeas PWA"
```

### 2. Súbelo a GitHub

```bash
gh repo create flashideas --public --push --source=.
```

O manualmente: crea el repo en github.com y luego:

```bash
git remote add origin https://github.com/TU_USUARIO/flashideas.git
git branch -M main
git push -u origin main
```

### 3. Activa GitHub Pages

1. Ve a tu repo → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `/ (root)`
4. Guarda — en ~1 min estará en:

```
https://TU_USUARIO.github.io/flashideas/
```

### 4. Instala como PWA en tu móvil

- **iPhone (Safari):** Abre la URL → botón compartir → "Agregar a pantalla de inicio"
- **Android (Chrome):** Abre la URL → menú → "Instalar app"

---

## Estructura

```
flashideas/
├── index.html      ← App completa (HTML + CSS + JS)
├── manifest.json   ← Config PWA
├── sw.js           ← Service Worker (offline)
├── icon-192.png    ← Ícono PWA
├── icon-512.png    ← Ícono PWA grande
└── README.md
```

## Datos

Todo se guarda en `localStorage` del navegador. No hay servidor ni cuenta necesaria.
