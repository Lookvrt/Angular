# 🚀 Angular + Bootstrap

Aplicación en Angular para el listado y filtrado dinámico de un catálogo de productos obtenido desde una API REST externa. La arquitectura utiliza un servicio inyectable (`producto.service.ts`) que gestiona las peticiones `HTTP GET`. En el componente `productos`, se implementa la lógica de filtrado dinámico para la búsqueda de productos por nombre y la segmentación por stock insuficiente, presentando los datos mediante tarjetas y tablas estilizadas con Bootstrap.

---

## 📂 Estructura del Proyecto

```text
.
├── src/
│   ├── app/
│   │   ├── productos/                  # Componente para el catálogo de productos
│   │   │   ├── productos.css
│   │   │   ├── productos.html          # Plantilla con campo de búsqueda, filtros y tarjetas
│   │   │   ├── productos.spec.ts
│   │   │   └── productos.ts            # Lógica de filtrado por nombre y stock insuficiente
│   │   ├── services/                   # Servicio de integración con la API
│   │   │   ├── producto.service.ts      # Servicio HTTP con peticiones GET y Observables
│   │   │   └── producto.service.spec.ts
│   │   ├── app.config.ts                # Configuración global (proveedor HttpClient)
│   │   ├── app.css                     # Estilos del componente raíz
│   │   ├── app.html                    # Plantilla raíz
│   │   ├── app.routes.ts               # Definición de rutas
│   │   ├── app.spec.ts                 # Pruebas unitarias
│   │   └── app.ts                      # Componente raíz
│   ├── index.html                      # Archivo HTML raíz
│   ├── main.ts                         # Punto de entrada de la aplicación
│   └── styles.css                      # Importación global de Bootstrap
├── angular.json                        # Configuración del workspace de Angular
├── package.json                        # Dependencias del proyecto
├── tsconfig.json                       # Configuración de TypeScript
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

### 3. Generación del Componente y Servicio
Crear el componente y el servicio inyectable:
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