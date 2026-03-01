# 📄 README.md - Solo Práctica 1 de Laboratorio

```markdown
# Práctica 1 - POO con TypeScript

> Ejercicios de Laboratorio - Clases, Atributos, Métodos e Instanciación de Objetos

---

## 📚 Información de la Práctica

- **Institución:** Universidad de Oriente (UNIVO)
- **Asignatura:** Programación Orientada a Objetos
- **Sesión:** 01
- **Lugar:** CDS2
- **Horario:** 8:40 AM - 10:30 AM
- **Tema:** Clases, atributos, métodos e instanciación de objetos

---

## 🎯 Objetivos

1. ✅ Reforzar la definición correcta de clases, atributos y métodos en TypeScript
2. ✅ Implementar constructores para inicializar atributos
3. ✅ Instanciar objetos y ejecutar sus métodos
4. ✅ Analizar cómo cada objeto mantiene su propio estado independiente

---

## 📋 Contenido

### **💻 Ejercicios en Clase (2)**

| # | Ejercicio | Descripción | Archivo |
|---|-----------|-------------|---------|
| 1 | **Estudiante** | Clase con nombre, carnet y nota final. Métodos para mostrar información y verificar aprobación | `practica1-estudiante.ts` |
| 2 | **Producto** | Clase con nombre, precio y cantidad. Métodos para calcular total y mostrar detalle | `practica1-producto.ts` |

### **📝 Tareas (4)**

| # | Tarea | Descripción | Archivo |
|---|-------|-------------|---------|
| 1 | **Empleado** | Salario base + horas trabajadas con tarifa fija | `tarea1-empleado.ts` |
| 2 | **Cuenta Bancaria** | Operaciones de depósito, retiro y consulta de saldo | `tarea2-cuenta.ts` |
| 3 | **Vehículo** | Información completa de marca, modelo y año | `tarea3-vehiculo.ts` |
| 4 | **Libro** | Título, autor, número de páginas con métodos de información | `tarea4-libro.ts` |

---

## 🛠️ Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- **Node.js** v18 o superior → [Descargar](https://nodejs.org/)
- **npm** (se instala con Node.js)
- **Visual Studio Code** (recomendado) → [Descargar](https://code.visualstudio.com/)

### **Verificar instalación:**

```bash
node --version    # v18 o superior
npm --version     # v9 o superior
```

---

## 🚀 Instalación

### **1. Clonar el repositorio:**

```bash
git clone https://github.com/TU_USUARIO/practica1-poo-typescript.git
cd practica1-poo-typescript
```

### **2. Instalar dependencias:**

```bash
npm install
```

### **3. Compilar TypeScript:**

```bash
npx tsc
```

---

## 📁 Estructura del Proyecto

```
practica1-poo-typescript/
│
├── src/                                # Código fuente TypeScript
│   ├── practica1-estudiante.ts         ✅ Ejercicio 1 (Clase)
│   ├── practica1-producto.ts           ✅ Ejercicio 2 (Clase)
│   ├── tarea1-empleado.ts              ✅ Tarea 1
│   ├── tarea2-cuenta.ts                ✅ Tarea 2
│   ├── tarea3-vehiculo.ts              ✅ Tarea 3
│   └── tarea4-libro.ts                 ✅ Tarea 4
│
├── dist/                               # JavaScript compilado
│   ├── practica1-estudiante.js
│   ├── practica1-producto.js
│   ├── tarea1-empleado.js
│   ├── tarea2-cuenta.js
│   ├── tarea3-vehiculo.js
│   └── tarea4-libro.js
│
├── node_modules/                       # Dependencias (no en Git)
├── .gitignore                          # Archivos ignorados
├── package.json                        # Configuración del proyecto
├── tsconfig.json                       # Configuración TypeScript
└── README.md                           # Este archivo
```

---

## ▶️ Cómo Ejecutar

### **Compilar todos los ejercicios:**

```bash
npx tsc
```

### **Ejecutar ejercicios en clase:**

```bash
# Ejercicio 1: Estudiante
node dist/practica1-estudiante.js

# Ejercicio 2: Producto
node dist/practica1-producto.js
```

### **Ejecutar tareas:**

```bash
# Tarea 1: Empleado
node dist/tarea1-empleado.js

# Tarea 2: Cuenta Bancaria
node dist/tarea2-cuenta.js

# Tarea 3: Vehículo
node dist/tarea3-vehiculo.js

# Tarea 4: Libro
node dist/tarea4-libro.js
```

---

## 📖 Descripción de Ejercicios

### **📌 Ejercicio 1: Clase Estudiante**

**Requisitos:**
- Atributos: `nombre`, `carnet`, `notaFinal`
- Constructor para inicializar valores
- Método `mostrarInformacion()` que imprime los datos
- Instanciar al menos 2 objetos

**Ejemplo de salida:**
```
=== CLASE ESTUDIANTE ===

═══════════════════════════════
Nombre: Juan Pérez
Carnet: 2024001
Nota Final: 8.5
═══════════════════════════════

Estado: Bueno
¿Aprobó?: Sí
```

---

### **📌 Ejercicio 2: Clase Producto**

**Requisitos:**
- Atributos: `nombre`, `precio`, `cantidad`
- Método `calcularTotal()` que retorna precio × cantidad
- Método `mostrarDetalle()` que imprime la información
- Instanciar al menos 1 objeto

**Ejemplo de salida:**
```
=== CLASE PRODUCTO ===

┌─────────────────────────────────┐
│ Producto: Laptop Dell           │
│ Precio: $850.00                 │
│ Cantidad: 2                     │
│ Total: $1700.00                 │
└─────────────────────────────────┘
```

---

### **📌 Tarea 1: Clase Empleado**

**Requisitos:**
- Atributos: `nombre`, `salarioBase`, `horasTrabajadas`
- Método `calcularSalarioTotal()` (salarioBase + horasTrabajadas × tarifa)
- Tarifa fija por hora: $15

**Ejemplo de salida:**
```
┌────────────────────────────────────────┐
│ Empleado: Ana Martínez                 │
├────────────────────────────────────────┤
│ Salario Base: $800.00                  │
│ Horas Trabajadas: 40                   │
│ Tarifa por Hora: $15.00                │
│ Pago por Horas: $600.00                │
├────────────────────────────────────────┤
│ SALARIO TOTAL: $1400.00                │
└────────────────────────────────────────┘
```

---

### **📌 Tarea 2: Clase CuentaBancaria**

**Requisitos:**
- Atributos: `titular`, `saldo` (inicia en 0)
- Método `depositar(monto)` con validación
- Método `retirar(monto)` validando saldo suficiente
- Método `mostrarSaldo()`

**Ejemplo de salida:**
```
--- Operaciones de Juan ---

✅ Depósito exitoso de $1000.00
💰 Nuevo saldo: $1000.00

✅ Retiro exitoso de $300.00
💰 Nuevo saldo: $700.00

❌ Error: Fondos insuficientes
   Saldo actual: $700.00
   Monto solicitado: $1000.00
```

---

### **📌 Tarea 3: Clase Vehiculo**

**Requisitos:**
- Atributos: `marca`, `modelo`, `año`
- Método `mostrarInformacion()` que imprime todos los datos
- Instanciar 2 vehículos diferentes

**Ejemplo de salida:**
```
┌───────────────────────────────────┐
│ 🚗 INFORMACIÓN DEL VEHÍCULO      │
├───────────────────────────────────┤
│ Marca: Toyota                     │
│ Modelo: Corolla                   │
│ Año: 2024                         │
└───────────────────────────────────┘

Antigüedad: 2 años
¿Es nuevo?: Sí
```

---

### **📌 Tarea 4: Clase Libro**

**Requisitos:**
- Atributos: `titulo`, `autor`, `numeroPaginas`
- Método para mostrar información
- Instanciar al menos 2 libros

**Ejemplo de salida:**
```
╔═══════════════════════════════════════╗
║ 📚 Cien Años de Soledad               ║
╠═══════════════════════════════════════╣
║ Autor: Gabriel García Márquez         ║
║ Páginas: 417                          ║
║ Categoría: Libro Largo                ║
╚═══════════════════════════════════════╝

⏱️  Tiempo de lectura estimado: 6h 57min
```

---

## 🎓 Conceptos Aplicados

| Concepto | Descripción |
|----------|-------------|
| **Clase** | Plantilla o molde para crear objetos |
| **Constructor** | Método especial que inicializa atributos |
| **Atributos** | Variables que almacenan el estado del objeto |
| **Métodos** | Funciones que definen el comportamiento |
| **Instanciación** | Crear objetos usando `new` |
| **Encapsulamiento** | Uso de `public`, `private` para control de acceso |
| **Estado Independiente** | Cada objeto mantiene sus propios valores |

---

## 📚 Sintaxis Básica TypeScript

### **Definir una clase:**

```typescript
class Estudiante {
  // Atributos
  nombre: string;
  carnet: string;
  notaFinal: number;

  // Constructor
  constructor(nombre: string, carnet: string, notaFinal: number) {
    this.nombre = nombre;
    this.carnet = carnet;
    this.notaFinal = notaFinal;
  }

  // Método
  mostrarInformacion(): void {
    console.log(`Nombre: ${this.nombre}`);
    console.log(`Carnet: ${this.carnet}`);
    console.log(`Nota: ${this.notaFinal}`);
  }
}
```

### **Instanciar objetos:**

```typescript
// Crear objetos
const estudiante1 = new Estudiante("Juan", "2024001", 8.5);
const estudiante2 = new Estudiante("María", "2024002", 9.2);

// Ejecutar métodos
estudiante1.mostrarInformacion();
estudiante2.mostrarInformacion();
```

### **Constructor compacto (recomendado):**

```typescript
class Producto {
  // Declaración e inicialización en una línea
  constructor(
    public nombre: string,
    public precio: number,
    public cantidad: number
  ) {}

  calcularTotal(): number {
    return this.precio * this.cantidad;
  }
}
```

---

## 🔧 Configuración del Proyecto

### **package.json:**

```json
{
  "name": "practica1-poo-typescript",
  "version": "1.0.0",
  "description": "Práctica 1 - POO con TypeScript",
  "main": "dist/practica1-estudiante.js",
  "scripts": {
    "build": "tsc",
    "start:estudiante": "tsc && node dist/practica1-estudiante.js",
    "start:producto": "tsc && node dist/practica1-producto.js",
    "start:empleado": "tsc && node dist/tarea1-empleado.js",
    "start:cuenta": "tsc && node dist/tarea2-cuenta.js",
    "start:vehiculo": "tsc && node dist/tarea3-vehiculo.js",
    "start:libro": "tsc && node dist/tarea4-libro.js"
  },
  "keywords": ["typescript", "poo", "practica"],
  "author": "Tu Nombre",
  "license": "ISC",
  "devDependencies": {
    "@types/node": "^22.0.0",
    "typescript": "^5.9.3"
  }
}
```

### **tsconfig.json:**

```json
{
  "compilerOptions": {
    "target": "ES2020",
    "module": "commonjs",
    "moduleResolution": "node",
    "rootDir": "./src",
    "outDir": "./dist",
    "strict": true,
    "esModuleInterop": true,
    "skipLibCheck": true,
    "forceConsistentCasingInFileNames": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules", "dist"]
}
```

---

## 📊 Resumen de Ejercicios

| Archivo | Clase | Atributos | Métodos | Estado |
|---------|-------|-----------|---------|--------|
| `practica1-estudiante.ts` | Estudiante | nombre, carnet, notaFinal | mostrarInformacion(), aprobo() | ✅ |
| `practica1-producto.ts` | Producto | nombre, precio, cantidad | calcularTotal(), mostrarDetalle() | ✅ |
| `tarea1-empleado.ts` | Empleado | nombre, salarioBase, horasTrabajadas | calcularSalarioTotal() | ✅ |
| `tarea2-cuenta.ts` | CuentaBancaria | titular, saldo | depositar(), retirar(), mostrarSaldo() | ✅ |
| `tarea3-vehiculo.ts` | Vehiculo | marca, modelo, año | mostrarInformacion() | ✅ |
| `tarea4-libro.ts` | Libro | titulo, autor, numeroPaginas | mostrarInformacion() | ✅ |

---

## 🐛 Solución de Problemas

### **Error: "Cannot find module 'typescript'"**
```bash
npm install -D typescript
```

### **Error: "Cannot find name 'process'"**
```bash
npm install -D @types/node
```

### **No se crea la carpeta dist/**
```bash
# Verificar que tsconfig.json está configurado correctamente
# Verificar que los archivos .ts están en src/
dir src
```

### **VSCode muestra errores pero compila bien**
```bash
# Reiniciar TypeScript Server
# Ctrl + Shift + P → "TypeScript: Restart TS Server"
```

---

## 📝 Checklist de Completado

- [ ] Ejercicio 1: Estudiante ✅
- [ ] Ejercicio 2: Producto ✅
- [ ] Tarea 1: Empleado
- [ ] Tarea 2: Cuenta Bancaria
- [ ] Tarea 3: Vehículo
- [ ] Tarea 4: Libro
- [ ] Todos compilan sin errores
- [ ] Todos ejecutan correctamente
- [ ] Código documentado y limpio
- [ ] README actualizado

---

## 👨‍💻 Autor

**Nombre:** [Tu Nombre Completo]  
**Carnet:** [Tu Número de Carnet]  
**Curso:** Programación Orientada a Objetos  
**Sección:** A  
**Universidad:** Universidad de Oriente (UNIVO)  
**Fecha:** Febrero 2026

---

## 📧 Contacto

- **Instructor:** Ing. William José Morales Berrios
- **Asignatura:** 1383 - Programación Orientada a Objetos
- **Sesión:** 01 - Práctica de Laboratorio

---

## 📄 Licencia

Este proyecto es material educativo para fines académicos.

**Universidad de Oriente** © 2026

---

## 🎯 Objetivos de Aprendizaje Cumplidos

Al completar esta práctica, has demostrado:

- ✅ Comprensión de clases y objetos en TypeScript
- ✅ Implementación correcta de constructores
- ✅ Uso apropiado de atributos y métodos
- ✅ Instanciación múltiple de objetos
- ✅ Validación de entrada de datos
- ✅ Separación de responsabilidades
- ✅ Código limpio y documentado

---

<div align="center">

**🎓 Práctica 1 - Programación Orientada a Objetos 🎓**

[![Made with TypeScript](https://img.shields.io/badge/Made%20with-TypeScript-blue)](https://www.typescriptlang.org/)

**Universidad de Oriente - 2026**

</div>
