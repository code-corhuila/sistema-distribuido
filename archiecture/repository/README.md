# 📦 Repositorios Oficiales — Arquitectura Shopping Cart

---

## 🔐 SECURITY

- shopping-cart-security-api
- shopping-cart-security-portal
- shopping-cart-security-app

**Resumen:**
Dominio de autenticación y autorización.
Gestiona usuarios, roles, permisos y emisión/validación de tokens.
Persistencia en la base de datos SQL central.

---

## 💳 BILL

- shopping-cart-bill-api
- shopping-cart-bill-data
- shopping-cart-bill-portal
- shopping-cart-bill-app

**Resumen:**
Dominio financiero y transaccional.
bill-api contiene la lógica de negocio.
bill-data centraliza acceso a datos, migraciones y soporte híbrido (SQL core + procesos especiales como reportes o migración).
Incluye frontend web (portal) y aplicación móvil.

---

## 📦 INVENTORY

- shopping-cart-inventory-api
- shopping-cart-inventory-portal
- shopping-cart-inventory-app

**Resumen:**
Gestión de productos, stock y movimientos de inventario.
Persistencia en la base de datos SQL core compartida.
Separación clara entre backend y capas de presentación.

---

## 🎯 Lineamientos Arquitectónicos

- Un repositorio por microservicio backend.
- Un repositorio por frontend (portal y app).
- Modelo de datos core centralizado en SQL.
- Separación estricta por dominio.
- Independencia de despliegue por microservicio.