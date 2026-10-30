# Controlador de Dron + Simulador

Proyecto con dos partes:

| Carpeta | Herramienta | Descripción |
|---|---|---|
| `firmware/` | PlatformIO (Arduino Uno) | Código del controlador del dron |
| `simulador/SimuladorDronUI/` | Processing 4 | Interfaz/simulador en PC |

## Estructura

```
.
├── platformio.ini          # Config PlatformIO (apunta a firmware/)
├── firmware/
│   ├── include/            # Headers (.h)
│   ├── src/                # main.cpp y fuentes
│   ├── lib/                # Librerías privadas
│   └── test/               # Tests unitarios
└── simulador/
    └── SimuladorDronUI/
        └── SimuladorDronUI.pde
```

## Uso en VS Code

Extensiones recomendadas (VS Code las sugiere al abrir la carpeta):
PlatformIO IDE, Processing, GitHub Pull Requests.

Tareas (`Ctrl+Shift+P` → *Tasks: Run Task*):

- **Firmware: Compilar** (`Ctrl+Shift+B`)
- **Firmware: Subir al Arduino**
- **Firmware: Monitor serie**
- **Simulador: Ejecutar (Processing)**
- **Simulador: Abrir en Processing IDE**

También funcionan los botones de la barra de PlatformIO y el botón ▶ de la extensión Processing al abrir el `.pde`.
