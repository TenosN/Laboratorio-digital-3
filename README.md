# Laboratorio 2: Diseño y Simulación de Circuitos Sumadores y Restadores
**Asignatura:** Electrónica Digital  
**Institución:** [Nombre de tu Universidad]  
**Autor:** [Tu Nombre Completo]  
**Fecha:** Septiembre 2026  

> **Resumen (Abstract):** Este informe/laboratorio presenta el diseño, implementación en HDL y simulación de circuitos aritméticos combinacionales. En la Parte A se aborda el desarrollo incremental desde un sumador de 1 bit hasta un sumador de 4 bits. En la Parte B se presenta el diseño de un sumador/restador parametrizado y la resolución de un reto de diseño aritmético complementario.

---

## 📄 Tabla de Contenidos
1. [Requisitos y Entorno de Desarrollo](#-requisitos-y-entorno-de-desarrollo)
2. [Parte A: Circuitos Sumadores](#-parte-a-circuitos-sumadores)
   - [1. Sumador Completo de 1 Bit](#1-sumador-completo-de-1-bit)
   - [2. Sumador de 4 Bits](#2-sumador-de-4-bits)
3. [Parte B: Sumador / Restador y Reto de Diseño](#-parte-b-sumador--restador-y-reto-de-diseño)
   - [1. Circuitos Sumador / Restador](#1-circuito-sumador--restador)
   - [2. Reto de Diseño](#2-reto-de-diseño)
4. [Conclusiones](#-conclusiones)

---

## 🛠️ Requisitos y Entorno de Desarrollo

El proyecto puede ser ejecutado, editado y simulado utilizando **GitHub Codespaces** o cualquier entorno local basado en VS Code.

| Herramienta / Software | Función / Descripción |
| :--- | :--- |
| **Lenguaje HDL** | Verilog / VHDL *(especificar según corresponda)* |
| **Simulador** | Icarus Verilog / ModelSim / Vivado |
| **Visor de Ondas** | GTKWave |
| **Entorno de desarrollo** | GitHub Codespaces / VS Code |

> **Nota para Codespaces:** Si utilizas GitHub Codespaces, asegúrate de tener instalada la extensión de Verilog/VHDL y GTKWave para visualizar las simulaciones `.vcd`.

---

## 🔬 Parte A: Circuitos Sumadores

### 1. Sumador Completo de 1 Bit

#### A. Código del Módulo
```verilog
// Reemplaza este código por tu implementación del Sumador de 1 bit
module full_adder_1bit (
    input wire a,
    input wire b,
    input wire cin,
    output wire sum,
    output wire cout
);

    assign sum = a ^ b ^ cin;
    assign cout = (a & b) | (b & cin) | (a & cin);

endmodulw
