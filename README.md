# 🟪 Angular

Introduccion a Angular. En este entorno se explora la estructura de componentes, la interpolación de datos y el flujo de CLI de Angular.

---

## 📂 Estructura del Proyecto

```text
.
├── src/
│   ├── app/
│   │   ├── app.config.ts       # Configuración global de la aplicación
│   │   ├── app.css             # Estilos específicos del componente principal
│   │   ├── app.html            # Plantilla HTML con interpolación
│   │   ├── app.routes.ts       # Definición de rutas del proyecto
│   │   ├── app.spec.ts         # Pruebas unitarias básicas
│   │   └── app.ts              # Lógica de la clase y atributos exportados
│   ├── index.html              # Archivo HTML raíz
│   ├── main.ts                 # Punto de entrada de la aplicación
│   └── styles.css              # Estilos globales
├── angular.json                # Configuración del workspace de Angular
├── package.json                # Dependencias y scripts
├── tsconfig.json               # Configuración del compilador TypeScript
└── README.md
```

---

# ⚙️ Configuración del Entorno

Documentación completa de la instalación de Angular CLI + creación del proyecto.

---

## 1. Instalación Global de Angular CLI

Para disponer de las herramientas y comandos `ng` en el sistema, instalamos el CLI de Angular de manera global:

```bash
npm install -g @angular/cli
```

---

## 2. Creación del Proyecto e Ingreso al Directorio

Generamos la estructura base del entorno Angular y accedemos a la carpeta creada:

```bash
ng new proyecto
cd proyecto
```

---

## 3. Compilación y Ejecución

Para iniciar el servidor de desarrollo local y previsualizar los cambios en el navegador:

```bash
ng serve
```

*(Si deseas que el navegador se abra automáticamente al iniciar el servidor, ejecuta: `ng serve -o`)*