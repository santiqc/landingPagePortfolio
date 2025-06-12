#  Test Tecnico

##  1. Conocimientos SQL

### 1. ¿Para qué sirve una vista? 
Una vista en SQL es una tabla virtual basada en el resultado de una consulta (`SELECT`).  
Se utiliza para:

- Simplificar consultas complejas.
- Mejorar la seguridad restringiendo acceso a ciertas columnas o filas.
- Reutilizar consultas complejas sin repetir código.

---

### 2. ¿Cuál es el objetivo de un JOB?
Un JOB se utiliza para **automatizar tareas** como:

- Respaldos de base de datos.
- Limpieza o actualización de datos.
- Envío de reportes programados.

Se ejecuta de forma **programada** sin intervención manual. Cada tiempo estimado

---

### 3. ¿Cuál es la diferencia entre TRUNCATE, DELETE y DROP?

| Comando  | Descripción |
|----------|-------------|
| **TRUNCATE** | Elimina todos los registros de una tabla de forma rápida y definitiva. No se puede deshacer ni activa triggers. |
| **DELETE**   | Elimina registros específicos (usando `WHERE`). Se puede deshacer con transacciones y activa triggers. |
| **DROP**     | Elimina una tabla, vista o base de datos completamente, incluyendo datos y estructura. No se puede recuperar. |

---

### 4. ¿Qué función SQL se usa para obtener el mayor valor de una lista?

Lista: `{8, 1, 7, 2, 0, 3, 6, 4, 5, 9}`

```sql
SELECT MAX(numero) FROM tabla;
```
---

### 5. ¿Para qué se utiliza HAVING?

Se utiliza para filtrar resultados agregados después de aplicar GROUP BY, a diferencia de WHERE, que filtra antes del agrupamiento.

---

### 6. Query de especialidades y cuántas veces se repiten

```sql
SELECT especialidad, COUNT(*) AS cantidad
FROM PRUEBAESTUDIANTE
GROUP BY especialidad;
```
---

### 7. Consultar inscripciones con horario M-F9

```sql
SELECT *
FROM PRUEBAESTUDIANTE
WHERE horario = 'M-F9';
```


## 2. Ejercicio Java

### 1. Función para calcular el área de un triángulo

La fórmula para calcular el área de un triángulo es:  
```java
public double areaTriangulo(double base, double altura) {
    return (base * altura) / 2;
}
```
---
### 2. Función para área de círculo

La fórmula para calcular el área del circulo es:  
```java
public double areaCirculo(double radio) {
    return Math.PI * radio * radio;
}
```
