# 🚀 Angular + Bootstrap

Aplicación en Angular para la consulta de detalles de estudiantes mediante navegación con rutas parametrizadas (`detalle/:id`). La interfaz inicia en la vista del componente `estudiantes`, donde se despliega la lista general. El servicio inyectable (`estudiante.service.ts`) gestiona la obtención del listado completo y la búsqueda específica por ID. Al navegar al componente `detalle`, se captura el parámetro dinámico de la URL para cargar la información del alumno. La interfaz está maquetada con componentes y estilos de Bootstrap.

---

## 📂 Estructura del Proyecto

```text
.
├── src/
│   ├── app/
│   │   ├── detalle/                       # Componente para visualizar la información detallada del alumno
│   │   │   ├── detalle.css
│   │   │   ├── detalle.html               # Plantilla con el expediente 
│   │   │   ├── detalle.spec.ts
│   │   │   └── detalle.ts                 # Captura de parámetros de ruta (ActivatedRoute) y consulta por ID
│   │   ├── services/                    # Servicio para la gestión y consulta de estudiantes
│   │   │   ├── estudiante.service.ts       # Métodos para obtener estudiantes
│   │   │   └── estudiante.service.spec.ts
│   │   ├── estudiantes/                    # Componente para el listado general
│   │   │   ├── estudiantes.css
│   │   │   ├── estudiantes.html           # Tabla principal
│   │   │   ├── estudiantes.spec.ts
│   │   │   └── estudiantes.ts             # Carga inicial del listado completo
│   │   ├── app.config.ts                  # Configuración global de la aplicación
│   │   ├── app.css                        # Estilos del componente raíz
│   │   ├── app.html                       # Plantilla raíz con router-outlet
│   │   ├── app.routes.ts                  # Mapeo de rutas ('estudiantes' y 'detalle/:id')
│   │   ├── app.spec.ts                    # Pruebas unitarias
│   │   └── app.ts                         # Componente raíz
│   ├── index.html                         # Archivo HTML raíz
│   ├── main.ts                            # Punto de entrada de la aplicación
│   └── styles.css                         # Importación global de Bootstrap
├── angular.json                           # Configuración del workspace de Angular
├── package.json                           # Dependencias del proyecto
├── tsconfig.json                          # Configuración de TypeScript
└── README.md
```

---

## ⚙️ Configuración del Entorno

---

### 1. Instalación Global de Angular CLI
Para disponer de las herramientas de comandos `ng` de forma global:
```bash
npm install -g @angular/cli
```

---

### 2. Creación del Proyecto e Ingreso al Directorio
Generar la estructura base de la aplicación e ingresar a la carpeta creada:
```bash
ng new proyecto
cd proyecto
```

---

### 3. Generación de Componentes y Servicio
Crear los componentes para el listado, la vista detallada y el servicio inyectable:
```bash
ng g c component
ng g s services/services.service
```

---

### 4. Instalación e Importación de Bootstrap
Dentro del directorio del proyecto, instalar la librería de Bootstrap:
```bash
npm install bootstrap
```

Añadir la importación al inicio del archivo `src/styles.css`:
```css
@import "bootstrap/dist/css/bootstrap.min.css";
```

---

### 5. Ejecución del Servidor Local
Iniciar el servidor de desarrollo local:
```bash
ng serve
```
*(Ejecutar `ng serve -o` para abrir automáticamente la pestaña en el navegador).*