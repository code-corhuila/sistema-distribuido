# 🛒 Sistema Distribuido - Shopping Cart

Sistema distribuido basado en arquitectura de microservicios para gestión de carrito de compras, inventario y facturación.

---

## 📋 Descripción

Sistema empresarial distribuido que implementa un ecosistema completo de e-commerce con separación por dominios:

- **Security**: Autenticación, autorización y gestión de usuarios
- **Bill**: Gestión financiera y transaccional
- **Inventory**: Control de productos y stock

---

## 🏗️ Arquitectura

El sistema está organizado en microservicios independientes, cada uno con su propia API backend y frontends especializados (portal web y aplicación móvil).

### Dominios Principales

#### 🔐 SECURITY
- `shopping-cart-security-api` - API de autenticación y autorización
- `shopping-cart-security-portal` - Portal web de administración de usuarios
- `shopping-cart-security-app` - Aplicación móvil de seguridad

Gestiona usuarios, roles, permisos y emisión/validación de tokens con persistencia en base de datos SQL central.

#### 💳 BILL
- `shopping-cart-bill-api` - API de lógica de negocio financiera
- `shopping-cart-bill-data` - Capa de acceso a datos y migraciones
- `shopping-cart-bill-portal` - Portal web de facturación
- `shopping-cart-bill-app` - Aplicación móvil de facturación

Dominio financiero y transaccional con soporte híbrido para reportes y procesos especiales.

#### 📦 INVENTORY
- `shopping-cart-inventory-api` - API de gestión de inventario
- `shopping-cart-inventory-portal` - Portal web de inventario
- `shopping-cart-inventory-app` - Aplicación móvil de inventario

Gestión de productos, stock y movimientos con persistencia en base de datos SQL core compartida.

---

## 🎯 Principios Arquitectónicos

- ✅ Un repositorio por microservicio backend
- ✅ Un repositorio por frontend (portal y app)
- ✅ Modelo de datos core centralizado en SQL
- ✅ Separación estricta por dominio
- ✅ Independencia de despliegue por microservicio

---

## 📚 Documentación Adicional

Para más detalles sobre la arquitectura y repositorios oficiales, consulta:

- [Documentación de Repositorios](archiecture/repository/README.md)

---

## 🚀 Tecnologías

- Arquitectura de Microservicios
- Base de datos SQL (centralizada)
- APIs REST
- Aplicaciones Web (Portal)
- Aplicaciones Móviles

---

## 📝 Notas

Este proyecto sigue un enfoque de arquitectura distribuida con separación clara de responsabilidades por dominio de negocio.