# Frontend - Desarrollo Web 

Aplicación React con autenticación JWT y Google OAuth.

## Tecnologías

- React 18 + Vite
- React Router DOM
- Axios
- CSS3

## Instalación

```bash
git clone <tu-repositorio>
cd frontend
npm install
```

## Configuración

Crear archivo `.env`:

```env
VITE_API_URL=http://localhost:5000/api
```

Para producción (`.env.production`):

```env
VITE_API_URL=https://tu-backend.onrender.com/api
```

## Ejecución

```bash
npm run dev
```

Aplicación en: `http://localhost:5173`

## Estructura

```
src/
├── components/       # Componentes reutilizables
├── pages/           # Páginas (Login, Dashboard, etc.)
├── services/        # Servicios API
└── App.jsx          # Componente principal
```

## Funcionalidades

- Registro de usuarios
- Login tradicional (email/password)
- Login con Google OAuth
- Dashboard protegido
- CRUD de usuarios
- Gestión de sesiones con localStorage

## Rutas

- `/login` - Iniciar sesión
- `/register` - Registro de usuario
- `/auth/callback` - Callback de Google OAuth
- `/dashboard` - Panel principal (protegido)
- `/users` - Gestión de usuarios (protegido)

## Despliegue en Vercel

1. Conectar repositorio de GitHub
2. Framework Preset: Vite
3. Build Command: `npm run build`
4. Output Directory: `dist`
5. Environment Variables: `VITE_API_URL=https://tu-backend.onrender.com/api`
6. Deploy

