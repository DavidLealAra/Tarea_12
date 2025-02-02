# Tarea_12

## Apartado 1

Accedemos a PgAdmin desde donde hacemos la siguiente query:
```bash
CREATE TABLE EmpresasFCT (
    idEmpresa SERIAL PRIMARY KEY,
    nombre VARCHAR(40) NOT NULL,
    quiereAlumnos BOOLEAN NOT NULL,
    numAlumnos INTEGER NOT NULL,
    fechaContacto DATE NOT NULL
);
```
![apartado_1](Tarea_12_Imagenes/consulta_apartado_1.png)

## Apartado 2

Insertar 5 registros
```bash
INSERT INTO EmpresasFCT (nombre, quiereAlumnos, numAlumnos, fechaContacto) VALUES
('Reverendos', FALSE, 0, '2024-01-15'),
('Maestros', TRUE, 5, '2023-12-10'),
('Entrenadores', FALSE, 0, '2024-02-05'),
('Libertinos', TRUE, 12, '2024-01-25'),
('HappyEnd', FALSE, 0, '2023-11-30');
```
![apartado_2](Tarea_12_Imagenes/consulta_apartado_2.png)

## Apartado 3

```bash
SELECT * FROM EmpresasFCT 
ORDER BY fechaContacto DESC;
```
![apartado_3](Tarea_12_Imagenes/consulta_apartado_3.png)

## Apartado 4

```bash
SELECT 
    rp.name AS Nombre,
    rp.city AS Ciudad,
    c.name AS NombreComercial
FROM res_partner rp
LEFT JOIN res_partner c ON rp.parent_id = c.id
WHERE rp.city = 'Tracy' 
AND rp.is_company = FALSE
ORDER BY c.name ASC;
```
![apartado_4](Tarea_12_Imagenes/consulta_apartado_4.png)






