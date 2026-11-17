# Panel de Vida

Panel personal con hábitos, XP y niveles, tareas, metas, finanzas, cuerpo, modo enfoque y logros.
Es una sola página (`index.html`) que guarda los datos en Firebase tras iniciar sesión con correo y contraseña.

## Conectar Firebase (una sola vez)

1. Entra en https://console.firebase.google.com y crea un proyecto.
2. **Authentication > Sign-in method**: activa **Correo electrónico/contraseña**.
3. **Firestore Database**: crea la base de datos en modo producción.
4. En la pestaña **Reglas** de Firestore, pega el contenido de `firestore.rules` y publica.
5. **Configuración del proyecto > Tus apps > Web (`</>`)**: registra una app y copia `apiKey`, `authDomain`, `projectId` y `appId` en `firebase-config.js`.
6. **Authentication > Settings > Dominios autorizados**: añade el dominio de GitHub Pages (`TU_USUARIO.github.io`).

Mientras `firebase-config.js` tenga `PEGA_AQUI`, el panel funciona sin inicio de sesión y guarda solo en el navegador.

## Uso personal

La página es pública, así que cualquiera podría crear su propia cuenta en tu proyecto (nunca ver tus datos).
Para evitarlo, crea tu cuenta y luego desactiva los registros en
**Authentication > Settings > User actions > Enable create (sign-up)**.
