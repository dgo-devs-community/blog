# Configurar Git y GitHub

## 🌐 Instalación de Git

### Por Sistema Operativo

- **Windows**: [Git for Windows](https://gitforwindows.org/)
- **Mac**: `brew install git` o desde [git-scm.com](https://git-scm.com/)
- **Linux**: `sudo apt install git`

### Verificar instalación

```bash
git --version
```

---

## ⚙️ Configuración Inicial

### Configurar identidad

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

### Configuraciones útiles

```bash
# Configurar editor predeterminado
git config --global core.editor "code --wait"

# Configurar merge tool
git config --global merge.tool vscode
```

---

## 🔑 GitHub Setup

### 1. Crear cuenta

- Ve a [github.com](https://github.com) y crea tu cuenta
- Usa el mismo email que configuraste en Git

### 2. Configurar SSH Keys (Recomendado)

**Generar clave SSH**:

```bash
ssh-keygen -t ed25519 -C "tu@email.com"
```

**Agregar al agente SSH**:

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

**Copiar clave pública**:

```bash
cat ~/.ssh/id_ed25519.pub
```

**Agregar en GitHub**:

1. Ve a Settings > SSH and GPG keys
2. Click "New SSH key"
3. Pega tu clave pública

### 3. Verificar conexión

```bash
ssh -T git@github.com
```

---

## 📚 Comandos Básicos

```bash
# Clonar repositorio
git clone git@github.com:usuario/repositorio.git

# Ver estado
git status

# Agregar cambios
git add .

# Hacer commit
git commit -m "Descripción del cambio"

# Subir cambios
git push origin main

# Bajar cambios
git pull origin main
```

---

➡️ Siguiente: [[Flujo de Trabajo con Git]]
