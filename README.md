# 🚀 Angular + Bootstrap

Aplicación en Angular que realiza peticiones HTTP a una API pública de imágenes de perros. El proyecto cuenta con un componente `perro` y un servicio dedicado (`perro.service.ts`) que solicita un lote de 6 imágenes aleatorias mediante un endpoint parametrizado. La interfaz incluye un botón interactivo que vuelve a consultar la API en tiempo real para refrescar las imágenes de la pantalla, maquetadas dentro de una cuadrícula de tarjetas de Bootstrap.

---

## 📂 Estructura del Proyecto

```text
.
├── src/
│   ├── app/
│   │   ├── perro/               # Componente para la galería de imágenes
│   │   │   ├── perro.css
│   │   │   ├── perro.html       # Plantilla con el botón de refresco y tarjetas
│   │   │   ├── perro.service.ts # Servicio HTTP para consumir la API pública
│   │   │   ├── perro.spec.ts
│   │   │   └── perro.ts         # Lógica del componente y llamada a la API
│   │   ├── app.config.ts        # Configuración global de la aplicación (HttpClient)
│   │   ├── app.css             # Estilos del componente principal
│   │   ├── app.html            # Plantilla raíz con el componente perro
│   │   ├── app.routes.ts       # Definición de rutas
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
ng proyecto
cd proyecto
```

---

### 3. Generación del Componente y Servicio
Crear el componente y el servicio dentro de la carpeta del componente:
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