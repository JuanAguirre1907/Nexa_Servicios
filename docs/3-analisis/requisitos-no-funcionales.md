
**Requisitos No Funcionales (RNF)**

Los RNF describen cómo debe comportarse el sistema. Cada uno incluye una métrica concreta y verificable.

**RNF-01 — Seguridad**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RNF-01 |
| **Categoría** | Seguridad |
| **Descripción** | El sistema debe garantizar que solo las personas con usuario y contraseña activos puedan entrar, y que cada persona solo pueda ver y hacer lo que su rol le permite. |
| **Métrica** | El 100% de los intentos de acceso sin credenciales válidas deben ser bloqueados. Un usuario con rol de auditor no debe poder ejecutar acciones de aprobación en ninguna prueba realizada. |

**RNF-02 — Disponibilidad**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RNF-02 |
| **Categoría** | Disponibilidad |
| **Descripción** | El sistema debe estar disponible para usarse durante el horario laboral de la organización sin interrupciones no programadas. |
| **Métrica** | El sistema debe estar disponible al menos el 99% del tiempo en días hábiles entre 7:00 a.m. y 7:00 p.m. Máximo 1 hora de caída no programada al mes. |

**RNF-03 — Rendimiento**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RNF-03 |
| **Categoría** | Rendimiento |
| **Descripción** | El sistema debe responder rápido. Las búsquedas y consultas no deben hacer esperar al usuario más de lo necesario. |
| **Métrica** | Las búsquedas y carga de historiales deben mostrar resultados en menos de 3 segundos con hasta 50 usuarios conectados al mismo tiempo. |

**RNF-04 — Usabilidad**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RNF-04 |
| **Categoría** | Usabilidad |
| **Descripción** | El sistema debe ser fácil de usar sin necesitar capacitación extensa. Cualquier persona con manejo básico de computador debe poder usarlo desde el primer día. |
| **Métrica** | Un usuario nuevo debe poder completar una búsqueda o consulta de historial sin ayuda después de una explicación de máximo 15 minutos. |

**RNF-05 — Portabilidad**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RNF-05 |
| **Categoría** | Portabilidad |
| **Descripción** | El sistema debe funcionar correctamente desde cualquier navegador de internet moderno, sin necesidad de instalar programas adicionales. |
| **Métrica** | El sistema debe funcionar sin errores en Chrome, Firefox, Edge y Safari en sus versiones lanzadas en los últimos 2 años, tanto en computador como en tableta. |

**RNF-06 — Rendimiento**

|     |     |
| --- | --- |
| **Campo** | **Descripción** |
| **ID** | RNF-06 |
| **Categoría** | Rendimiento |
| **Descripción** | El sistema debe poder actualizarse o corregirse sin que los datos históricos se pierdan ni se dañen. |
| **Métrica** | Después de cualquier actualización, el 100% de los historiales, bitácoras y registros anteriores deben seguir accesibles e intactos, verificable mediante prueba de consulta posterior. |
