# PersistApp
Software de rastreo de hábitos y análisis de tendencias semanales.

## Definición del problema
Es muy común que cuando una persona se propone crear un hábito (bien un hábito positivo, o dejar de caer en patrones negativos), se vea incapaz de hacerlo por no tener un soporte constante que le anime a seguir adelante.

Existen ya muchos servicios locales (instalados en tu propio dispositivo) que te ponen recordatorios diarios. Yo tuve durante un tiempo un programa en mi teléfono que todos los días me recordaba 5 veces que bebiese agua, y al final acabaron siendo como una notificación cualquiera en mi dispositivo a la que no le prestaba atención una vez me acostumbré a recibirlas. El añadido que propongo a esta base es hacer un análisis sobre qué días de la semana es más probable que no se cumplan esos objetivos.

Por ejemplo, digamos que un usuario se propone acostarse todos los días sin excepción a las 21:30, pero que los fines de semana, al no tener la presión de ser el día siguiente lectivo, se acuesta más tarde. PersistApp, en este caso, notificará cuando se acerque la fecha al usuario para recordarle que su tendencia es que los viernes y los sábados se quede despierto hasta las tantas.

Esto es una especificación, pero se puede ampliar a muchos ámbitos: la persona que deja de fumar tiene la manía de fumarse un cigarro todos los días después de comer, quien intenta bajar de peso se da atracones los fines de semana al salir, hay personas que intentan estudiar a diario dos horas y caen en el ciclo de no estudiar los fines de semana...

## Necesidad de cómputo principal del software

El análisis de los patrones donde se rompen estos ciclos no es trivial. Se debe tener previamente un registro de las tendencias que ha tenido el usuario previamente y compararla con los datos actuales. Si tanto esta semana, como la anterior, los viernes no cumple su objetivo, se determina que existe un factor común, y se guardan esos datos.

## Necesidad de despliegue en la nube

El usuario ha de tener un registro constante en cualquiera de sus dispositivos, y en cualquier parte, lo que ya es indicio de la necesidad de un despliegue en la nube. Además, se deben guardar datos de estos patrones, por lo que debe existir algún almacenamiento persistente remoto al que cualquier instancia del programa en diferentes dispositivos del usuario deben ser capaces de acceder.

## Documentos

Se puede consultar lo relativo al objetivo 0 [aquí](/Objetivos/Objetivo_0/objetivo-0.md).
