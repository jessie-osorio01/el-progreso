# Cómo conectar la página a una base de datos más adelante

Hoy todo se guarda en el navegador con **LocalStorage**. En `index.html` existe un objeto `Store` que centraliza el almacenamiento: solo hay que cambiar estas funciones, el resto de la página no se toca.

| Función actual | Dato | Equivalente en Firebase (Firestore) |
|---|---|---|
| `Store.saveUser(u)` | Registro del cliente | `setDoc(doc(db,'clientes',uid), u)` |
| `Store.saveOrder(o)` | Pedido | `addDoc(collection(db,'pedidos'), o)` |
| `Store.getOrders()` | Historial | `query(collection(db,'pedidos'), where('customer.phone','==',tel))` |
| `CONFIG.coupons` | Códigos de descuento | colección `cupones` (campos `codigo`, `pct`, `activo`) |
| `PRODUCTS` | Catálogo | colección `productos` |

## Pasos con Firebase
1. Crea un proyecto en https://console.firebase.google.com y activa **Firestore** y **Authentication** (teléfono o correo).
2. Agrega una app web y copia el `firebaseConfig`.
3. Carga el SDK con `<script type="module">` desde el CDN de Firebase, inicializa `db` y reemplaza las funciones del `Store` por versiones `async`.
4. Reglas de seguridad: cada cliente solo lee y escribe sus propios pedidos.

## Alternativa con Python (FastAPI)
- Endpoints: `POST /pedidos`, `GET /pedidos?telefono=`, `POST /clientes`, `GET /productos`, `POST /cupones/validar`.
- Base de datos: SQLite o PostgreSQL.
- En la página, el `Store` pasaría a usar `fetch('/api/...')`.
