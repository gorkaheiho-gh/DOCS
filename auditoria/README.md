# Auditoría

## MIA · Auditoría Técnica Integral — Prompt/Proceso v1.0

[Abrir el documento](MIA_Auditoria_Tecnica_Integral_Prompt_Proceso_v1.0.md)

- **Versión:** 1.0
- **Última actualización:** septiembre 2026

### Qué es

Un prompt para que un agente de IA, con acceso autorizado al repositorio y a
herramientas de desarrollo, haga una revisión técnica integral de un producto
software.

Más que un prompt, es la especificación de un proceso que el agente puede
ejecutar. El agente no se limita a buscar errores de programación: actúa como
un equipo de auditoría completo. Evalúa el estado real del producto, documenta
lo que encuentra con evidencias, prioriza y, si se le autoriza, corrige y
vuelve a auditar.

### Qué define

| Aspecto | Contenido | Sección |
|---|---|---|
| Perfiles | Diez especialidades: arquitectura, seguridad, datos, DevOps, pruebas, rendimiento, accesibilidad, IA… | 0 |
| Alcance | Datos del encargo que hay que completar y cómo tratar los que falten | 1–2 |
| Referencias | ISO/IEC 25010, OWASP (ASVS, Top 10, LLM, agéntico), NIST SSDF y SP 800-218A, SLSA, WCAG 2.2, RGPD, ENS… | 3 |
| Restricciones | Línea base, solo lectura durante el diagnóstico, gestión de secretos, evidencias, reproducibilidad | 4 |
| Entregables | Estructura documental en `docs/audit/[AAAA-MM-DD]/` | 5 |
| Fases | Inventario, construcción, análisis automático, revisión manual y auditoría de IA y agentes | 6–10 |
| Severidad y prioridad | Identificadores `AUD-[ÁREA]-[NÚMERO]`, severidad de Crítica a Oportunidad, CVSS 4.0 solo para seguridad, prioridad de P0 a P4 | 11 |
| Madurez | Escala de 0 a 5 por área, sin una media global que oculte riesgos | 12 |
| Arquitectura objetivo y hoja de ruta | ADR propuestos y horizontes de contención inmediata, 30 días, 90 días, 3–6 meses y largo plazo | 13–14 |
| Permisos para corregir | Qué puede corregirse automáticamente y qué requiere aprobación humana | 15 |
| Criterios de aceptación | Cuándo un hallazgo puede darse por resuelto y estados permitidos | 16 |
| Reauditoría | Comparación antes/después e informe de cierre | 17 |
| Formato de salida | Resumen ejecutivo, `findings.json`, CSV y orden obligatorio de ejecución | 18–22 |

### Modos de ejecución

| Modo | Qué permite |
|---|---|
| `SOLO_AUDITORÍA` | Diagnóstico sin modificar el código |
| `AUDITORÍA_Y_CORRECCIONES_SEGURAS` | Correcciones acotadas: errores confirmados, pruebas, validaciones, documentación… |
| `AUDITORÍA_CORRECCIÓN_COMPLETA` | Corrección más amplia, siempre sujeta a la lista de acciones que requieren aprobación |

Aunque se autorice la corrección completa, hay cambios que siempre necesitan
aprobación explícita: arquitectura, autenticación y autorización, migraciones
destructivas, rotación de secretos, borrado de datos, infraestructura de
producción, despliegues y operaciones con coste.

### Cómo usarlo

1. Copia el documento en la conversación con el agente.
2. Completa los datos de la sección 1 (producto, repositorio, rama, datos
   tratados, componentes de IA…). Si falta alguno, el agente lo deduce y lo
   registra como hipótesis.
3. Elige el modo de ejecución.
4. Revisa el informe después de cada fase. El agente debe informar sobre la
   marcha y no guardarse los resultados importantes para el final.

### Importante

Esta revisión no sustituye una auditoría independiente, una certificación, un
análisis jurídico ni una prueba de penetración profesional.
