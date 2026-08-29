# Quality Attribute Scenario: ESC-CAL-CON-0008 
Si la plataforma supera las métricas saludables de funcionamiento y se aproxima la caída del sistema, se deben realizar acciones para mitigar daños mayores

## Metadata
* **Quality Attribute:** Confiabilidad
* **Priority:** High
* **Difficulty / Risk:** High
* **Status:** Draft

## Scenario Definition

| Part | Component | Description |
| :--- | :--- | :--- |
| **1** | **Source** |Sistema |
| **2** | **Stimulus** | Se detectan valores comprometedores de almacenamiento, rendimiento y demás componentes que apunten a una pronta caída del sistema|
| **3** | **Artifact** | Todo el sistema |
| **4** | **Environment** | Operación normal con alta concurrencia de usuarios |
| **5** | **Response** | El sistema genera una alerta y ejecuta o habilita las acciones de mitigación previstas antes de que la degradación provoque una interrupción del servicio|
| **6** | **Response Measure** | En pruebas controladas, el 95% de las amenazas se logran controlar antes de que llegue la caída del sistema |

## Architecture Notes
* **Business Rationale:** Si este escenario no existiera, la plataforma podría alcanzar niveles críticos de utilización de recursos sin detectarlos oportunamente, provocando degradaciones o caídas inesperadas del servicio. Esto obligaría al equipo técnico a reaccionar después de ocurrido el fallo, aumentando el impacto sobre los usuarios y el riesgo de interrupción de operaciones activas

* **Architectural Tactics:** Utilizar health check, circuit breaker y monitoreo proactivo, que son técnicas con pruebas automatizadas que verifican el comportamiento del sistema a través de errores de ejecución en tiempo real, más específicamente:

El health check genera unas “comprobaciones de salud” en las que cada componente expone o permite comprobar si está funcionando correctamente con el fin de llegar directamente a la falla sin necesidad de hacer un barrido general de todos los componentes a ciegas 

El patrón circuit breaker que permite tener mayor tolerancia a fallos

Monitoreo proactivo
Se recopilan continuamente métricas de salud de la plataforma, la idea es detectar tendencias antes de que lleguen al punto de falla como uso de CPU, almacenamiento, memoria, tiempos de respuesta, entre otros

Alertas automáticas
Cuando se supera un umbral, no podemos depender de que alguien esté mirando un dashboard. El sistema debería poder generar automáticamente una alerta al equipo responsable.
* **Assumptions & Risks:** Se asume que los recursos críticos podrán ser monitoreados mediante métricas capaces de anticipar condiciones de degradación, que será posible establecer umbrales preventivos confiables y que existirá tiempo y capacidad técnica suficiente para ejecutar acciones de mitigación antes de una caída. También se asume que el sistema de monitoreo estará disponible y que las acciones preventivas no producirán efectos adversos
