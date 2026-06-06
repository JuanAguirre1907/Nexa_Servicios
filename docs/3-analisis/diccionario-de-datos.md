| Entidad        | Atributo             | Tipo      | Descripción                                | Restricciones                                                | Ejemplo                 |
|----------------|----------------------|-----------|--------------------------------------------|--------------------------------------------------------------|-------------------------|
| Solicitud      | id_solicitud         | Entero    | Identificador único de la solicitud        | Autoincrement, no nulo                                       | 102                     |
|                | fecha_creacion       | Fecha     | Fecha en que se creó la solicitud          | No nulo                                                      | 6/5/26                  |
|                | estado               | Texto     | Estado actual de la solicitud              | Pendiente, En proceso, Aprobada, Rechazada                   | Aprobada                |
|                | area                 | Texto     | Área responsable de la solicitud           | Valores definidos por organización                           | Finanzas                |
| Historial      | id_historial         | Entero    | Identificador único del registro de acción | Autoincrement, no nulo                                       | 5501                    |
|                | id_solicitud         | Entero    | Relación con la solicitud                  | Referencia a Solicitud                                       | 102                     |
|                | accion               | Texto     | Acción realizada sobre la solicitud        | Crear, Aprobar, Rechazar, Modificar                          | Aprobar                 |
|                | usuario              | Entero    | Usuario que ejecutó la acción              | Referencia a Usuario, no nulo                                | 501                     |
|                | fecha_hora           | FechaHora | Momento exacto de la acción                | No nulo                                                      | 6/5/26 14:32            |
| Reasignación   | id_reasignacion      | Entero    | Identificador único de la reasignación     | Autoincrement                                                | 3002                    |
|                | id_solicitud         | Entero    | Relación con la solicitud                  | Referencia a Solicitud                                       | 102                     |
|                | responsable_anterior | Entero    | Usuario que tenía la solicitud antes       | Referencia a Usuario                                         | 502                     |
|                | responsable_nuevo    | Entero    | Usuario que recibe la solicitud            | Referencia a Usuario                                         | 503                     |
|                | motivo               | Texto     | Justificación de la reasignación           | Obligatorio                                                  | “Carga de trabajo alta” |
| ArchivoAdjunto | id_archivo           | Entero    | Identificador único del archivo            | Autoincrement                                                | 7001                    |
|                | id_solicitud         | Entero    | Relación con la solicitud                  | Referencia a Solicitud                                       | 102                     |
|                | nombre_archivo       | Texto     | Nombre del archivo adjunto                 | No nulo                                                      | contrato.pdf            |
|                | usuario_subida       | Entero    | Usuario que subió el archivo               | Referencia a Usuario                                         | 501                     |
|                | fecha_subida         | Fecha     | Fecha en que se cargó el archivo           | No nulo                                                      | 6/5/26                  |
| Bitácora       | id_evento            | Entero    | Identificador único del evento             | Autoincrement                                                | 9001                    |
|                | descripcion_evento   | Texto     | Detalle de la acción registrada            | Solo lectura                                                 | “Inicio de sesión”      |
|                | usuario              | Entero    | Usuario que ejecutó la acción              | Referencia a Usuario                                         | 501                     |
|                | fecha_hora           | FechaHora | Momento exacto del evento                  | No nulo                                                      | 6/5/26 9:15             |
| Usuario        | id_usuario           | Entero    | Identificador único del usuario            | Autoincrement                                                | 501                     |
|                | nombre               | Texto     | Nombre completo del usuario                | No nulo                                                      | Juan Pérez              |
|                | rol                  | Texto     | Rol asignado en el sistema                 | Auditor, Coordinador, Administrativo, Gerente, Administrador | Gerente                 |
| Alerta         | id_alerta            | Entero    | Identificador único de la alerta           | Autoincrement                                                | 8001                    |
|                | id_solicitud         | Entero    | Solicitud asociada a la alerta             | Referencia a Solicitud                                       | 102                     |
|                | dias_inactividad     | Entero    | Número de días sin movimiento              | Configurable por Administrador                               | 5                       |
| Reporte        | id_reporte           | Entero    | Identificador único del reporte            | Autoincrement                                                | 6001                    |
|                | tipo_reporte         | Texto     | Tipo de reporte generado                   | Mensual, Rechazadas, Exportación                             | Rechazadas              |
|                | periodo              | Texto     | Rango de fechas del reporte                | Formato AAAA-MM-DD a AAAA-MM-DD                              | 2026-05-01 a 2026-05-31 |
