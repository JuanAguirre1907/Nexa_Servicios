
**Requisitos Funcionales (RF)**

Cada RF describe una sola acción concreta y verificable. Se indica el CU que lo modela y la RN que aplica para trazabilidad completa en ambos sentidos.

**RF-01 — Relacionado con HU-01**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-01 |
| **HU Relacionada** | HU-01 |
| **Descripción** | Cuando alguien con rol de auditor abra una solicitud, el sistema debe mostrarle una lista con todo lo que le ha pasado desde que fue creada: quién la abrió, quién la tocó, quién la aprobó o la rechazó, y en qué día y a qué hora pasó cada cosa. Nada puede faltar ni estar oculto. |
| **CU que lo modela** | CU-01 |
| **RN que aplica** | RN-01 |

**RF-02 — Relacionado con HU-02**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-02 |
| **HU Relacionada** | HU-02 |
| **Descripción** | El sistema debe tener una opción de búsqueda en el historial donde el coordinador pueda elegir filtrar por el nombre de una persona, por un rango de fechas, o por el tipo de acción que se realizó (crear, aprobar, rechazar, modificar, etc.). Los resultados deben aparecer solo con lo que coincida con lo elegido. |
| **CU que lo modela** | CU-02 |
| **RN que aplica** | RN-04 |

**RF-03 — Relacionado con HU-03**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-03 |
| **HU Relacionada** | HU-03 |
| **Descripción** | Dentro de cada solicitud debe existir una sección que muestre, en orden cronológico, todas las veces que fue pasada de una persona a otra. Por cada cambio debe verse el nombre de quien la tenía antes, el nombre de quien la recibió, la fecha en que ocurrió y el motivo del cambio. |
| **CU que lo modela** | CU-03 |
| **RN que aplica** | RN-02 |

**RF-04 — Relacionado con HU-04**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-04 |
| **HU Relacionada** | HU-04 |
| **Descripción** | Al inicio de cada mes, el sistema debe generar automáticamente un resumen con todas las solicitudes que se movieron en el área del coordinador durante el mes anterior. Ese resumen debe estar listo para consultarse sin que el coordinador tenga que hacer nada, solo entrar y verlo. |
| **CU que lo modela** | CU-04 |
| **RN que aplica** | RN-03 |

**RF-05 — Relacionado con HU-05**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-05 |
| **HU Relacionada** | HU-05 |
| **Descripción** | En cada solicitud debe haber una sección que liste todos los archivos que le fueron adjuntados. Por cada archivo debe verse su nombre, el nombre de la persona que lo subió y la fecha en que fue cargado al sistema. |
| **CU que lo modela** | CU-05 |
| **RN que aplica** | RN-08 |

**RF-06 — Relacionado con HU-06**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-06 |
| **HU Relacionada** | HU-06 |
| **Descripción** | El sistema debe tener una barra de búsqueda donde cualquier usuario autorizado pueda escribir el nombre de una solicitud, una fecha o el nombre de un área, y ver de inmediato los resultados que coincidan. El sistema mostrará únicamente las solicitudes que el usuario tiene permitido ver, según el acceso que tenga asignado. |
| **CU que lo modela** | CU-06 |
| **RN que aplica** | RN-04 |

**RF-07 — Relacionado con HU-07**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-07 |
| **HU Relacionada** | HU-07 |
| **Descripción** | El sistema debe tener un tablero general donde el gerente pueda ver, de un solo vistazo, cuántas solicitudes tiene cada área, en qué estado están (pendientes, en proceso, aprobadas, rechazadas) y si algún área tiene alertas o retrasos. Todo en una sola pantalla sin tener que entrar a cada área por separado. |
| **CU que lo modela** | CU-07 |
| **RN que aplica** | —   |

**RF-08 — Relacionado con HU-08**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-08 |
| **HU Relacionada** | HU-08 |
| **Descripción** | El sistema debe revisar automáticamente cada día si alguna solicitud lleva quieta más días de los permitidos y, si encuentra alguna, enviará un aviso al gerente indicando el nombre de la solicitud, cuántos días lleva sin moverse y quién es el responsable de atenderla. |
| **CU que lo modela** | CU-08 |
| **RN que aplica** | RN-05 |

**RF-09 — Relacionado con HU-09**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-09 |
| **HU Relacionada** | HU-09 |
| **Descripción** | El sistema debe permitir que el Administrador del Sistema defina cuántos días pueden pasar antes de que una solicitud sin movimiento se considere un retraso. Ese número puede ajustarse en cualquier momento. Cada vez que se cambie, el sistema guarda quién lo hizo, cuándo y cuál era el valor anterior. |
| **CU que lo modela** | CU-09 |
| **RN que aplica** | RN-05 |

**RF-10 — Relacionado con HU-10**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-10 |
| **HU Relacionada** | HU-10 |
| **Descripción** | El sistema debe llevar un registro continuo de todo lo que ocurre dentro de él: entradas, cambios, aprobaciones y rechazos. Por cada evento debe quedar guardado el nombre del usuario, la fecha y la hora exacta. Este registro no puede ser modificado ni eliminado por nadie, ni siquiera por los administradores. Además, debe conservarse durante el tiempo que exija la ley o la política interna. |
| **CU que lo modela** | CU-10 |
| **RN que aplica** | RN-06 |

**RF-11 — Relacionado con HU-11**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-11 |
| **HU Relacionada** | HU-11 |
| **Descripción** | Dentro de cada solicitud debe haber un botón que permita al coordinador descargar todo el historial. El sistema debe ofrecer elegir entre PDF o Excel, y el archivo descargado debe contener la misma información completa que se ve en pantalla. |
| **CU que lo modela** | CU-11 |
| **RN que aplica** | RN-01 |

**RF-12 — Relacionado con HU-12**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RF-12 |
| **HU Relacionada** | HU-12 |
| **Descripción** | El sistema debe tener una opción para que el gerente elija un período (fecha de inicio y fecha de fin) y genere un listado con todas las solicitudes rechazadas en ese período. Por cada una debe verse el motivo del rechazo, quién la rechazó y cuándo. |
| **CU que lo modela** | CU-12 |
| **RN que aplica** | RN-07 |
