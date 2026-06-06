
**Actores del Sistema**

Los actores son las personas que interactúan con el sistema.

**ACT-01 — Auditor**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID Actor** | ACT-01 |
| **Nombre del Actor** | Auditor |
| **Tipo** | Primario |
| **Descripción** | Persona encargada de revisar que todos los procesos del sistema se hayan llevado a cabo correctamente. |
| **Responsabilidades** | Consultar historial, revisar archivos adjuntos y validar la bitácora. |
| **Permisos / Rol** | Consultor — solo lectura |
| **CU Relacionados** | CU-01, CU-05, CU-10 |
| **HU Relacionadas** | HU-01, HU-05, HU-10 |
| **Restricciones** | No puede crear, modificar ni aprobar solicitudes. |

**ACT-02 — Coordinador**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID Actor** | ACT-02 |
| **Nombre del Actor** | Coordinador |
| **Tipo** | Primario |
| **Descripción** | Persona responsable de gestionar las solicitudes de su área. |
| **Responsabilidades** | Filtrar historial, consultar reasignaciones, ver resumen mensual y exportar registros. |
| **Permisos / Rol** | Gestor — ver, gestionar y exportar solicitudes de su área |
| **CU Relacionados** | CU-02, CU-03, CU-04, CU-11 |
| **HU Relacionadas** | HU-02, HU-03, HU-04, HU-11 |
| **Restricciones** | Solo ve solicitudes de su área salvo permiso ampliado. |

**ACT-03 — Administrativo**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID Actor** | ACT-03 |
| **Nombre del Actor** | Administrativo |
| **Tipo** | Primario |
| **Descripción** | Persona encargada de tareas operativas, como buscar solicitudes rápidamente. |
| **Responsabilidades** | Buscar solicitudes por nombre, fecha o área. |
| **Permisos / Rol** | Consultor — según nivel de acceso asignado |
| **CU Relacionados** | CU-06 |
| **HU Relacionadas** | HU-06 |
| **Restricciones** | Solo ve las solicitudes que su nivel de acceso le permita. |

**ACT-04 — Gerente**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID Actor** | ACT-04 |
| **Nombre del Actor** | Gerente |
| **Tipo** | Primario |
| **Descripción** | Persona con autoridad para supervisar todas las áreas, recibir alertas y generar reportes. |
| **Responsabilidades** | Ver tablero general, recibir avisos de inactividad y generar reportes. |
| **Permisos / Rol** | Consultor general — solo lectura de todas las áreas |
| **CU Relacionados** | CU-07, CU-08, CU-12 |
| **HU Relacionadas** | HU-07, HU-08, HU-12 |
| **Restricciones** | No puede modificar solicitudes ni configurar parámetros. |

**ACT-05 — Administrador del Sistema**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID Actor** | ACT-05 |
| **Nombre del Actor** | Administrador del Sistema |
| **Tipo** | Primario |
| **Descripción** | Persona de soporte que configura parámetros del sistema como días de alerta y permisos. |
| **Responsabilidades** | Definir límite de días de inactividad y asignar nivel de acceso a usuarios. |
| **Permisos / Rol** | Administrador — acceso total a la configuración |
| **CU Relacionados** | CU-09 |
| **HU Relacionadas** | HU-09 |
| **Restricciones** | No puede aprobar ni rechazar solicitudes. |

**Tabla Resumen de Actores**

|     |     |     |     |     |
| --- | --- | --- | --- | --- |
| **ID** | **Nombre** | **Tipo** | **Permisos** | **CU Relacionados** |
| ACT-01 | Auditor | Primario | Consultor — solo lectura | CU-01, CU-05, CU-10 |
| ACT-02 | Coordinador | Primario | Gestor — ver, gestionar y exportar solicitudes de su área | CU-02, CU-03, CU-04, CU-11 |
| ACT-03 | Administrativo | Primario | Consultor — según nivel de acceso asignado | CU-06 |
| ACT-04 | Gerente | Primario | Consultor general — solo lectura de todas las áreas | CU-07, CU-08, CU-12 |
| ACT-05 | Administrador del Sistema | Primario | Administrador — acceso total a la configuración | CU-09 |
