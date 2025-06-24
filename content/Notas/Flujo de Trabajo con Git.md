# Flujo de Trabajo con Git

## 🔄 Flujo Básico en Obreros Tech

### 1. Clonar el repositorio del proyecto

```bash
git clone git@github.com:usuario/proyecto.git
cd proyecto
```

### 2. Crear rama para tu tarea

```bash
# Crear y cambiar a nueva rama
git checkout -b feature/mi-nueva-funcionalidad

# O usar el comando más nuevo
git switch -c feature/mi-nueva-funcionalidad
```

### 3. Trabajar en tu código

```bash
# Ver cambios
git status

# Agregar archivos específicos
git add archivo.js

# O agregar todos los cambios
git add .
```

### 4. Hacer commit

```bash
# Commit con mensaje descriptivo
git commit -m "feat: agregar función de login de usuario"
```

### 5. Subir cambios

```bash
# Primera vez
git push -u origin feature/mi-nueva-funcionalidad

# Siguientes veces
git push
```

---

## 📝 Convenciones de Mensajes

### Formato recomendado

```
tipo: descripción breve

Descripción más detallada si es necesario
```

### Tipos comunes

- `feat`: Nueva funcionalidad
- `fix`: Corrección de bug
- `docs`: Cambios en documentación
- `style`: Formateo, espacios, etc.
- `refactor`: Refactorización de código
- `test`: Agregar o modificar tests

### Ejemplos

```bash
git commit -m "feat: agregar validación de email en formulario"
git commit -m "fix: corregir error de cálculo en total"
git commit -m "docs: actualizar README con instrucciones"
```

---

## 🔀 Trabajar con Ramas

### Comandos útiles

```bash
# Ver todas las ramas
git branch -a

# Cambiar de rama
git checkout nombre-rama
# o
git switch nombre-rama

# Actualizar rama desde main
git checkout main
git pull origin main
git checkout mi-rama
git merge main
```

### Pull Requests

1. Sube tu rama a GitHub
2. Ve al repositorio en GitHub
3. Click "Compare & pull request"
4. Describe tus cambios
5. Asigna reviewers si es necesario

---

## 🛠️ Comandos de Rescate

### Deshacer último commit (mantener cambios)

```bash
git reset --soft HEAD~1
```

### Deshacer cambios no commitados

```bash
git checkout -- archivo.js
# o deshacer todo
git checkout -- .
```

### Ver historial

```bash
git log --oneline
git log --graph --oneline --all
```

### Stash (guardar cambios temporalmente)

```bash
# Guardar cambios
git stash

# Ver stash
git stash list

# Recuperar cambios
git stash pop
```

---

## ⚠️ Mejores Prácticas

1. **Commits pequeños y frecuentes**
2. **Mensajes descriptivos**
3. **Actualizar rama antes de hacer PR**
4. **No hacer push directo a main**
5. **Revisar cambios antes de commit**

---

➡️ Siguiente: [[Apps de Productividad para Desarrollo]]
