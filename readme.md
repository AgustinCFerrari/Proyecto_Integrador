# 🎾 Tenis Master – Sistema de Gestión de Reservas

## 📘 Descripción general

**Tenis Master** es una aplicación web desarrollada por **Redsoft** como parte del Proyecto Integrador (Comisión D).  
El sistema permite la **gestión integral de reservas de canchas de tenis**, el **matcheo de jugadores**, el **control administrativo** y la **gestión de clientes**, con diferentes roles de acceso (Administrador, Empleado y Cliente).

La interfaz está diseñada para ser **totalmente responsiva**, permitiendo su uso tanto en **PC** como en **dispositivos móviles**.  
- Los roles **Administrador** y **Empleado** están optimizados para escritorio.  
- El rol **Cliente** está pensado para una experiencia fluida en móviles.

---

## 👥 Integrantes del equipo Redsoft

- **Diego Arias**  
- **Agustín Ferrari**  
- **Sergio Godoy**

---

## 🌐 Enlaces del proyecto

- **Repositorio GitHub:**  
  [https://github.com/AgustinCFerrari/Proyecto_Integrador](https://github.com/AgustinCFerrari/Proyecto_Integrador)

- **Demo en Vercel:**  
  [https://proyecto-integrador-rose-ten.vercel.app/](https://proyecto-integrador-rose-ten.vercel.app/)

---

## 🔐 Roles y credenciales de acceso

| Rol | Correo electrónico | Contraseña |
|-----|--------------------|-------------|
| Administrador | `admin@mail.com` | `1234` |
| Empleado | `usuario@mail.com` | `1234` |
| Cliente | `cliente@mail.com` | `1234` |

> Los nuevos clientes pueden **autoregistrarse** desde la opción **“Crear cuenta”**.

---

## 🧭 Flujo principal del sistema

### 1️⃣ Inicio y autenticación
- Si el usuario no está logueado, el sistema redirige automáticamente de `index.html` a `login.html`.
- Dependiendo del rol, se accede a distintas vistas y funcionalidades.

### 2️⃣ Registro de nuevos clientes
- En “Crear cuenta” se completa un formulario con los datos personales.  
- Los empleados o administradores también pueden registrar clientes desde el **CRUD de Clientes**.

### 3️⃣ Panel de inicio (Cliente)
El cliente puede:
- Reservar una cancha.  
- Realizar matcheo con otros jugadores de su nivel.  
- Consultar sus reservas.  
- Cerrar sesión mediante el botón “Salir”.

### 4️⃣ Reservas
Desde la opción **Reservar**, el usuario ingresa:
- Fecha.  
- Hora de inicio y finalización.  
- Número de cancha.

Tras completar la información:
- Se accede a **pago.html**, donde se confirman los datos y se selecciona el método de pago.  
- Las reservas no pagadas aparecen como **pendientes** en “Mis reservas”.

### 5️⃣ Macheo de jugadores
El cliente puede elegir su nivel y disponibilidad.  
El sistema sugiere:
- Rival compatible.  
- Cancha y horario.  
- Al confirmar, se genera una reserva pendiente de pago.

---

## 🧑‍💼 Funcionalidades por rol

### 🟩 Rol Empleado
- Tiene un panel similar al cliente, pero con acceso adicional a:
  - **Gestión de Clientes (CRUD):** alta, baja, búsqueda y modificación.  
- Puede registrar reservas o clientes de manera presencial o telefónica.  

### 🟥 Rol Administrador
- Accede al **Panel de control**, con módulos específicos:
  - **Dashboard:** resumen diario de movimientos.  
  - **Calendario:** visualización de ocupación semanal por cancha.  
  - **Reservas:** listado general de reservas.  
  - **Reportes:** gráficos de ocupación e ingresos.  
  - **Usuarios:** listado con nivel, última reserva y cantidad de reservas.  
  - **Gestión de Clientes:** acceso al mismo CRUD que los empleados.

---

## 💻 Estructura del Front

- **index.html** – pantalla principal.  
- **login.html** – inicio de sesión.  
- **registro.html** – alta de nuevos clientes.  
- **reservar.html** – registro de reservas.  
- **pago.html** – confirmación y pago.  
- **mis-reservas.html** – listado de reservas.  
- **macheo.html** – emparejamiento de jugadores.  
- **admin-dashboard.html** – panel del administrador.  
- **admin-reservas.html**, **admin-calendario.html**, **admin-clientes.html** – vistas de gestión administrativa.

---

## 🖥️ Capturas de pantalla (resumen visual)

*(Las imágenes se encuentran documentadas en el archivo “Capturas de pantalla.docx”)*  
- Login y registro de usuarios.  
- Panel de inicio del cliente.  
- Formulario de reservas y pantalla de pago.  
- Macheo de jugadores.  
- CRUD de clientes.  
- Dashboard del administrador, calendario y reportes.

---

## ⚙️ Tecnologías utilizadas

- **HTML5**, **CSS3**, **JavaScript**  
- **TailwindCSS** (maquetado y responsive design)  
- **LocalStorage** (manejo de sesión y datos simulados)  
- **Vercel** (deploy del frontend)

---

## 🚀 Cómo ejecutar el proyecto

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/AgustinCFerrari/Proyecto_Integrador.git
   ```
2. Abrir el archivo `index.html` en el navegador.  
3. Utilizar las credenciales de prueba según el rol deseado.

---

## 🧾 Licencia
© Redsoft – 2025. Todos los derechos reservados.
