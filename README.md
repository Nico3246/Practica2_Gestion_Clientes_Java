# Práctica 2 — Gestión de Clientes en Java

Práctica académica desarrollada en **Java** para trabajar conceptos fundamentales de **programación orientada a objetos**, especialmente herencia, polimorfismo, clonación, encapsulación y gestión de colecciones de objetos.

El proyecto modela una empresa con distintos tipos de clientes y operaciones básicas de alta, baja, búsqueda, facturación y aplicación de descuentos.

## Contexto académico

Este repositorio corresponde a una práctica universitaria. Su objetivo principal es aplicar conceptos de POO en Java dentro de un ejercicio estructurado, no representar una aplicación de producción ni un proyecto comercial independiente.

## Funcionalidades principales

La clase `Empresa` gestiona un conjunto de clientes y permite realizar operaciones como:

- dar de alta nuevos clientes;
- buscar clientes por NIF;
- eliminar clientes;
- consultar el número de clientes;
- calcular la facturación total;
- aplicar descuentos a determinados tipos de cliente;
- clonar objetos;
- comparar objetos mediante `equals`;
- mostrar información mediante `toString` y `ver()`.

## Modelo de clases

El proyecto incluye las siguientes clases principales:

- `Cliente`
- `ClienteMovil`
- `ClienteTarifaPlana`
- `Empresa`
- `Fecha`
- `Proceso`

### Cliente

Clase base con información como:

- NIF;
- código de cliente;
- nombre;
- fecha de nacimiento;
- fecha de alta.

Implementa clonación y comparación entre clientes.

### ClienteMovil

Especialización de `Cliente` orientada a clientes con tarifa por minuto y datos asociados al contrato móvil.

### ClienteTarifaPlana

Especialización de `Cliente` para clientes con un modelo de tarifa plana.

### Empresa

Mantiene una colección interna de clientes y centraliza operaciones de gestión, búsqueda, alta, baja, facturación y descuentos.

### Fecha

Clase auxiliar utilizada para representar y gestionar fechas asociadas a clientes.

### Proceso

Interfaz con operaciones básicas de comparación y visualización.

## Conceptos trabajados

Esta práctica aplica varios conceptos de programación orientada a objetos:

- herencia;
- polimorfismo;
- encapsulación;
- constructores;
- sobrecarga;
- sobrescritura;
- `equals`;
- `clone`;
- conversión de tipos;
- clases abstractas e interfaces;
- gestión manual de arrays de objetos;
- composición entre clases.

## Estructura del repositorio

```text
Practica2-version-final-/
├── Cliente.java
├── ClienteMovil.java
├── ClienteTarifaPlana.java
├── Empresa.java
├── Fecha.java
├── Proceso.java
└── .gitignore
```

Las clases pertenecen al paquete:

```text
LibClases
```

## Ejecución

El repositorio contiene principalmente las clases de dominio de la práctica. Para utilizarlas es necesario integrarlas en un proyecto Java que respete el paquete `LibClases` y disponga de una clase `main` o de pruebas que invoque sus operaciones.

Ejemplo de compilación, suponiendo que los archivos estén colocados en la estructura correcta del paquete:

```bash
javac LibClases/*.java
```

## Estado del proyecto

Es una práctica académica centrada en el aprendizaje de POO. Algunas decisiones están orientadas al ejercicio didáctico y no a una arquitectura de producción.

## Autor

Repositorio mantenido por [Nico3246](https://github.com/Nico3246).
