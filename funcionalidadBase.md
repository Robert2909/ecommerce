# Funcionalidad de la base de datos

## Descripción

Base de datos desarrollada en SQL para gestionar y manipular la información del software de administración del gimnasio.

### Recursos utilizados

1. Procedimientos almacenados (Procedures).
2. Procedimientos con cursores.
3. Función sin parámetros.
4. Función con parámetros.
5. Trigger simple.
6. Trigger de eliminación en cascada - **BEFORE**.
7. Trigger de eliminación en cascada - **AFTER**.
8. Índices para optimización.

## Ejemplo implementación

| Método | Código |
|--------|--------|
| Procedure | delimiter // create procedure paProductos() begin select * from producto; end // delimiter // |
| Función sin parámetros | delimiter // create function HolaMundo() returns **VARCHAR(20)** as begin RETURN 'Hola mundo'; END |
| Trigger simple | create trigger trgDespuesDeCliente on Clientes after INSERT AS BEGIN PRINT 'Se ha insertado un nuevo cliente en la tabla clientes'; END |
| Índice | create index idxNombreCliente on Clientes (Nombre); |
