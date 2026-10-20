# 🚀 Angular + Bootstrap

Aplicación en Angular estructurada modularmente mediante componentes y navegación por rutas (`routerLink` y `router-outlet`). El proyecto cuenta con un componente `lista` para visualizar los alumnos registrados y un componente `agregar` con un formulario para incorporar nuevos estudiantes. El manejo del estado y la persistencia de datos compartida entre componentes se gestiona de manera centralizada en el archivo `store.ts`. La interfaz gráfica está estilizada utilizando las clases globales de Bootstrap.

---

## 📂 Estructura del Proyecto

```text
.
├── src/
│   ├── app/
│   │   ├── agregar/            # Componente formulario para registrar estudiantes
│   │   │   ├── agregar.css
│   │   │   ├── agregar.html
│   │   │   ├── agregar.spec.ts
│   │   │   └── agregar.ts
│   │   ├── lista/              # Componente para visualizar la tabla de estudiantes
│   │   │   ├── lista.css
│   │   │   ├── lista.html
│   │   │   ├── lista.spec.ts
│   │   │   └── lista.ts
│   │   ├── app.config.ts       # Configuración global de la aplicación
│   │   ├── app.css             # Estilos del componente principal
│   │   ├── app.html            # Plantilla con navegación y router-outlet
│   │   ├── app.routes.ts       # Definición de rutas (/lista y /agregar)
│   │   ├── app.spec.ts         # Pruebas unitarias
│   │   ├── app.ts              # Lógica del componente raíz
│   │   └── store.ts            # Estado centralizado / Store de datos
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

### 3. Generación de Componentes
Crear los componentes independientes para el formulario y el listado:
```bash
ng g c component
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