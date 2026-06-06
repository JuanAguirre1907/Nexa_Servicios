
**Casos de uso**

**Diagrama General de Casos de Uso**

Vista general del sistema mostrando todos los actores y su relación con los 12 casos de uso.

<img width="921" height="754" alt="image" src="https://github.com/user-attachments/assets/c539c6ee-7d23-4568-8c71-f31db01948ae" />

**Diagramas Individuales por Caso de Uso**

Cada diagrama muestra el actor que inicia el caso de uso, el ID del caso de uso y su descripción completa dentro del óvalo, siguiendo la notación UML simplificada.

**CU-01 — Consultar historial completo de acciones de una solicitud**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/5cdc08f2-31cd-4fc7-8dff-633e8cb142f6" />

**CU-02 — Filtrar historial de solicitudes**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/ea8afcce-f16e-4b20-acae-6002c541c35d" />

**CU-03 — Consultar historial de reasignaciones de una solicitud**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/849ff3a9-b9b5-453c-ae7f-f54e0218e4bd" />

**CU-04 — Ver resumen mensual automático de solicitudes del área**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/f45a7496-f1f9-42d5-b879-a896fca760f3" />

**CU-05 — Ver archivos adjuntos de una solicitud**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/7120dd4f-0695-4aba-9c67-8b1d5c60ba02" />

**CU-06 — Buscar solicitudes por nombre, fecha o área**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/75d8d778-3daa-4960-a685-1a45cc6abac9" />

**CU-07 — Ver tablero general del estado de todas las áreas**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/0e41c336-3691-4d7a-8ce5-e8d2ae019426" />

**CU-08 — Recibir alerta por solicitud sin movimiento**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/58ca4cce-c898-4097-80d1-d8e99a33f2dd" />

**CU-09 — Configurar días máximos para alertas de inactividad**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/ef27ee62-65e2-4397-ba20-b70bb68e3b50" />

**CU-10 — Consultar la bitácora completa del sistema**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/848d4b9f-3978-4216-bbb0-403d6ceeb82c" />

**CU-11 — Exportar historial en PDF o Excel**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/d7d9b1b4-5a04-4a9f-b37d-7f9bd58521ac" />

**CU-12 — Generar reporte de solicitudes rechazadas**
<img width="938" height="552" alt="image" src="https://github.com/user-attachments/assets/6f031af7-104e-4ba7-9eeb-c0d1340761e1" />

**Descripción de los Casos de Uso**

**CU-01 — Consultar historial completo de acciones de una solicitud**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-01 |
| **Nombre** | Consultar historial completo de acciones de una solicitud |
| **HU Relacionada** | HU-01 |
| **RF que realiza** | RF-01 |
| **RN que aplica** | RN-01 |
| **Actor(es)** | Auditor |
| **Descripción** | El auditor entra a una solicitud y el sistema le muestra todo lo que le ha pasado: quién la creó, quién la tocó, quién la aprobó o rechazó, y exactamente cuándo. |
| **Precondiciones** | El auditor debe haber iniciado sesión. La solicitud debe existir. |
| **Postcondiciones** | El auditor puede ver el historial completo y ordenado. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Auditor | Busca y abre la solicitud que quiere revisar. |
| 2   | Sistema | Muestra el detalle con la sección 'Historial de acciones'. |
| 3   | Auditor | Hace clic en la sección de historial. |
| 4   | Sistema | Muestra la lista completa: quién hizo cada acción, qué tipo fue y en qué fecha y hora. |
| 5   | Auditor | Revisa y verifica que el proceso se siguió correctamente. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Si nunca tuvo movimientos después de crearse, muestra solo el registro de creación. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Solicitud inexistente: 'No se encontró la solicitud'. |
| **FE-02** | Sin permiso: mensaje de acceso no permitido. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Diaria |
| **RN Relacionadas** | RN-01 |
| **Notas / Observaciones** | Principal herramienta de trazabilidad para el equipo auditor. |

**CU-02 — Filtrar historial de solicitudes**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-02 |
| **Nombre** | Filtrar historial de solicitudes |
| **HU Relacionada** | HU-02 |
| **RF que realiza** | RF-02 |
| **RN que aplica** | RN-04 |
| **Actor(es)** | Coordinador |
| **Descripción** | El coordinador aplica filtros sobre el historial para encontrar acciones por persona, fechas o tipo de movimiento. |
| **Precondiciones** | El coordinador debe haber iniciado sesión. Debe haber solicitudes con historial. |
| **Postcondiciones** | El sistema muestra solo los registros que coinciden. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Coordinador | Entra a la sección de historial general. |
| 2   | Sistema | Muestra el historial con opciones de filtro visibles. |
| 3   | Coordinador | Elige filtros: nombre de usuario, rango de fechas o tipo de acción. |
| 4   | Sistema | Muestra únicamente los registros que coinciden. |
| 5   | Coordinador | Revisa los resultados para identificar patrones. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Varios filtros combinados muestran solo registros que cumplen todos. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin resultados: 'No se encontraron resultados para los filtros seleccionados'. |
| **FE-02** | Fecha incorrecta: el sistema avisa y pide corregirlo. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Semanal |
| **RN Relacionadas** | RN-04 |
| **Notas / Observaciones** | Útil para auditorías internas y seguimiento de procesos. |

**CU-03 — Consultar historial de reasignaciones de una solicitud**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-03 |
| **Nombre** | Consultar historial de reasignaciones de una solicitud |
| **HU Relacionada** | HU-03 |
| **RF que realiza** | RF-03 |
| **RN que aplica** | RN-02 |
| **Actor(es)** | Coordinador |
| **Descripción** | El coordinador puede ver la lista de todas las veces que una solicitud fue pasada de una persona a otra, con nombre, fecha y motivo. |
| **Precondiciones** | El coordinador debe haber iniciado sesión. La solicitud debe haber tenido al menos una reasignación. |
| **Postcondiciones** | El coordinador puede ver el historial ordenado de reasignaciones. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Coordinador | Abre la solicitud que quiere revisar. |
| 2   | Sistema | Muestra el detalle con la sección 'Historial de reasignaciones'. |
| 3   | Coordinador | Hace clic en esa sección. |
| 4   | Sistema | Lista cada reasignación: quién la tenía, a quién pasó, cuándo y por qué. |
| 5   | Coordinador | Revisa para identificar cuellos de botella. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Sin reasignaciones: 'Esta solicitud no ha tenido reasignaciones'. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Solicitud inexistente: 'No se encontró la solicitud'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Media |
| **Frecuencia de uso** | Semanal |
| **RN Relacionadas** | RN-02 |
| **Notas / Observaciones** | Permite detectar demoras o pasos innecesarios. |

**CU-04 — Ver resumen mensual automático de solicitudes del área**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-04 |
| **Nombre** | Ver resumen mensual automático de solicitudes del área |
| **HU Relacionada** | HU-04 |
| **RF que realiza** | RF-04 |
| **RN que aplica** | RN-03 |
| **Actor(es)** | Coordinador |
| **Descripción** | El coordinador puede ver un resumen generado automáticamente al inicio de cada mes con todas las solicitudes del área del mes anterior. |
| **Precondiciones** | El coordinador debe haber iniciado sesión. Debe haber al menos un mes completo de solicitudes. |
| **Postcondiciones** | El coordinador consulta el resumen sin necesidad de armarlo manualmente. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Coordinador | Entra a la sección 'Resumen mensual'. |
| 2   | Sistema | Muestra el resumen del mes anterior: totales, aprobadas, rechazadas y pendientes. |
| 3   | Coordinador | Revisa el resumen. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Puede seleccionar un mes anterior y el sistema carga ese resumen. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin solicitudes en el período: 'No hay solicitudes registradas para este período'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Media |
| **Frecuencia de uso** | Mensual |
| **RN Relacionadas** | RN-03 |
| **Notas / Observaciones** | Ahorra tiempo en reportes de gestión. |

**CU-05 — Ver archivos adjuntos de una solicitud**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-05 |
| **Nombre** | Ver archivos adjuntos de una solicitud |
| **HU Relacionada** | HU-05 |
| **RF que realiza** | RF-05 |
| **RN que aplica** | RN-08 |
| **Actor(es)** | Auditor |
| **Descripción** | El auditor puede ver dentro de cada solicitud la lista de archivos cargados: nombre, quién los subió y en qué fecha. |
| **Precondiciones** | El auditor debe haber iniciado sesión. La solicitud debe existir. |
| **Postcondiciones** | El auditor verifica que los archivos requeridos están presentes. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Auditor | Abre la solicitud que quiere revisar. |
| 2   | Sistema | Muestra el detalle con la sección 'Archivos adjuntos'. |
| 3   | Auditor | Hace clic en esa sección. |
| 4   | Sistema | Lista todos los archivos con nombre, quién lo subió y fecha. |
| 5   | Auditor | Verifica que corresponden a las evidencias requeridas. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Puede hacer clic sobre un archivo para abrirlo o descargarlo. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin archivos: 'Esta solicitud no tiene archivos cargados'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Diaria |
| **RN Relacionadas** | RN-08 |
| **Notas / Observaciones** | Fundamental para auditoría y validación de evidencias. |

**CU-06 — Buscar solicitudes por nombre, fecha o área**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-06 |
| **Nombre** | Buscar solicitudes por nombre, fecha o área |
| **HU Relacionada** | HU-06 |
| **RF que realiza** | RF-06 |
| **RN que aplica** | RN-04 |
| **Actor(es)** | Administrativo |
| **Descripción** | El administrativo escribe en una barra de búsqueda y el sistema muestra resultados según el acceso asignado. |
| **Precondiciones** | El administrativo debe haber iniciado sesión. El Administrador debe haber definido su nivel de acceso. |
| **Postcondiciones** | El sistema muestra las solicitudes que coinciden dentro del alcance del usuario. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Administrativo | Entra a la sección de búsqueda general. |
| 2   | Sistema | Muestra la barra de búsqueda y los filtros disponibles. |
| 3   | Administrativo | Escribe nombre, fecha o área y hace clic en 'Buscar'. |
| 4   | Sistema | Filtra los resultados según lo escrito y el nivel de acceso. |
| 5   | Administrativo | Revisa y abre la solicitud que necesita. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Con acceso parcial, el sistema muestra solo las áreas permitidas. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin resultados: 'No se encontraron solicitudes con esa información'. |
| **FE-02** | Sin permiso: 'No tienes permiso para ver esta solicitud'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Diaria |
| **RN Relacionadas** | RN-04 |
| **Notas / Observaciones** | El control de acceso lo gestiona el Administrador del Sistema. |

**CU-07 — Ver tablero general del estado de todas las áreas**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-07 |
| **Nombre** | Ver tablero general del estado de todas las áreas |
| **HU Relacionada** | HU-07 |
| **RF que realiza** | RF-07 |
| **RN que aplica** | —   |
| **Actor(es)** | Gerente |
| **Descripción** | El gerente puede ver en una sola pantalla cuántas solicitudes tiene cada área, en qué estado están y si hay alertas. |
| **Precondiciones** | El gerente debe haber iniciado sesión. Debe haber solicitudes en al menos un área. |
| **Postcondiciones** | El gerente tiene vista completa del estado de todas las áreas. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Gerente | Entra al sistema y va al tablero general. |
| 2   | Sistema | Carga el resumen de todas las áreas: totales, estados y alertas activas. |
| 3   | Gerente | Revisa el tablero para identificar problemas. |
| 4   | Gerente | Si quiere detalle de un área, hace clic sobre ella. |
| 5   | Sistema | Muestra el listado de solicitudes de esa área. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Puede elegir una fecha pasada para ver el estado de las áreas en ese momento. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin solicitudes: 'No hay solicitudes registradas todavía'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Diaria |
| **RN Relacionadas** | —   |
| **Notas / Observaciones** | Da visibilidad inmediata sin depender de reportes manuales. |

**CU-08 — Recibir alerta cuando una solicitud lleva demasiado tiempo sin movimiento**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-08 |
| **Nombre** | Recibir alerta cuando una solicitud lleva demasiado tiempo sin movimiento |
| **HU Relacionada** | HU-08 |
| **RF que realiza** | RF-08 |
| **RN que aplica** | RN-05 |
| **Actor(es)** | Gerente |
| **Descripción** | El sistema revisa cada día si alguna solicitud supera el límite de días sin atención y avisa al gerente. |
| **Precondiciones** | El Administrador debe haber configurado el límite de días. El gerente debe tener notificaciones activas. |
| **Postcondiciones** | El gerente recibe el aviso con nombre, días quieta y responsable. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Sistema | Cada día a hora fija, revisa solicitudes activas sin movimiento. |
| 2   | Sistema | Compara días quietos con el límite configurado. |
| 3   | Sistema | Si alguna supera el límite, genera un aviso para el gerente. |
| 4   | Gerente | Recibe el aviso en pantalla o por correo. |
| 5   | Gerente | Revisa la situación y decide si interviene. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Varias solicitudes con retraso se agrupan en un solo aviso. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin límite configurado: aviso indicando que falta esa configuración. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Diaria (automático) |
| **RN Relacionadas** | RN-05 |
| **Notas / Observaciones** | La alerta es preventiva, no bloquea el proceso. |

**CU-09 — Configurar el número de días máximo para alertas de inactividad**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-09 |
| **Nombre** | Configurar el número de días máximo para alertas de inactividad |
| **HU Relacionada** | HU-09 |
| **RF que realiza** | RF-09 |
| **RN que aplica** | RN-05 |
| **Actor(es)** | Administrador del Sistema |
| **Descripción** | El Administrador define cuántos días puede estar una solicitud sin movimiento antes de que el sistema avise al gerente. |
| **Precondiciones** | El administrador debe haber iniciado sesión con cuenta de administración. |
| **Postcondiciones** | El sistema aplica el nuevo límite desde la próxima revisión automática. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Administrador del Sistema | Entra a la sección de configuración del sistema. |
| 2   | Sistema | Muestra la configuración actual con el límite de días vigente. |
| 3   | Administrador del Sistema | Cambia el número de días y guarda. |
| 4   | Sistema | Confirma el cambio y registra quién lo hizo, cuándo y el valor anterior. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Puede configurar umbrales distintos para diferentes áreas. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Valor cero o negativo: 'El número de días debe ser mayor a cero'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Ocasional |
| **RN Relacionadas** | RN-05 |
| **Notas / Observaciones** | Base que hace funcionar CU-08. |

**CU-10 — Consultar la bitácora completa de acciones del sistema**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-10 |
| **Nombre** | Consultar la bitácora completa de acciones del sistema |
| **HU Relacionada** | HU-10 |
| **RF que realiza** | RF-10 |
| **RN que aplica** | RN-06 |
| **Actor(es)** | Auditor |
| **Descripción** | El auditor consulta el registro completo de todo lo que ha pasado en el sistema, con usuario, fecha y hora. No puede modificarse ni borrarse. |
| **Precondiciones** | El auditor debe haber iniciado sesión. El sistema debe llevar registro continuo. |
| **Postcondiciones** | El auditor puede ver la bitácora completa y verificar la trazabilidad. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Auditor | Entra a la sección 'Bitácora del sistema'. |
| 2   | Sistema | Muestra el registro completo de lo más reciente a lo más antiguo. |
| 3   | Auditor | Aplica filtros por fecha, usuario o tipo de acción. |
| 4   | Sistema | Muestra los registros que coinciden. |
| 5   | Auditor | Revisa para verificar que todo ocurrió correctamente. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Puede exportar la bitácora filtrada en PDF o Excel. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin resultados: 'No se encontraron registros para los criterios seleccionados'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Alta |
| **Frecuencia de uso** | Semanal / según necesidad |
| **RN Relacionadas** | RN-06 |
| **Notas / Observaciones** | La inmutabilidad y retención mínima son obligatorias. |

**CU-11 — Exportar el historial de una solicitud en PDF o Excel**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-11 |
| **Nombre** | Exportar el historial de una solicitud en PDF o Excel |
| **HU Relacionada** | HU-11 |
| **RF que realiza** | RF-11 |
| **RN que aplica** | RN-01 |
| **Actor(es)** | Coordinador |
| **Descripción** | El coordinador descarga el historial completo de una solicitud en PDF o Excel para usarlo como evidencia. |
| **Precondiciones** | El coordinador debe haber iniciado sesión. La solicitud debe existir y tener historial. |
| **Postcondiciones** | El coordinador tiene el archivo descargado en el formato elegido. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Coordinador | Abre la solicitud cuyo historial quiere exportar. |
| 2   | Sistema | Muestra el detalle con el botón 'Exportar historial'. |
| 3   | Coordinador | Hace clic en 'Exportar historial'. |
| 4   | Sistema | Muestra las opciones: PDF o Excel. |
| 5   | Coordinador | Elige el formato. |
| 6   | Sistema | Genera el archivo y lo descarga automáticamente. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | En Excel, cada acción aparece en una fila separada. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin historial: 'No hay historial disponible para exportar'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Media |
| **Frecuencia de uso** | Ocasional |
| **RN Relacionadas** | RN-01 |
| **Notas / Observaciones** | PDF para presentaciones formales; Excel para análisis. |

**CU-12 — Generar reporte de solicitudes rechazadas en un período**

1\. Identificación del Caso de Uso

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | CU-12 |
| **Nombre** | Generar reporte de solicitudes rechazadas en un período |
| **HU Relacionada** | HU-12 |
| **RF que realiza** | RF-12 |
| **RN que aplica** | RN-07 |
| **Actor(es)** | Gerente |
| **Descripción** | El gerente genera un reporte con las solicitudes rechazadas en un período elegido, con motivo, quién rechazó y cuándo. |
| **Precondiciones** | El gerente debe haber iniciado sesión. Debe haber al menos una solicitud rechazada. |
| **Postcondiciones** | El gerente tiene el reporte listo para revisar. |

2\. Flujo Principal (lo que pasa cuando todo sale bien)

|     |     |     |
| --- | --- | --- |
| **Paso** | **Actor** | **Acción** |
| 1   | Gerente | Entra a la sección 'Reportes'. |
| 2   | Sistema | Muestra las opciones de reportes disponibles. |
| 3   | Gerente | Selecciona 'Reporte de rechazadas' y elige fechas de inicio y fin. |
| 4   | Sistema | Genera el reporte con nombre, motivo, quién rechazó y cuándo. |
| 5   | Gerente | Revisa para identificar patrones. |

3\. Flujos Alternativos (variaciones válidas del proceso)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FA-01** | Puede descargarlo en PDF o Excel. |

4\. Flujos de Excepción (qué pasa cuando algo falla)

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **FE-01** | Sin rechazos: 'No se encontraron solicitudes rechazadas para ese período'. |
| **FE-02** | Período inválido: 'El período seleccionado no es válido'. |

5\. Información Adicional

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **Prioridad** | Media |
| **Frecuencia de uso** | Mensual / Ocasional |
| **RN Relacionadas** | RN-07 |
| **Notas / Observaciones** | Herramienta clave para mejora continua de procesos. |
