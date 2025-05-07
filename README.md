<img width="637" alt="Beetrack-presentation" src="https://github.com/user-attachments/assets/931e206d-e36f-498e-8454-ce97d1f22a74" />

# Beetrack

**Beetrack** es una aplicación de gestión de comercio con panel de control (dashboard) inteligente que permite visualizar reportes diarios, comparar rangos de tiempo, identificar los productos más vendidos y consultar el saldo total en caja. Diseñada para ofrecer una visión clara del rendimiento del negocio.

## 🚀 Características

- 📅 Reportes diarios agregados por tienda
- 📈 Comparación de periodos personalizados
- 🏆 Top 10 productos más vendidos
- 💵 Visualización del saldo total en caja
- 🔐 Autenticación por tienda
- ⚙️ Backend estructurado con Prisma, servicios y validaciones DTO
- 💡 Frontend con Chakra UI y componentes reutilizables

## 🧑‍💻 Tecnologías

- **Frontend:** React, TypeScript, Chakra UI
- **Backend:** Next.js (App Router), Prisma, PostgreSQL
- **ORM:** Prisma
- **Validación:** Zod
- **Autenticación:** Tokens (cookie-based)

1. Instalar dependencias:

```bash
npm install
```

2. Configurar las variables de entorno:

Crea un archivo `.env`:

```env
DATABASE_URL=postgresql://user:password@localhost:5432/beetrack
JWT_SECRET=your_secret_key
```

3. Ejecutar migraciones y abrir Prisma Studio (opcional):

```bash
npx prisma migrate dev
npx prisma studio
```

4. Levantar el servidor:

```bash
npm run dev
```

## 📊 Ejemplo de uso de la API

### Obtener saldo total en caja

```http
GET /api/dashboard?view=cash
```

### Obtener reporte diario

```http
GET /api/dashboard?view=daily&date=2025-05-06
```
---

Desarrollado con ❤️ por [Germán](https://github.com/germandosaula), [Javier](https://github.com/javierhidalgodev), [Jason](https://github.com/GuyFawkess) y [Jonathan](https://github.com/jomuarribas)
