# Soporte de Cuentas y Privacidad · TE ESCUCHO APP

Portal web ligero pensado para desplegar en **Vercel** (y migrar posteriormente a un subdominio oficial de `teescuchoaqp.com`).

## Funciones incluidas
1. **Confirmación de correo electrónico** (`type=signup` / `email`) enviado vía Supabase Auth + Gmail SMTP.
2. **Recuperación y cambio de contraseña** (`type=recovery`) con validación de sesión PKCE/OTP.
3. **Política de Privacidad y Protección de Menores** (`#privacidad`), lista para registrar en Google Play Console.
4. **Eliminación de cuenta y datos** (`#eliminar`), requerida por Google Play Data Safety.

## Despliegue rápido en Vercel
1. Importa este repositorio en [vercel.com](https://vercel.com).
2. No requiere comando de compilación (es un sitio estático HTML/JS puro).
3. Copia el dominio asignado por Vercel (por ejemplo `https://soporte-te-escucho.vercel.app`).
4. Agrégalo en **Supabase Dashboard → Authentication → URL Configuration → Redirect URLs** y en el archivo `.env` de la app Flutter (`AUTH_REDIRECT_URL`).
