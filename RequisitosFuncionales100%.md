# Requisitos Funcionales

## Resumen de clasificación

| Criterio | Número | Porcentaje (%) | Total de requisitos |
|:---|---:|---:|---:|
| Requisitos que impactan al negocio | 15 | 32.61 | 46 |
| Requisitos que son retos tecnológicos | 2 | 4.35 | 46 |

## Catálogo de requisitos funcionales

| ID | Descripción | ¿Impacta al negocio? | ¿Es un reto tecnológico? | ¿Por qué? |
|:---|:---|:---:|:---:|:---|
| RF-01 | El sistema debe permitir registrar usuarios con nombre, apellido, correo y contraseña | No | No | Es genérico, es un problema ya resuelto |
| RF-02 | El sistema debe permitir iniciar sesión con usuario y contraseña al sistema | No | No | Es genérico, es un problema ya resuelto |
| RF-03 | El sistema debe permitir cerrar sesión | No | No | Es genérico, es un problema ya resuelto |
| RF-04 | El sistema debe permitir recuperar la contraseña en caso de que el usuario la haya olvidado | No | No | Es genérico, es un problema ya resuelto |
| RF-05 | El sistema debe permitirle a un usuario consultar su propia información | No | No | Es genérico, es un problema ya resuelto |
| RF-06 | El sistema debe permitirle al usuario eliminar su cuenta | No | No | Es genérico, es un problema ya resuelto |
| RF-07 | El sistema debe permitirle al usuario actualizar sus datos | No | No | Es genérico, es un problema ya resuelto |
| RF-08 | El sistema debe permitir crear publicaciones con producto, tipo (Compra/intercambio), nombre, descripción, fotos y ciudad | Sí | No | Es nuestra propuesta de valor principal |
| RF-09 | El sistema debe permitir editar cualquier apartado de una publicación creada | No | No | Es una funcionalidad genérica |
| RF-10 | El sistema debe permitir visualizar las publicaciones | No | No | Es una funcionalidad genérica |
| RF-11 | El sistema debe permitir eliminar publicaciones | No | No | CRUD genérico, sin valor diferencial ni dificultad técnica. |
| RF-12 | El sistema debe permitir filtrar las publicaciones por parámetros como ciudad, precio o categoría | Sí | No | Filtrar por ciudad es importante para la idea de negocio |
| RF-13 | El sistema debe permitir agregar productos a una lista de favoritos | No | No | Es una funcionalidad genérica |
| RF-14 | El sistema debe permitir realizar propuestas de intercambio con producto, valor, encime y lugar | Sí | No | Es nuestro motor principal de generación de valor |
| RF-15 | El sistema debe permitir realizar contraofertas a un intercambio propuesto | Sí | No | Es parte del posible flujo de los intercambios |
| RF-16 | El sistema debe verificar que un usuario no se haga una propuesta de intercambio o se compre a sí mismo | No | No | Es una verificación básica |
| RF-17 | El sistema debe marcar una publicación como no disponible luego de que se finalice una compra o intercambio de la misma | No | No | Es algo genérico |
| RF-18 | El sistema debe permitir aceptar o rechazar propuestas de intercambio | Sí | No | Porque permite fomalizar el intercambio, que es parte fundamental del negocio |
| RF-19 | El sistema debe permitir comprarle un producto directamente al vendedor | Sí | No | Es la función principal de uno de nuestros segmentos |
| RF-20 | El sistema debe permitir pagar el encime de un intercambio a través de una pasarela | Sí | No | Aquí se garantiza que el dinero pase por la plataforma, asegurando la monetización de la misma |
| RF-21 | El sistema debe retener el dinero de una compra o intercambio hasta la confirmación de entrega por parte de ambos miembros | Sí | Sí | Es un proceso importantísimo de seguridad que le da confianza al cliente. Es un reto porque se necesita hacer una buena integración con las reglas de negocio y estados para que el sistema no se corrompa |
| RF-22 | El sistema debe liberar el dinero hacia el vendedor/persona con el objeto de mayor valor en un intercambio luego de la confirmación de entrega por parte de ambos miembros | Sí | Sí | Es parte del cierre financiero del intercambio y tiene una parte importante de complejidad de las reglas de negocio |
| RF-23 | El sistema debe calcular la comisión del valor de la compra o encime de un intercambio | No | No | Es lógica de las comisiones que se hayan tomado de forma matemática |
| RF-24 | El sistema debe permitir suscribirse a uno de los planes premium que ofrece la plataforma pagando a través de una pasarela de pago | No | No | Es un patrón freemium estándar, ya está establecido |
| RF-25 | El sistema debe permitir crear nuevos planes de suscripción | No | No | Es un CRUD simple desde la parte administrativa |
| RF-26 | El sistema debe permitir cancelar su suscripción a un plan premium | No | No | Es una funcionalidad de gestión de cuenta genérica |
| RF-27 | El sistema debe permitir pagar una insignia de verificación por medio de una pasarela de pago | No | No | No se necesita implementar una pasarela de pago, solo integrarla |
| RF-28 | El sistema debe priorizar en los resultados de búsqueda y listados las publicaciones de usuarios con un plan premium activo. | No | No | Es una regla de ordenamiento que puede seguir algoritmos ya creados y probados |
| RF-29 | El sistema debe notificarle al usuario por medio de correo electrónico que hay nuevos mensajes en un chat | No | No | Es un patrón estándar de notificaciones, hay soluciones ya creadas y no es nuestro diferencial competidor |
| RF-30 | El sistema debe notificarle al usuario por medio de correo electrónico propuestas de intercambio o compra | No | No | Es un patrón estándar de notificaciones, hay soluciones ya creadas y no es nuestro diferencial competidor |
| RF-31 | El sistema debe permitir iniciar un chat con el dueño de una publicación para aclarar detalles de la negociación | No | No | Es una funcionalidad básica no inherente a la generación de valor del proyecto, además de que es un problema ya solucionado y probado ampliamente |
| RF-32 | El sistema debe permitir enviar mensajes en un chat | No | No | Es una funcionalidad básica no inherente a la generación de valor del proyecto, además de que es un problema ya solucionado y probado ampliamente |
| RF-33 | El sistema debe permitir calificar a un usuario luego de un intercambio o compra en una escala numérica de 1 a 5 | Sí | No | Es una funcionalidad que aumenta la cantidad de datos para la reputación de un usuario, lo que es importante para cumplir con la promesa de confianza de la plataforma |
| RF-34 | El sistema debe permitir al usuario acceder a su historial de compras e intercambios finalizados o en curso con el estado en que se encuentre | No | No | Es una funcionalidad básica que no genera valor al negocio y no tiene una gran complejidad de implementación |
| RF-35 | El sistema debe permitir acceder al historial de intercambios de cualquier usuario | Sí | No | Es una funcionalidad importante para cumplir con la promesa de confianza del proyecto |
| RF-36 | El sistema debe permitir consultar la reputación de un usuario | Sí | No | Es la manera en que un usuario puede tener o no confianza en realizar una compra/intercambio con otro |
| RF-37 | El sistema debe permitir reportar publicaciones con contenido inapropiado o engañoso | No | No | Es una moderación genérica presente en cualquier plataforma |
| RF-38 | El sistema debe permitir reportar usuarios por incumplir las normas de la plataforma | No | No | Mismo caso, funcionalidad de moderación genérica. |
| RF-39 | El sistema debe permitir visualizar los reportes a los administradores | No | No | Es una herramienta administrativa interna, consulta simple. |
| RF-40 | El sistema debe permitir a los administradores marcar al usuario responsable de una publicación o comportamiento inapropiado en chat con un strike. | No | No | Es una moderación genérica y sin mucha complejidad técnica |
| RF-41 | El sistema debe permitir a cada parte de un intercambio o compra confirmar que la entrega presencial fue completada exitosamente. | Sí | No | Es la función final del flujo completo de una compra/intercambio en la plataforma, permite confirmar que todo salió bien |
| RF-42 | El sistema debe permitir cancelar una propuesta de intercambio o compra antes de su confirmación final. | Sí | No | Es una función que le da control al usuario de la negociación, lo que le da cierta tolerancia a fallos en su decisión |
| RF-43 | El sistema debe reembolsar el dinero retenido de una compra o intercambio si este se cancela antes de la confirmación de entrega. | Sí | No | Es una función que protege el dinero si el encuentro no se lleva a cabo o no se concreta, de vital importancia para la seguridad de los usuarios; en este caso la pasarela ya tiene la solución implementada |
| RF-44 | El sistema debe permitir consultar la lista de publicaciones marcadas como favoritas por el usuario. | No | No | Es una funcionalidad genérica, parte de un CRUD, no aporta valor al negocio |
| RF-45 | El sistema debe permitir eliminar una publicación de la lista de favoritos del usuario. | No | No | Es una funcionalidad genérica, parte de un CRUD, no aporta valor al negocio |
| RF-46 | El sistema debe permitir a los administradores cerrar la cuenta de un usuario responsable de una publicación o comportamiento inapropiado en chat. | No | No | Es una accción administrativa estándar que no aporta valor de negocio |

## Funcionalidades críticas

### RF-14

**Funcionalidad crítica:** El sistema debe permitir realizar propuestas de intercambio con producto, valor, encime y lugar

**Justificación:** Es crítica porque materializa el dominio de negocio de nuestro proyecto: La negociación de intercambios. Permite iniciar una operación especificando los productos que serán negociados y constituye el punto de partida del flujo principal de generación de valor de la plataforma.

### RF-15

**Funcionalidad crítica:** El sistema debe permitir realizar contraofertas a un intercambio propuesto

**Justificación:** Es crítica porque forma parte directamente del mecanismo de negociación que diferencia al proyecto de un marketplace convencional. Permitir contraofertas hace posible que el intercambio sea dinámico y no se limite a una propuesta de compra de un solo lado.

### RF-19

**Funcionalidad crítica:** El sistema debe permitir comprarle un producto directamente al vendedor

**Justificación:** Es crítica porque, aunque la compra directa es un segmento secundario del negocio, reutiliza el mecanismo económico mediante el cual se obtienen ingresos. La comisión se calcula sobre el dinero que pasa por la plataforma, por lo que esta funcionalidad condiciona capacidades relacionadas con pagos, comisiones y ciclo de vida de la operación.

### RF-21

**Funcionalidad crítica:** El sistema debe retener el dinero de una compra o intercambio hasta la confirmación de entrega por parte de ambos miembros

**Justificación:** Es crítica porque materializa una parte fundamental de la promesa de valor relacionada con la seguridad de las operaciones. Retener el dinero hasta que ambas partes confirmen la entrega introduce decisiones arquitectónicas relacionadas con el estado de la operación, coordinación entre las partes y comunicación con la pasarela de pagos.

### RF-22

**Funcionalidad crítica:** El sistema debe liberar el dinero hacia el vendedor/persona con el objeto de mayor valor en un intercambio luego de la confirmación de entrega por parte de ambos miembros

**Justificación:** Es crítica porque determina el resultado financiero de un intercambio con diferencia monetaria. El sistema debe identificar quién debe recibir los fondos y garantizar que la liberación ocurra únicamente después de cumplirse la finalización de la operación

### RF-41

**Funcionalidad crítica:** El sistema debe permitir a cada parte de un intercambio o compra confirmar que la entrega presencial fue completada exitosamente.

**Justificación:** Es crítica porque conecta la operación digital con el evento físico que permite finalizarla. La confirmación de entrega por ambas partes es una condición necesaria para determinar que el intercambio se completó y, por tanto, afecta directamente el flujo de seguridad y liberación del dinero.

### RF-42

**Funcionalidad crítica:** El sistema debe permitir cancelar una propuesta de intercambio o compra antes de su confirmación final.

**Justificación:** Es crítica porque define uno de los caminos principales del ciclo de vida de una operación. Debe determinarse en qué estados puede cancelarse una operación y qué consecuencias tiene dicha cancelación sobre los demás elementos del proceso, especialmente sobre el dinero retenido.

### RF-43

**Funcionalidad crítica:** El sistema debe reembolsar el dinero retenido de una compra o intercambio si este se cancela antes de la confirmación de entrega.

**Justificación:** Es crítica porque establece qué pasa con el dinero cuando una operación no llega a completarse. Forma parte de la garantía financiera ofrecida por la plataforma y debe coordinarse con el estado de la operación y con la pasarela de pagos para evitar que una cancelación deje el dinero en el lugar incorrecto

### RF-18

**Funcionalidad crítica:** El sistema debe permitir aceptar o rechazar propuestas de intercambio

**Justificación:** Es crítica porque formaliza el resultado de la negociación. La aceptación o rechazo determina si una propuesta se convierte en una operación acordada o finaliza sin intercambio entre dichos usuarios.

### RF-33

**Funcionalidad crítica:** El sistema debe permitir calificar a un usuario luego de un intercambio o compra en una escala numérica de 1 a 5

**Justificación:** Es una funcionalidad que aumenta la cantidad de datos para la reputación de un usuario, lo que es importante para cumplir con la promesa de confianza de la plataforma, y asi los usuarios puedan tener confinza a la hora de comprar

### RF-35

**Funcionalidad crítica:** El sistema debe permitir acceder al historial de intercambios de cualquier usuario

**Justificación:** Es una funcionalidad importante para cumplir con la promesa de confianza del proyecto, y a su vez, permite ver la confiabilidad de la persona con la cual realizará el intercambio o, en su defecto, a quien le comprara algun producto

### RF-36

**Funcionalidad crítica:** El sistema debe permitir consultar la reputación de un usuario

**Justificación:** Porque facilita que un usuario tenga o no confianza en realizar una compra/intercambio con otro, lo cual le da seguridad en la plataforma. Así puede ver si este usuario es confiable, es bueno y cómo le ha ido en sus intercambios anteriores

### RF-08

**Funcionalidad crítica:** El sistema debe permitir crear publicaciones con producto, tipo (Compra/intercambio), nombre, descripción, fotos y ciudad

**Justificación:** Es significativa porque las publicaciones son el punto de entrada del marketplace y permiten representar la oferta disponible para compra o intercambio. Sin este elemento no puede iniciarse el flujo comercial principal ni materializarse la propuesta de valor

### RF-12

**Funcionalidad crítica:** El sistema debe permitir filtrar las publicaciones por parámetros como ciudad, precio o categoría

**Justificación:** Los filtros ayudan a los compradores a ver articulos en especifico, permitiendo buscarlos por lugar de venta, precio, categorias y mas filtros que ayudan a facilitar las busquedas
