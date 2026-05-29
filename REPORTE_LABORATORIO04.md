# REPORTE DE LABORATORIO 04

**Curso:** Control de Versiones para Desarrollo Full Stack
**Docente:** Ing. Luis Flores

---

## 1. Identificación del Equipo Ágil

**Grupo de Trabajo N°:** 

**Integrantes de Ingeniería:**

* **[DESARROLLADOR 1] (Líder):** Keyling Jaritza Sanchez Vivas | GitHub: keylings766
* **[DESARROLLADOR 2] (Colaborador):** Alexander Aguilar Vanegas | GitHub: Alex-SQLNIC

---

## 2. Hito 1: Implementación de Seguridad Perimetral (.gitignore)

### 1. Estructura del archivo `.gitignore` consolidada:

```text
# Secretos locales de ApexPay
.env
.env.local

# Temporales de compilacion y dependencias generadas por el script
node_modules/
dist/
*.log
```

### 2. Prueba de Inmunidad de Credenciales

```text
$ git status

On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

---

## 3. Hito 2: Resolución de la Colisión de Interfaces (Merge Conflict)

### 1. Discrepancia Técnica Inicial

**Respuesta:**
El rechazo ocurrió porque el Desarrollador 2 intentó realizar un `git push` sobre una versión desactualizada de la rama `main`. Git detectó diferencias entre el repositorio local y remoto e inyectó marcadores de conflicto en el archivo `README.md` utilizando las etiquetas `<<<<<<<`, `=======` y `>>>>>>>`.

### 2. Resultado Consolidado de Consenso

```markdown
# ApexPay Dashboard

Tema del proyecto: Híbrido
```

---

## 4. Hito 3: Mitigación de Exposición de Infraestructura (`git revert`)

### 1. Histórico del Historial Clínico de Producción (Git Log)

```text
cab7699 Revert "feat: modulo de pruebas de red expuestas"
619a175 feat: modulo de pruebas de red expuestas
c72cbdd merge: conciliar conflicto de temas
f9839cf feat: configurar tema oscuro
```

### 2. Análisis de Resiliencia Organizacional

**Respuesta:**
El comando `git reset --hard` se considera peligroso en ramas públicas porque modifica y reescribe el historial compartido del repositorio. Si se utiliza después de realizar un `git push`, los demás integrantes del equipo quedarían desincronizados y podrían perder cambios importantes, generando conflictos graves en el flujo colaborativo.

Por otro lado, `git revert` crea un nuevo commit que deshace los cambios de un commit anterior sin eliminar el historial existente. Esto permite mantener la trazabilidad de los errores, conservar evidencia de las modificaciones realizadas y garantizar la estabilidad del trabajo colaborativo dentro del equipo de desarrollo.

---

## 5. Hito 4: Enlaces de Gobernanza y Solicitudes de Integración

* **Pull Request de Menú (`feat/menu-principal`):**
  `https://github.com/keylings766/apexpay-dashboard/compare/main...feat/menu-principal `

* **Pull Request de Footer (`feat/footer`):**
  `https://github.com/keylings766/apexpay-dashboard/compare/main...feat/footer`
