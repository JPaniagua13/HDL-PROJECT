# HDL-PROJECT
<h1 align="center"> Circuito decodificador de Gray </h1>

# Descripción general
Este proyecto se basa en implementar un circuito decodificador que permita mediante el ingreso de un número de Gray transformarlo a un número binario que represente a un número decimal en un display de siete segmentos. Esto será posible por medio de tres subsistemas que mostrarán las etapas del decodificador.
## Subsistema 1
[comment]: <> (Por Favor revisar esta descripción. Si necesitan hacer cambios Go Ahead. "Este subsistema es aquel que a su entrada tendrá un número de cuatro bits en forma de Gray para luego ser transformado a su forma binaria a través de un código programado. Es decir, se encarga de hacer una lectura del código de Gray que se verá en la entrada para luego pasarlo a binario y, que este a su vez llegue al subsistema 2. Además se encargará de contener una tasa de refresco de 500 ms.")

## Subsistema 2
[comment]: <> (No supe cómo describirla. Por favor, agregar lo que se debe. "Este subsistema es el encargado de recibir el código binario debidamente transformado del subsistema 1, el cual indica por medio de los LEDs de la FPGA a una tasa de refresco de 500 ms, que ese display")

## Subsistema 3
[comment]: <> (En este subsistema se crean cuatro partes que componen a dicho subsistema, además de tener en cuenta al clock del subsistema 2. Estas partes se dividen en una etapa "colocar nombre de etapa de refresh_counter" que está asociada al clock antes mencionado y esta se encarga de tener un contador de refresco que permitirá que dos etapas funcionen al mismo tiempo, las cuales serán: la etapa "colocar nombre de etapa bcd_control" que es aquella que determina cuál dígito se mostrará en el display y la etapa "colocar nombre de etapa del anode_control" que define en cuál ánodo será encendido. La etapa "colocar nombre de etapa de bcd_to_cathodes" sería la que se encarga de recibir el dígito que ...)

# Diagramas de bloques
[comment]: <> (de cada subsistema y su funcionamiento fundamental, según descritos en la sección 5.)
# Diagramas de estado
[comment]: <> (de todas las FSM diseñadas, si existen, según descritos en la sección 5)
# Ejemplo y análisis de una simulación funcional
[comment]: <> (del sistema completo, desde el estímulo de entrada hasta el manejo de los 7 segmentos.)
# Análisis de consumo de recursos en la FPGA 
[comment]: <> (LUTs, FFs, etc. y del consumo de potencia que reporta la herramienta Vivado.)
# Reporte de velocidades máximas de reloj 
[comment]: <> (posibles en el diseño mínima frecuencia de reloj para este diseño: 50 MHz.)
# Análisis de principales problemas 
[comment]: <> (hallados durante el trabajo y de las soluciones aplicadas)
