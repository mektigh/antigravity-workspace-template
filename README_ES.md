# 🪐 Plantilla de Espacio de Trabajo Google Antigravity (Edición Empresarial)

![License](https://img.shields.io/badge/License-MIT-green)
![LangChain](https://img.shields.io/badge/LangChain-%F0%9F%9A%AB_Free-red)
```mermaid
sequenceDiagram
    participant User
    participant Agent as 🤖 GeminiAgent
    participant Memory as 🧠 Memory
    participant Tools as 🛠️ Tools
    participant Artifacts as 📂 Artifacts

    User->>Agent: "Refactorizar Autenticación"
    activate Agent
    
    Agent->>Artifacts: Crear Plan de Implementación
    
    Note over Agent: <thought> Proceso de Pensamiento Profundo </thought>
    Agent->>Agent: Formular Estrategia
    
    Agent->>Tools: Ejecutar Herramienta (code_edit)
    activate Tools
    Tools-->>Agent: Resultado
    deactivate Tools
    
    Agent->>Artifacts: Guardar Registros/Evidencia
    
    Agent-->>User: Informe Final (Walkthrough)
    deactivate Agent
```

## 🔥 Funciones Asesinas

- 🧠 **Motor de Memoria Infinita**: La resumición recursiva comprime el historial automáticamente; los límites de contexto dejan de ser un problema.
- 🛠️ **Protocolo Universal de Herramientas**: Patrón ReAct genérico. Registra cualquier función de Python en `available_tools` y el Agente sabrá usarla.
- ⚡️ **Nativo de Gemini**: Optimizado para la velocidad y las llamadas a funciones de Gemini 2.0 Flash.

## 🚀 Inicio Rápido

### Desarrollo Local
1. **Instalar dependencias**:
    ```bash
    pip install -r requirements.txt
    ```
2. **Ejecutar el Agente**:
    ```bash
    python src/agent.py
    ```

### Despliegue con Docker
1. **Construir y ejecutar**:
    ```bash
    docker-compose up --build
    ```

## 📂 Estructura del Proyecto

```
.
├── .antigravity/       # 🛸 Configuración Oficial de Antigravity
│  └── rules.md        # Reglas y Permisos del Agente
├── artifacts/          # 📂 Salidas del Agente (Planes, Registros, Visuales)
├── .context/           # Base de Conocimiento de IA
├── .github/            # Flujos de Trabajo CI/CD
├── src/                # Código Fuente
│  ├── agent.py        # Lógica Principal del Agente
│  ├── config.py       # Gestión de Configuraciones
│  ├── memory.py       # Gestor de Memoria JSON
│  └── tools/          # Herramientas del Agente
├── tests/              # Suite de Pruebas
├── .cursorrules        # Puntero de Compatibilidad
├── Dockerfile          # Construcción de Producción
├── docker-compose.yml  # Configuración de Desarrollo Local
└── mission.md          # Objetivo del Agente
```

## 🚀 Flujo de Trabajo “Cero-Configuración”

Deja de escribir largos prompts del sistema. Este espacio de trabajo precarga la arquitectura cognitiva de la IA por ti.

### Paso 1: Clonar y Renombrar (El “Molde”)
Trata este repositorio como un molde de fábrica. Clónalo y renombra la carpeta con el nombre de tu proyecto.
```bash
git clone https://github.com/study8677/antigravity-workspace-template.git my-agent-project
cd my-agent-project
# Ahora estás listo. No se requiere configuración.
```

### Paso 2: El Momento Mágico ⚡️
Abre la carpeta en Cursor o Google Antigravity.
- 👀 **Observa**: El IDE detecta automáticamente `.cursorrules`.
- 🧠 **Carga**: La IA ingiere silenciosamente la personalidad “Experto en Antigravity” desde `.antigravity/rules.md`.

### Paso 3: Solo Pregunta (Sin Instrucciones Extras)
No necesitas decirle a la IA que “tenga cuidado” o “use la carpeta src”. Ya está programada para ser un Ingeniero Senior.

**Forma Antigua (Prompting Manual)**:
> “Por favor escribe un juego de la serpiente. Asegúrate de usar código modular. Pon los archivos en src. No olvides los comentarios…”

**La Forma Antigravity**:
> “Construye un juego de la serpiente.”

La IA automáticamente:
1. 🛑 **Pausa**: “Según los protocolos, debo planificar primero.”
2. 📄 **Documenta**: Genera `artifacts/plan_snake.md`.
3. 🔨 **Construye**: Escribe código modular en `src/game/` con docstrings completos estilo Google.

## 🗺️ Hoja de Ruta

- [x] **Fase 1: Fundación** (Andamiaje, Configuración, Memoria)
- [x] **Fase 2: DevOps** (Docker, CI/CD)
- [x] **Fase 3: Cumplimiento Antigravity** (Reglas, Artefactos)
- [x] **Fase 4: Memoria Avanzada** (Buffer de Resumen Implementado ✅)
- [x] **Fase 5: Arquitectura Cognitiva** (Despacho Genérico de Herramientas Implementado ✅)
## 👥 Colaboradores

Un agradecimiento especial a los miembros de la comunidad que han contribuido a este proyecto:

- [@devalexanderdaza](https://github.com/devalexanderdaza) 💻 **(¡Primer Colaborador!)**
  - Implementó scripts de herramientas de demostración y mejoró la funcionalidad del agente.

**¿Quieres contribuir?** ¡Revisa nuestra página de [Issues](https://github.com/study8677/antigravity-workspace-template/issues)!
## 💡 Llamada a Ideas: Protocolo Swarm

¡Valoramos las **ideas** tanto como el código!
Actualmente estamos ideando la arquitectura para la **Fase 6: Swarm Multi-Agente**. Si proporcionas una sugerencia arquitectónica sólida o un diseño detallado que sea adoptado, **serás añadido a nuestro README como Colaborador**.

No dudes en compartir tus pensamientos en los [Issues](https://github.com/study8677/antigravity-workspace-template/issues), incluso si no tienes tiempo para escribir la implementación.