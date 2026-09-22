# PersistApp
Software de rastreo de hábitos y análisis de tendencias semanales.

## Definición del problema
Es muy común que cuando una persona se propone crear un hábito (bien un hábito positivo, o dejar de caer en patrones negativos), se vea incapaz de hacerlo por no tener un soporte constante que le anime a seguir adelante. No existe una alternativa real que permita predecir con seguridad el patrón con el que se falla a la hora de intentar establecer un hábito saludable, que a menudo es posible medirlo, pues suele estar asociado a eventos (estrés laboral/académico, mala calidad de sueño, o días festivos, entre otros).

Los servicios tradicionales basados en notificaciones periódicas sufren de habituación, perdiendo efectividad al corto plazo al no poder identificar los momentos de mayor vulnerabilidad o riesgo de incumplimiento de metas. Por tanto, aparece la necesidad de analizar y caracterizar los patrones por los que se falla a partir de un historial de actividad para poder identificar cuándo y bajo qué circunstancias hay mayor riesgo de ruptura de un ciclo de hábitos.

Por ejemplo, digamos que un usuario se propone acostarse todos los días sin excepción a las 21:30, pero que los fines de semana, al no tener la presión de ser el día siguiente lectivo, se acuesta más tarde. PersistApp, en este caso, notificará cuando se acerque la fecha al usuario para recordarle que su tendencia es que los viernes y los sábados se quede despierto hasta las tantas.

Esto es una especificación, pero se puede ampliar a muchos ámbitos: la persona que deja de fumar tiene la manía de fumarse un cigarro todos los días después de comer, quien intenta bajar de peso se da atracones los fines de semana al salir, hay personas que intentan estudiar a diario dos horas y caen en el ciclo de no estudiar los fines de semana...

## Necesidad de cómputo principal del software

El análisis de los patrones donde se rompen estos ciclos no es trivial. Se debe tener previamente un registro de las tendencias que ha tenido el usuario previamente y se debe procesar y comparar con los datos actuales. Si tanto esta semana, como la anterior, los viernes no cumple su objetivo, se determina que existe un factor común, y se guardan esos datos.

## Necesidad de despliegue en la nube

El usuario ha de tener un registro constante en cualquiera de sus dispositivos, y en cualquier parte, lo que ya es indicio de la necesidad de un despliegue en la nube. Además, se deben guardar datos de estos patrones, por lo que debe existir algún almacenamiento persistente remoto al que cualquier instancia del programa en diferentes dispositivos del usuario deben ser capaces de acceder.

## Datos

Actualmente existen varias fuentes reales y públicas de conjuntos de datos, extraídos de un sector de la población que fueron monitorizados a lo largo de su rutina diaria. En concreto, para este proyecto, se usarán a la hora de pasar las pruebas los conjuntos de datos del repositorio de GLOBEM y del proyecto StudentLife, hecho por la universidad de Dartmouth. El primero montiroea diferentes propiedades de la vida, y el segundo se centra en el uso del teléfono móvil.

Para nuestro caso, ambos son perfectamente válidos (digamos que monitorizan dos tipos de hábitos diferentes).

## Configuración

Pendiente de concretar.

## Referencias

- **[Repositorio de conjunto de datos de tendencias en sociedad GLOBEM](https://github.com/UW-EXP/GLOBEM)**
- **[Repositorio de conjunto de datos de tendencias de estudiantes universitarios en Dartmouth](https://github.com/frycast/studentlife)**

## Documentos

Se puede consultar lo relativo al objetivo 0 [aquí](/Objetivos/Objetivo_0/objetivo-0.md).
