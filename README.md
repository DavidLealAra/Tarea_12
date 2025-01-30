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
![odoo_db](Tarea_12_Imagenes/consulta_apartado_1.png)


