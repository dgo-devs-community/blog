# Configurar Node.js y Frontend

## 🚀 Node.js Installation

### Descargar e Instalar

- **Sitio oficial**: [nodejs.org](https://nodejs.org/)
- **Versión recomendada**: LTS (Long Term Support)

### Verificar instalación

```bash
node --version
npm --version
```

---

## 📦 Gestores de Paquetes

### npm (incluido con Node.js)

```bash
# Instalar dependencias
npm install

# Instalar paquete específico
npm install nombre-paquete

# Instalar globalmente
npm install -g nombre-paquete
```

### Yarn (alternativa a npm)

```bash
# Instalar Yarn
npm install -g yarn

# Usar Yarn
yarn install
yarn add nombre-paquete
```

---

## ⚛️ Frameworks Frontend Populares

### React

```bash
# Crear nuevo proyecto React
npx create-react-app mi-proyecto
cd mi-proyecto
npm start
```

### Vue.js

```bash
# Instalar Vue CLI
npm install -g @vue/cli

# Crear proyecto
vue create mi-proyecto
```

### Vite (Build Tool Moderno)

```bash
# Crear proyecto con Vite
npm create vite@latest mi-proyecto
cd mi-proyecto
npm install
npm run dev
```

---

## 🔧 Herramientas de Desarrollo

### Prettier (Formateo de código)

```bash
npm install --save-dev prettier
```

### ESLint (Linting)

```bash
npm install --save-dev eslint
npx eslint --init
```

---

## 🌍 Variables de Entorno

### Archivo .env

```bash
# .env
REACT_APP_API_URL=http://localhost:3000
VITE_API_URL=http://localhost:3000
```

### Uso en código

```javascript
// React
const apiUrl = process.env.REACT_APP_API_URL

// Vite
const apiUrl = import.meta.env.VITE_API_URL
```

---

## ✅ Verificar Setup

Crea un proyecto de prueba:

```bash
npx create-react-app test-setup
cd test-setup
npm start
```

Si se abre en `http://localhost:3000`, ¡todo está listo!

---

➡️ Siguiente: [[Configurar Herramientas de Testing]]
