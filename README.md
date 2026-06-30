# 💄 Girly Essentials - Inventario en la nube

Sistema completo de inventario con login, base de datos en Supabase y deploy en Vercel.

---

## 🚀 Pasos para subirlo (15 minutos)

### PASO 1: Crear cuenta en Supabase (gratis)

1. Ve a **https://supabase.com** y crea una cuenta (puedes usar tu email o Google)
2. Click en **"New Project"**
3. Llena los datos:
   - **Name:** `girly-essentials`
   - **Database Password:** elige una contraseña segura (guárdala bien)
   - **Region:** elige la más cercana a México (por ejemplo, `East US`)
4. Click **"Create new project"** y espera 1-2 minutos a que se cree

### PASO 2: Crear las tablas en Supabase

1. En tu proyecto de Supabase, ve a **SQL Editor** (menú de la izquierda)
2. Click en **"New query"**
3. Abre el archivo **`schema.sql`** de este proyecto, copia TODO el contenido
4. Pégalo en el editor SQL de Supabase y click en **"Run"** (esquina inferior derecha)
5. Debes ver "Success. No rows returned"

### PASO 3: Cargar tus 738 productos

1. En el mismo **SQL Editor**, click en **"New query"**
2. Abre **`seed_products.sql`**, copia TODO
3. Pégalo y click **"Run"**
4. Debes ver "Success. 738 rows inserted"

### PASO 4: Conseguir tus credenciales de Supabase

1. En Supabase, ve a **Settings → API** (engranaje en el menú izquierdo)
2. Copia estos dos valores:
   - **Project URL** (algo como `https://abcdefg.supabase.co`)
   - **anon public** key (un texto largo)

### PASO 5: Configurar el proyecto

1. Abre el archivo **`config.js`**
2. Reemplaza los valores:
   ```javascript
   const SUPABASE_URL = 'https://tu-proyecto.supabase.co';
   const SUPABASE_KEY = 'tu-anon-key';
   ```
3. Guarda el archivo

### PASO 6: Subir a Vercel (gratis)

#### Opción A — La más fácil (drag & drop)

1. Ve a **https://vercel.com** y crea cuenta (puedes usar GitHub o email)
2. En el dashboard, click en **"Add New..." → "Project"**
3. En la parte de abajo verás **"Deploy a template"** o **"Browse all templates"**
4. Mejor: arrastra toda esta carpeta a `https://vercel.com/new` (busca "Drag and drop")
5. Si te pide configurar algo, déjalo todo por defecto
6. Click **"Deploy"** y espera 30 segundos
7. ¡Listo! Te dará un link como `https://girly-essentials.vercel.app`

#### Opción B — Con GitHub (recomendada si vas a hacer cambios)

1. Sube esta carpeta a un repositorio nuevo en GitHub
2. En Vercel, click **"Add New" → "Project"**
3. Conecta tu cuenta de GitHub e importa el repo
4. Click **"Deploy"**

---

## 🔑 Datos de acceso

- **URL:** la que te dé Vercel después del deploy
- **Usuario:** `fatima`
- **Contraseña:** `girly2026`

---

## ✨ Características

- ✅ **Login con tu usuario** — solo tú accedes
- ✅ **Sincronización real entre dispositivos** — abres desde celular, compu, tablet y todo se actualiza
- ✅ **738 productos precargados**
- ✅ **Catálogo completo** con búsqueda, filtros y orden
- ✅ **Gestión de clientes** con abonos parciales
- ✅ **Subir fotos** desde tu galería (se guardan en la nube)
- ✅ **Exportar a CSV** cuando quieras

---

## 📱 Cómo usarlo después del deploy

1. Abre el link de Vercel desde tu celular o computadora
2. Inicia sesión con `fatima` / `girly2026`
3. Lo que hagas en un dispositivo se ve en cualquier otro al instante
4. Te recomiendo guardar el link en favoritos o crear un acceso directo en tu pantalla de inicio

---

## ❓ ¿Algún problema?

- **No se ve nada al abrir:** revisa que `config.js` tenga las credenciales correctas de Supabase
- **No me deja entrar:** asegúrate de que ejecutaste `schema.sql` completo (debe crear la tabla `users` con fatima)
- **No aparecen los productos:** ejecuta `seed_products.sql` en el SQL Editor de Supabase

---

¡Disfruta tu inventario! 🎀
