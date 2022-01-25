# Sleep mode
-----------------
El modo "Sleep" es una manera de reducir el consumo energetico del dispositivo, llevando al minimo el consumo del microcontrolador y sus perifericos dejando solo lo necesario para su operacion hasta que tenga que realizar alguna accion. La reduccion del consumo energetico aplica principalmente durante la mayor parte del tiempo que permanece en reposo y de esa forma externder la vida util de las baterias. 
Sin hacer uso de este modo y dependiendo de los modulos utilizados (ADC, USART, TWI, etc), el dispositivo puede consumir desde los 3mA de manera constante. Con ese consumo energetico y unas pilas AAA, el tiempo estimado de duracion de las pilas es de 1 a 3 semanas. Una vez se utiliza el modo Sleep, los consumos pueden ir hasta los 5uA en estado de reposo. 

A continuacion se muestran algunos de los ejemplos pero aplicando el modo Sleep para la reduccion del consumo energetico.

