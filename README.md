# 🛒 API Tienda

Proyecto de práctica usando:

- Node.js
- Express
- MySQL (XAMPP)
- HTML + Tailwind CSS

## Funcionalidades
- CRUD de productos
- CRUD de clientes
- Control de inventario
- Validaciones y mensajes visuales
- Diseño tipo dashboard oscuro

## Instalación

```bash
npm install
node src/app.js


CREATE DATABASE tienda;
USE tienda;

CREATE TABLE productos (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nombre VARCHAR(100),
  precio DECIMAL(10,2)
);

INSERT INTO productos (nombre, precio)VALUES
('Mouse',30000),
('Teclado',80000),
('Monitor',600000);

CREATE TABLE clientes (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nombre VARCHAR(100),
  email VARCHAR(100)
);

ALTER TABLE productos
ADD cantidad INT DEFAULT 0;
