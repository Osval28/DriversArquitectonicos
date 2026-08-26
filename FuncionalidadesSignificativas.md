# Funcionalidades Significativas

## Índice

| Identificador | Tipo de funcionalidad significativa |
|:---|:---|
| RF-14 | Valor de negocio |
| RF-15 | Valor de negocio |
| RF-19 | Valor de negocio |
| RF-21 | Ambos |
| RF-22 | Ambos |
| RF-41 | Ambos |
| RF-42 | Valor de negocio |
| RF-43 | Ambos |
| RF-18 | Valor de negocio |
| RF-33 | Valor de negocio |
| RF-35 | Valor de negocio |
| RF-36 | Valor de negocio |
| RF-08 | Valor de negocio |
| RF-12 | Valor de negocio |

## Detalle

### RF-14

El sistema debe permitir realizar propuestas de intercambio con producto, valor, encime y lugar

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es crítica porque materializa el dominio de negocio de nuestro proyecto: La negociación de intercambios. Permite iniciar una operación especificando los productos que serán negociados y constituye el punto de partida del flujo principal de generación de valor de la plataforma.

### RF-15

El sistema debe permitir realizar contraofertas a un intercambio propuesto

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es crítica porque forma parte directamente del mecanismo de negociación que diferencia al proyecto de un marketplace convencional. Permitir contraofertas en el intercambio haciendo posible que el intercambio sea dinámico y no se limite a una propuesta de compra de un solo lado.

**Observación:** Una contraoferta se refiere a la "negociación" que quiera hacer una persona frente a un valor en un intercambio, valor excedente, cambios mano a mano, y demas

### RF-19

El sistema debe permitir comprarle y/o encimarle por un producto directamente al vendedor a través de una pasarela

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es significativa porque representa el segundo flujo comercial del proyecto además del intercambio. Permite atender usuarios que desean realizar una compra directa y alimenta el mecanismo de monetización asociado a las operaciones que pasan por la plataforma.

**Observación:** Se aclara a los vendedores y compradores que, al realizar una compra o una venta, el modelo de negocio utiliza un proceso de comision por venta

### RF-21

El sistema debe retener el dinero de una compra o intercambio hasta la confirmación de entrega por parte de ambos miembros

**Tipo de funcionalidad significativa:** Ambos

**Justificación:** Es crítica porque materializa una parte fundamental de la promesa de valor relacionada con la seguridad y confianza de las operaciones. Retener el dinero hasta que ambas partes confirmen la entrega, introduce decisiones arquitectónicas relacionadas con el estado de la operación, coordinación entre las partes y comunicación con la pasarela de pagos.

### RF-22

El sistema debe liberar el dinero hacia el vendedor/persona con el objeto de mayor valor en un intercambio luego de la confirmación de entrega por parte de ambos miembros

**Tipo de funcionalidad significativa:** Ambos

**Justificación:** Es crítica porque determina el resultado financiero de un intercambio con diferencia monetaria. El sistema debe identificar quién debe recibir los fondos y garantizar que la liberación ocurra únicamente después de cumplirse la finalización de la operación

**Observación:** Con resultado financiero nos referimos a qué parte se le entrega el dinero después de la aplicación de la comisión

### RF-41

El sistema debe permitir a cada parte de un intercambio o compra confirmar que la entrega presencial fue completada exitosamente.

**Tipo de funcionalidad significativa:** Ambos

**Justificación:** Es crítica porque conecta la operación digital con el evento físico que permite finalizarla, lo que le garantiza seguridad y confianza en la plataforma al usuario. La confirmación de entrega por ambas partes es una condición necesaria para determinar que el intercambio se completó y, por tanto, afecta directamente el flujo de seguridad y liberación del dinero.

### RF-42

El sistema debe permitir cancelar una propuesta de intercambio o compra antes de su confirmación final.

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es crítica porque define uno de los caminos principales del ciclo de vida de una operación, dándole seguridad al usuario de que si el producto no es lo que esperaba tiene cierto margen para recuperar su dinero. Debe determinarse en qué estados puede cancelarse una operación y qué consecuencias tiene dicha cancelación sobre los demás elementos del proceso

### RF-43
El sistema debe reembolsar el dinero retenido de una compra o intercambio si este se cancela antes de la confirmación de entrega.

**Tipo de funcionalidad significativa:** Ambos

**Justificación:** Es crítica porque establece qué pasa con el dinero cuando una operación no llega a completarse. Forma parte de la garantía financiera ofrecida por la plataforma y debe coordinarse con el estado de la operación y con la pasarela de pagos para evitar que una cancelación deje el dinero en el lugar incorrecto

### RF-18

El sistema debe permitir aceptar o rechazar propuestas de intercambio

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es crítica porque formaliza el resultado de la negociación. La aceptación o rechazo determina si una propuesta se convierte en una operación acordada, puede finalizar en una compra o en el peor de los casos, no se realiza ningun acuerdo

### RF-33

El sistema debe permitir calificar a un usuario luego de un intercambio o compra en una escala numérica de 1 a 5

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es una funcionalidad que aumenta la cantidad de datos para la reputación de un usuario, lo que es importante para cumplir con la promesa de confianza de la plataforma, y asi los usuarios puedan tener confinza a la hora de comprar

### RF-35

El sistema debe permitir acceder al historial de intercambios de cualquier usuario

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es una funcionalidad importante para cumplir con la promesa de confianza del proyecto, y a su vez, permite ver la confiabilidad de la persona con la cual realizará el intercambio o, en su defecto, a quien le comprara algun producto

### RF-36

El sistema debe permitir consultar la reputación de un usuario

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Porque facilita que un usuario tenga o no confianza en realizar una compra/intercambio con otro, lo cual le da seguridad en la plataforma. Así puede ver si este usuario es confiable, es bueno y cómo le ha ido en sus intercambios anteriores

### RF-08

El sistema debe permitir crear publicaciones con producto, tipo (Compra/intercambio), nombre, descripción, fotos y ciudad

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Es significativa porque las publicaciones son el punto de entrada del marketplace y permiten representar la oferta disponible para compra o intercambio. Sin este elemento no puede iniciarse el flujo comercial principal ni materializarse la propuesta de valor

### RF-12

El sistema debe permitir filtrar las publicaciones por parámetros como ciudad, precio o categoría

**Tipo de funcionalidad significativa:** Valor de negocio

**Justificación:** Los filtros ayudan a los compradores a ver articulos en especifico, permitiendo buscarlos por lugar de venta, precio, categorias y mas filtros que ayudan a facilitar las busquedas
