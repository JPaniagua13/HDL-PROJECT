# HDL-PROJECT
<h1 align="center"> Circuito decodificador de Gray </h1>

# Descripción general
Este proyecto se basa en implementar un circuito decodificador que permita mediante el ingreso de un número Gray el despliegue de su representación decimal en un display de siete segmentos. Para esto se utiliza una placa Basys 3/FPGA en donde se hace uso de los conmutadores, los LEDs y los displays siete segmentos.
## Subsistema 1
Este subsistema es aquel que a su entrada recibe un número de cuatro bits en formato Gray para luego ser transformado en su representación binaria. Este proceso requiere de la asignación de cuatro entradas y cuatro salidas. Las entradas corresponden a los computadores y las salidas se visualizan mediante la herramienta de simulación. Al utilizar la herramienta de simulación, la taza de refrescamiento debe estar asignada a 500 ms.

## Subsistema 2
Este subsistema que corresponde a la continuación del subsistema anterior, consiste en ahora sí desplegar las salidas pero utilizando los LEDs de la placa FPGA.

## Subsistema 3
Este último subsistema está compuesto por cuatro partes. Requiere también hacer uso del "clock" del subsistema dos. Estas partes se dividen en una etapa "refresh counter" que está asociada al clock y, a su vez se encarga de tener un contador de refresco que permita que las dos etapas funcionen simultáneamente. Estas dos etapas corresponden a: la etapa "multiplexor" que es aquella que determina cuál dígito se mostrará en el display y la etapa "ánodo" que define cuál ánodo será encendido. La etapa "cátodos" sería la que se encarga de recibir el dígito que enciende alguno de los siete segmentos.

# Diagramas de bloques
![Implementación lógica del subsistema 1](https://user-images.githubusercontent.com/111257726/195086713-428fa68d-39e8-4790-b95a-875f62756907.jpeg)
En la figura anterior se muestra un diagrama lógico que describe al subsistema 1. 


![555](https://user-images.githubusercontent.com/111306099/195545917-4bfa05bc-5faf-4c1b-9d29-5337c2d09aac.PNG)
En la figura anterior se muestra un diagrama lógico que describe al subsistema 2. 


![photo_5060016296040704608_y](https://user-images.githubusercontent.com/111306099/195543709-bf73c428-4b8c-4a5e-a71e-58c394abf8fe.jpg)
En la figura anterior se muestra un diagrama lógico que describe al subsistema 3. 



[comment]: <> (de cada subsistema y su funcionamiento fundamental, según descritos en la sección 5.)
# Diagramas de estado
[comment]: <> (de todas las FSM diseñadas, si existen, según descritos en la sección 5)
# Ejemplo y análisis de una simulación funcional
[comment]: <> (del sistema completo, desde el estímulo de entrada hasta el manejo de los 7 segmentos.)
# Análisis de consumo de recursos en la FPGA 
[comment]: <> (LUTs, FFs, etc. y del consumo de potencia que reporta la herramienta Vivado.)


![power](https://user-images.githubusercontent.com/111306099/195584545-877af257-13df-469f-8acf-07df53a0b796.PNG)


# Reporte de velocidades máximas de reloj 
[comment]: <> (posibles en el diseño mínima frecuencia de reloj para este diseño: 50 MHz.)
# Análisis de principales problemas 
[comment]: <> (hallados durante el trabajo y de las soluciones aplicadas)
A la hora de empezar el proyecto un problema que surgió fue la verificación de usuario a la hora de instalar Vivado. Un requerimiento para instalar Vivado es la creación de un usuario y una consecuente verificación de datos personales. En esta esta etapa ocurrió que al llenar los datos desplegaba un mensaje de error. Se intentó utilizando la cuenta institucional del Instituto Tecnológico de Costa Rica pero el problema persistió. Finalmente, se envió un correo a la dirección de soporte de Xilinx. Dentro del plazo de dos horas, el correo fue contestado explicando que la cuenta no se encontraba más bloqueada. Sin embargo, los datos del perfil no debían cambiar ya que de lo contrario resultaría en la reaparición del mismo problema.   
&nbsp;&nbsp;&nbsp;&nbsp; Cabe destacar que el software Vivado corre únicamente en sistemas Linux/Windows. Está información habría sido de gran utilidad ya que se intentó correr en una máquina virtual Linux. No habría sido un problema si no fuera a causa de la gran cantidad de memoria que requiere. Es decir la computadora en la que se quiere instalar debe tener como mínimo 160 GB.  
&nbsp;&nbsp;&nbsp;&nbsp; Para los miembros cuyos problemas de instalación persistieron se tomó la decisión de utilizar VMWare para realizar las pruebas iniciales del programa. Al hacer uso de este programa ocurrió otro problema. La interfaz de Vivado se trababa a cortos plazos de tiempo que únicamente se solucionaba reiniciando el computador.
