# Manual tecnico - GreenLife

## Arquitectura
Aplicación cliente-servidor con API REST.

## Tecnologías
- Backend: Node.js
- Frontend: React
- Base de datos: PostgreSQL

## Estructura del codigo
- `/backend` - API y lógica de negocio
- `/frontend` - Interfaz de usuario
- `/database` - Migraciones y modelos

## Autenticació JWT
L'API utilitza JSON Web Tokens (JWT) per autenticar els usuaris.
1. L'usuari fa login a `POST /api/auth/login` amb el seu email i contrasenya.
2. El servidor retorna un token JWT.
3. A cada petició, s'envia el token a la capçalera:
   `Authorization: Bearer <token>`
4. El token caduca al cap de 24 hores.