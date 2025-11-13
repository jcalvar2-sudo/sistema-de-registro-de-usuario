# 💻 Sistema de Registro de Usuarios

## 📌 Descripción del Caso
El sistema de registro de usuarios constituye un componente esencial de la plataforma, encargado de gestionar la creación, validación y administración de cuentas.  
Actualmente presenta problemas de usabilidad, seguridad y escalabilidad, como:
- Dificultad en el registro por requisitos de contraseña.
- Alta tasa de abandono en la confirmación por correo.
- Vulnerabilidades frente a ataques de fuerza bruta.
- Limitaciones técnicas en la base de datos y documentación insuficiente.

---

## 🎯 Objetivos
- Optimizar la experiencia de registro para nuevos usuarios.
- Garantizar altos estándares de seguridad y protección de datos.
- Mejorar la mantenibilidad y escalabilidad del sistema.
- Reducir la carga de soporte técnico mediante automatización.
- Alinear el sistema con estándares modernos de usabilidad y confiabilidad.

---

## 📋 Requerimientos

### Funcionales
- RF01: Registro de nuevos usuarios con validación de datos.
- RF02: Inicio de sesión con credenciales seguras.
- RF03: Recuperación de contraseñas mediante correo de verificación.
- RF04: Administración de usuarios (crear, editar, eliminar).
- RF05: Registro de fecha y hora de creación de cuentas.

### No Funcionales
- RNF01: Tiempo de respuesta ≤ 2.5 segundos.
- RNF02: Cifrado seguro de contraseñas (bcrypt/SHA-256).
- RNF03: Interfaz responsiva para móviles y escritorio.
- RNF04: Soporte de al menos 500 registros simultáneos sin pérdida de datos.

---

## 🧪 Tabla de Pruebas

| ID Caso | Tipo de Prueba | Requerimiento Asociado | Datos de Entrada | Resultado Esperado | Validación |
|---------|----------------|------------------------|------------------|--------------------|------------|
| CPU-01  | Unitaria       | RF01                   | Nombre: "Carlos Vega", Correo: "carlos@mail.com", Contraseña: "Car12345" | Registro exitoso | ✔ |
| CPU-02  | Integración    | RF02                   | Autenticación con Google | Inicio de sesión correcto | ✔ |
| CPU-03  | Validación     | RF03                   | Contraseña incorrecta 3 veces | Bloqueo temporal de cuenta | ✔ |
| CPU-04  | Rendimiento    | RNF01                  | 1,000 registros simultáneos | Respuesta < 3s | ✔ |
| CPU-05  | Seguridad      | RF04                   | Intento de acceso sin credenciales válidas | Error "Acceso denegado" | ✔ |

---

## 🔧 Tipos de Mantenimiento Propuesto
- **Correctivo:** Reparación de bugs en verificación de email y protección contra fuerza bruta.  
- **Adaptativo:** Integración con OAuth 2.0 y soporte biométrico.  
- **Perfectivo:** Rediseño de interfaz y optimización del flujo de registro.  
- **Preventivo:** Migración a microservicios y creación de pruebas automatizadas.  

---

## 🔄 Reflexión sobre el Control de Versiones
El control de versiones (ej. Git/GitHub) es fundamental para la evolución del sistema:  
- Permite **rastrear cambios** en el código y documentación.  
- Facilita la **colaboración** entre múltiples desarrolladores.  
- Garantiza la **reproducibilidad** de pruebas y mantenimientos.  
- Ayuda a gestionar **ramas de desarrollo** para nuevas funciones sin afectar la versión estable.  
- Proporciona evidencia visual (historial de commits, diagramas de flujo de trabajo) que respalda la calidad académica y profesional del proyecto.  

En conclusión, el control de versiones no solo organiza el trabajo técnico, sino que también asegura la transparencia y confiabilidad del proceso de mejora continua del sistema.

---
