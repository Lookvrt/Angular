# 🚀 Angular + Bootstrap

Aplicación en Angular modularizada mediante componentes (`agregar` y `lista`), navegación por rutas y consumo de datos desvinculado a través de un servicio (`estudiante.service.ts`). A diferencia de manejar el estado local o en un archivo estático, esta arquitectura implementa un servicio inyectable que simula las peticiones HTTP a una API REST leyendo los datos iniciales desde un archivo local `estudiante.json`. La interfaz se encuentra maquetada con estilos y componentes de Bootstrap.

---

## 📂 Estructura del Proyecto

```text
.
├── public/
│   └── estudiante.json         # Mock API local con datos iniciales en formato JSON
├── src/
│   ├── app/
│   │   ├── agregar/            # Componente formulario para registrar estudiantes
│   │   │   ├── agregar.css
│   │   │   ├── agregar.html
│   │   │   ├── agregar.spec.ts
│   │   │   └── agregar.ts
│   │   ├── estudiante/         # Servicio inyectable para la gestión de datos
│   │   │   └── estudiante.service.ts
│   │   ├── lista/              # Componente para listar y visualizar estudiantes
│   │   │   ├── lista.css
│   │   │   ├── lista.html
│   │   │   ├── lista.spec.ts
│   │   │   └── lista.ts
│   │   ├── app.config.ts       # Configuración global de la aplicación
│   │   ├── app.css             # Estilos del componente principal
│   │   ├── app.html            # Plantilla con menú de navegación y router-outlet
│   │   ├── app.routes.ts       # Definición de rutas (/lista y /agregar)
│   │   ├── app.spec.ts         # Pruebas unitarias
│   │   └── app.ts              # Componente raíz
│   ├── index.html              # Archivo HTML raíz
│   ├── main.ts                 # Punto de entrada de la aplicación
│   └── styles.css              # Importación global de Bootstrap
├── angular.json                # Configuración del workspace de Angular
├── package.json                # Dependencias del proyecto
├── tsconfig.json               # Configuración de TypeScript
└── README.md
```

---

## ⚙️ Configuración del Entorno

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

### 3. Generación del Servicio y Componentes
Crear el servicio inyectable dentro de su respectiva carpeta y los componentes independientes:
```bash
ng g c component
```

---

### 4. Creación de la Mock API Local
Crear el archivo `datos.json` dentro del directorio `public/` para simular la fuente de datos externa.

---

### 5. Instalación e Importación de Bootstrap
Dentro del directorio del proyecto, instalar la librería de Bootstrap:
```bash
npm install bootstrap
```

Añadir la importación al inicio del archivo `src/styles.css`:
```css
@import "bootstrap/dist/css/bootstrap.min.css";
```

---

### 6. Ejecución del Servidor Local
Iniciar el servidor de desarrollo local:
```bash
ng serve
```
*(Ejecutar `ng serve -o` para abrir automáticamente la pestaña en el navegador).*