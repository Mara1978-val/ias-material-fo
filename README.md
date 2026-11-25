# IAs para crear material docente (FO)

Guía interactiva para profesoras y profesores de **Formación Ocupacional**: qué inteligencias artificiales
usar para crear **presentaciones**, **páginas web dinámicas** y **material en GitHub**, con la instalación
y configuración paso a paso en **PowerShell**.

## Contenido de la guía

| Sección | Qué encontrarás |
|---|---|
| 1. Qué IA para cada tarea | Tabla resumen por tipo de material |
| 2. Agentes de código | OpenCode, Kiro (AWS), Antigravity (Google), Claude Code y Gemini CLI: instalación + configuración en PowerShell |
| 3. OmniRouter | Un router local que unifica varios modelos tras una sola clave (`Godde3s/omnirouter`) |
| 4. GitHub | GitHub CLI (`gh`), creación de repositorios y publicación con GitHub Pages |
| 5. Presentaciones y web | Gamma, Canva Magic Design, v0, Bolt y Lovable (sin instalar) |
| 6. FreeBuf | Aclaración: es un portal de ciberseguridad, no una IA de creación de material |
| 7. Flujo de trabajo | Ejemplo completo de la idea a la web pública |
| 8. Problemas frecuentes | Soluciones a errores típicos de PowerShell |

## Cómo verla

1. **En local:** abre `index.html` con doble clic (no necesita servidor ni Internet salvo para los enlaces).
2. **En GitHub Pages:** tras activar Pages (sección 4 de la guía) estará en
   `https://Mara1978-val.github.io/ias-material-fo/`

## Comandos rápidos (PowerShell)

```powershell
# Prerrequisitos
winget install Git.Git
winget install OpenJS.NodeJS.LTS
winget install GitHub.cli

# Agentes
npm install -g @opencode/cli        # OpenCode
irm 'https://cli.kiro.dev/install.ps1' | iex   # Kiro CLI (Windows 11)
irm https://antigravity.google/cli/install.ps1 | iex  # Antigravity CLI

# GitHub
gh auth login
gh repo create ias-material-fo --public --source . --push
```

## Fuentes

Toda la información de instalación procede de la documentación oficial (noviembre 2026):

- <https://opencode.ai/docs/>
- <https://kiro.dev/docs/getting-started/installation>
- <https://antigravity.google/docs/getting-started>
- <https://github.com/Godde3s/omnirouter>
- <https://docs.github.com/en/cli>
