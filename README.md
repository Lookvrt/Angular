# 🚀 Angular + Bootstrap

Esta aplicación simula un mini sistema de gestión académica enfocado en el manejo de arreglos de objetos, lógica de validación mediante métodos en el componente y renderizado de tablas responsivas con Bootstrap.

---

## 📂 Estructura del Proyecto

```text
.
├── src/
│   ├── app/
│   │   ├── app.config.ts       # Configuración global de la aplicación
│   │   ├── app.css             # Estilos específicos del componente principal
│   │   ├── app.html            # Plantilla HTML con la tabla y formularios
│   │   ├── app.routes.ts       # Configuración de rutas (no utilizadas en esta etapa)
│   │   ├── app.spec.ts         # Pruebas unitarias
│   │   └── app.ts              # Arreglo de estudiantes, métodos y lógica
│   ├── index.html              # Archivo HTML raíz
│   ├── main.ts                 # Punto de entrada de la aplicación
│   └── styles.css              # Importación global de Bootstrap
├── angular.json                # Configuración del workspace de Angular
├── package.json                # Dependencias del proyecto
├── tsconfig.json               # Configuración del compilador TypeScript
└── README.md
```

---

## ⚙️ Configuración del Entorno

Documentación completa de la instalación de Angular CLI + creación del proyecto.

### 1. Instalación Global de Angular CLI
Si aún no cuentas con el CLI de Angular instalado globalmente:

```bash
npm install -g @angular/cli
```

---

### 2. Creación del Proyecto e Ingreso al Directorio
Genera la estructura base de la aplicación y entra a la carpeta creada (paso obligatorio antes de instalar dependencias):

```bash
ng new mini-lms
cd mini-lms
```

---

### 3. Instalación e Importación de Bootstrap
Dentro de la carpeta del proyecto, instala Bootstrap:
```bash
npm install bootstrap
```

Abre el archivo `src/styles.css` e importa los estilos globales de Bootstrap al inicio del archivo:
```css
@import "bootstrap/dist/css/bootstrap.min.css";
```

---

## 🚀 Compilación y Ejecución

Para iniciar el servidor local de desarrollo y visualizar el resultado en el navegador:

```bash
ng serve
```

*(Puedes agregar la bandera `-o` para abrir la pestaña en el navegador automáticamente: `ng serve -o`)*