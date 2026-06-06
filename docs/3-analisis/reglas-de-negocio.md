
**Reglas de Negocio (RN)**

Las reglas de negocio son condiciones que el sistema debe respetar siempre. El campo 'Origen' conecta cada regla con la HU que la motiva.

**RN-01 — Historial de acciones es permanente e inmodificable**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-01 |
| **Título** | Historial de acciones es permanente e inmodificable |
| **Descripción** | El historial de acciones de una solicitud no puede ser modificado ni eliminado por ningún usuario una vez que una acción queda registrada. Esto incluye al Administrador del Sistema. |
| **Origen** | HU-01, HU-11 / Política interna de trazabilidad |

**RN-02 — Reasignación requiere motivo obligatorio**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-02 |
| **Título** | Reasignación requiere motivo obligatorio |
| **Descripción** | Toda reasignación de una solicitud debe incluir obligatoriamente un motivo escrito antes de poder completarse. El sistema no debe permitir reasignaciones sin justificación. |
| **Origen** | HU-03 / Política interna de gestión de solicitudes |

**RN-03 — Resumen mensual generado automáticamente y sin modificación**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-03 |
| **Título** | Resumen mensual generado automáticamente y sin modificación |
| **Descripción** | El resumen mensual del área se genera de forma automática el primer día de cada mes con los datos del mes anterior. Ningún usuario puede modificarlo ni eliminarlo una vez generado. |
| **Origen** | HU-04 / Política interna de reportes |

**RN-04 — Acceso a solicitudes limitado por nivel de permiso**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-04 |
| **Título** | Acceso a solicitudes limitado por nivel de permiso |
| **Descripción** | Cada usuario solo puede ver las solicitudes que corresponden al nivel de acceso que le asignó el Administrador del Sistema. Esta restricción aplica en búsquedas, consultas, historiales y reportes. |
| **Origen** | HU-02, HU-06 / Política interna de seguridad de la información |

**RN-05 — Umbral de días de inactividad configurable y con registro de cambios**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-05 |
| **Título** | Umbral de días de inactividad configurable y con registro de cambios |
| **Descripción** | El número de días máximo sin movimiento que puede tener una solicitud antes de generar una alerta lo define el Administrador del Sistema y puede cambiarse cuando el negocio lo requiera. Cada cambio debe quedar registrado con el nombre de quien lo hizo, la fecha y el valor anterior. |
| **Origen** | HU-08, HU-09 / Política interna de seguimiento de procesos |

**RN-06 — Bitácora de solo lectura con retención mínima obligatoria**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-06 |
| **Título** | Bitácora de solo lectura con retención mínima obligatoria |
| **Descripción** | La bitácora del sistema es de solo lectura para todos los usuarios sin excepción, incluido el Administrador del Sistema. Los registros deben conservarse durante el tiempo mínimo que exija la ley o la política interna. |
| **Origen** | HU-10 / Normativa legal de trazabilidad y auditoría |

**RN-07 — Reporte de rechazadas incluye únicamente solicitudes con ese estado**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-07 |
| **Título** | Reporte de rechazadas incluye únicamente solicitudes con ese estado |
| **Descripción** | Un reporte de solicitudes rechazadas solo puede mostrar solicitudes con estado 'Rechazada'. No puede incluir solicitudes pendientes, en proceso ni aprobadas. |
| **Origen** | HU-12 / Política interna de reportes |

**RN-08 — Archivos adjuntos no pueden eliminarse una vez cargados**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RN-08 |
| **Título** | Archivos adjuntos no pueden eliminarse una vez cargados |
| **Descripción** | Los archivos adjuntos a una solicitud no pueden ser eliminados por ningún usuario una vez cargados al sistema. Solo pueden ser consultados y descargados. |
| **Origen** | HU-05 / Política interna de gestión documental |
