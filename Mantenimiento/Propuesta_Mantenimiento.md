# 💻 Propuesta de Mantenimiento del Sistema de Registro de Usuarios

## 📖 Introducción
El sistema de registro de usuarios constituye un componente esencial de la plataforma, encargado de gestionar la incorporación de nuevos usuarios.  
Actualmente presenta problemas de **usabilidad**, **seguridad** y **limitaciones técnicas**, que afectan la experiencia del usuario y la confiabilidad del servicio.  

Entre los principales problemas detectados se encuentran:
- Complejidad en requisitos de contraseña y confirmación por correo.
- Ausencia de opciones de registro alternativo (redes sociales).
- Vulnerabilidades de seguridad (fuerza bruta, falta de MFA).
- Escalabilidad limitada y tiempos de respuesta lentos.
- Documentación técnica insuficiente.

Con base en estas observaciones, se propone un plan de mantenimiento que combine acciones **correctivas**, **adaptativas**, **perfectivas** y **preventivas**.

---

## 🛠 Tipos de mantenimiento aplicables

### 1. Mantenimiento Correctivo
- **Objetivo:** Corregir errores y vulnerabilidades que afectan la operación normal.  
- **Aplicación en el caso:**  
  - Implementar *rate limiting* para prevenir ataques de fuerza bruta.  
  - Reparar bugs en el proceso de verificación de correo electrónico.  
- **Beneficio esperado:**  
  - Mayor seguridad y confiabilidad en el proceso de autenticación.

---

### 2. Mantenimiento Adaptativo
- **Objetivo:** Ajustar el sistema a nuevos entornos y requisitos.  
- **Aplicación en el caso:**  
  - Integración con **OAuth 2.0** para autenticación social.  
  - Soporte para autenticación biométrica en móviles.  
  - Adaptación a normativas como **GDPR** y **LGPD**.  
- **Beneficio esperado:**  
  - Cumplimiento normativo y mayor flexibilidad de acceso.

---

### 3. Mantenimiento Perfectivo
- **Objetivo:** Mejorar la funcionalidad y experiencia del usuario.  
- **Aplicación en el caso:**  
  - Rediseño de la interfaz para simplificar el registro.  
  - Validación en tiempo real con retroalimentación visual.  
  - Indicadores de fortaleza de contraseña.  
- **Beneficio esperado:**  
  - Incremento en la tasa de conversión y satisfacción del usuario.

---

### 4. Mantenimiento Preventivo
- **Objetivo:** Prevenir futuros problemas y asegurar la mantenibilidad.  
- **Aplicación en el caso:**  
  - Migración hacia arquitectura de **microservicios**.  
  - Implementación de pruebas automatizadas y *logging* estructurado.  
- **Beneficio esperado:**  
  - Mayor escalabilidad y reducción de incidentes en producción.

---

## 📂 Cambios funcionales propuestos
1. Formularios de registro simplificados en un solo paso.  
2. Validación en tiempo real con indicadores visuales.  
3. Integración con redes sociales mediante OAuth 2.0.  
4. Autenticación multifactor (MFA) y biométrica.  
5. Exportación automática de reportes en PDF para usuarios conflictivos.  
6. Migración progresiva hacia microservicios para mejorar escalabilidad.  

---

## 📊 Evaluación del impacto

| Criterio              | Antes del cambio | Después del cambio |
|-----------------------|------------------|--------------------|
| Usabilidad            | Baja             | Alta               |
| Seguridad             | Media            | Alta               |
| Escalabilidad         | Limitada         | Alta               |
| Conversión de registros | 70%             | 90%                |
| Retención de usuarios | 65%              | 80%                |
| Mantenibilidad        | Media            | Alta               |

---

## 🔄 Reflexión sobre el control de versiones
El uso de **Git/GitHub** es esencial para gestionar este proceso de mantenimiento.  
Permite:
- Documentar cada cambio en el código y la base de datos.  
- Coordinar el trabajo en equipo sin sobrescribir avances.  
- Revertir errores y comparar versiones anteriores.  
- Mantener un historial claro de la evolución del sistema.  

En este proyecto, el control de versiones asegura que las mejoras correctivas, adaptativas, perfectivas y preventivas se integren de manera ordenada, garantizando la calidad y sostenibilidad del software.

---

## ✅ Conclusión
La propuesta de mantenimiento permitirá que el **Sistema de Registro de Usuarios** evolucione hacia una solución más segura, escalable y centrada en la experiencia del usuario.  
La combinación de los distintos tipos de mantenimiento, junto con el uso disciplinado de **control de versiones**, asegura que el sistema se mantenga competitivo y preparado para futuras mejoras.

