PetLog

Gestor de bitácora de mascotas desarrollado en Python para la materia Programación 1.

Temas a incluir:
- Matrices
- Tuplas
- Rebanado y Comprensión de listas
- Cadena de caracteres
- Diccionarios
- Conjuntos
- Funciones lambda , map, filter y reduce
- Excepciones
- Archivos
- Expresiones Regulares

Descripción:

PetLog es una aplicación de consola que permite llevar un registro completo de mascotas y sus dueñxs, incluyendo:
- Alta, baja y modificación de mascotas y dueñxs
- Registro de visitas médicas con historial
- Asociación entre mascotas y dueñxs
- Control de sesiones de usuario (login / registro)
- Persistencia de datos en archivos JSON (mascotas.json, duenios.json y usuariosRegistrados.json) y texto (logAuditoría.txt)

🚀 Características principales

Autenticación: Inicio de sesión y registro de usuarios.

Gestión de dueñxs: Agregar, eliminar, modificar y listar dueñxs.

Gestión de mascotas: Agregar, eliminar, modificar y listar mascotas.

Asociaciones: Vincular mascotas a dueñxs y viceversa.

Historial médico: Registrar visitas médicas con fecha, motivo, diagnóstico, tratamiento y veterinario responsable.

Menús interactivos en consola con validación de entradas.

Estructura de archivos
├── .github/workflows        # Configuración de acciones de GitHub
├── Archivos/
│   ├── Usuarios/
│   │   └── usuariosRegistrados.txt
├── core/                    # Módulo de procesamiento de lenguaje
├── cuestionarios/           # Archivos con preguntas/respuestas
├── documentos/              # Documentación del proyecto
├── logs/                    # Registro de interacciones
├── tests/                   # Casos de prueba
└── ui/                      # Interfaz de usuario (Textual)

PetLog/
├── Archivos/
│   ├── Usuarios/
│   │   └── usuariosRegistrados.txt
│   ├── Mascotas/
│   │   └── mascotas.json
│   └── Duenios/
│       └── duenios.json
├── PetLog_G.py            # Código principal
├── README.md             # Documentación del proyecto
└── .gitignore

⚙️ Instalación y uso

Clonar el repositorio

git clone https://github.com/tu-usuario/PetLog.git
cd PetLog

Crear entorno virtual (opcional pero recomendado)

python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate    # Windows

Instalar dependencias

Este proyecto solo usa la librería estándar de Python (no hay dependencias externas).

Ejecutar la aplicación

python PetLog_G.py

Primer arranque

Si no existen los archivos en Archivos/, se crearán vacíos.

Crear un usuario para iniciar sesión.

Comenzar a gestionar mascotas y dueñxs.

📋 Funcionalidades detalladas

Menú principal: Navegación por opciones numeradas.

Validaciones: Verificación de IDs, formatos de email, campos no vacíos.

Persistencia: Lectura/escritura atómica de archivos con json.dump y bloques with open(...).

Historial: Cada visita médica es una lista de cadenas con etiquetas y nombre del veterinario.

