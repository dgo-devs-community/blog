# 🧱 Infraestructura - Landing Page DgoTecHub

## 📦 Repositorio

- **GitHub:** [github.com/DgoTecHub/landing-page](https://github.com/DgoTecHub/landing-page)
- **Owner:** Comunidad DgoTecHub
- **Privado/Público:** Público (para atraer colaboradores)
- **Branch principal:** `main`
- **Convención de ramas:** `feature/*`, `fix/*`, `docs/*`

---

## ☁️ Hosting / Deploy

- **Proveedor:** Vercel
- **URL de producción:** [https://dgotechub.com](https://dgotechub.com)
- **URL de preview por pull request:** Automático vía Vercel

---

## 🔁 Integraciones CI/CD

- **Vercel GitHub Integration:** activa
- **Build automático:** sí, en cada push a `main` y PR
- **Previews:** sí, por cada rama

---

## 🌱 Ambientes

| Ambiente   | URL                                      | Branch         |
| ---------- | ---------------------------------------- | -------------- |
| Producción | https://dgotechub.com                    | `main`         |
| Preview    | https://landing-git-feature-x.vercel.app | `feature/*`    |
| Local      | `localhost:3000`                         | cualquier rama |

---

## 🔑 Variables de entorno

> 🛡️ Solo necesarias si se integra con CMS, forms externos o APIs

| Variable              | Descripción                        | Ambiente     |
| --------------------- | ---------------------------------- | ------------ |
| `NEXT_PUBLIC_API_URL` | Enlace a API de eventos (opcional) | preview/prod |
| `DISCORD_INVITE`      | Link directo a Discord             | todos        |

---

## 🧪 Tests

- **Tipo:** Manual (por ahora)
- **Automatización futura:** Cypress o Playwright

---

## 🧭 Enlaces relacionados

- [[Proyecto Landing Page DgoTecHub]]
- [Figma diseño](https://www.figma.com/file/XXXX)
- [Panel Vercel](https://vercel.com/dgotechub/landing-page)
