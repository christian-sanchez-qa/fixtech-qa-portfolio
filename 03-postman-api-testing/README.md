# Fixtech API Simulation – Postman Collection

Simulación de pruebas funcionales sobre endpoints de productos, basada en la lógica de testing aplicada en Fixtech e-commerce.

---

## Descripción

Este proyecto contiene una colección de Postman con pruebas funcionales que simulan las operaciones CRUD (Create, Read, Update, Delete) sobre un catálogo de productos. Los requests están modelados según la lógica de testing aplicada en un entorno real de e-commerce, utilizando JSONPlaceholder como API pública de práctica.

---

## Tecnologías utilizadas

- [Postman](https://www.postman.com/)
- [JSONPlaceholder](https://jsonplaceholder.typicode.com/) – API REST pública de práctica

---

## Estructura de la colección

```
Fixtech API Simulation
└── Productos
    ├── Obtener todos los productos   → GET    /posts
    ├── Obtener producto por ID       → GET    /posts/1
    ├── Crear producto                → POST   /posts
    ├── Actualizar producto           → PUT    /posts/1
    └── Eliminar producto             → DELETE /posts/1
```

---

## Casos de prueba

| Request | Método | URL | Código esperado | Resultado |
|---|---|---|---|---|
| Obtener todos los productos | GET | /posts | 200 OK | Lista completa de productos |
| Obtener producto por ID | GET | /posts/1 | 200 OK | Objeto con datos del producto |
| Crear producto | POST | /posts | 201 Created | Producto creado con ID asignado |
| Actualizar producto | PUT | /posts/1 | 200 OK | Objeto con datos actualizados |
| Eliminar producto | DELETE | /posts/1 | 200 OK | Objeto vacío `{}` |

---

## Cómo importar la colección

1. Abrí Postman
2. Click en **Import**
3. Seleccioná el archivo `Fixtech API Simulation.postman_collection.json`
4. La colección aparecerá lista en tu panel izquierdo

---

## Contexto

Esta colección forma parte de mi portfolio como QA Tester en transición profesional hacia el área de IT. Los requests replican la estructura de pruebas funcionales que aplico en mi experiencia real en Fixtech, un e-commerce donde realizo smoke testing, testing funcional y documentación de casos de prueba.

---

## Autor

**Christian Sanchez**  
QA Tester | Software Tester
[LinkedIn](https://www.linkedin.com/in/christian-sanchez-qa-analist-17-) · [GitHub](https://github.com/christian-sanchez-qa/fixtech-qa-portfolio)

