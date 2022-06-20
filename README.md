# RECONOCIMIENTO_FACIAL
Este repositorio contiene las instrucciones para obtener el reconocimiento facial usando la camara del ESP32


1. cargar el ejemplo en aarduino de "CamaraWebServer" al ESP32, configurar, el tipo de camara (AI_THINKER), red (SSID) y password
2. acceder a la IP que arroja el ESP32 al ejecutar el programa de arduino
3. colocar la resolucion de  "Resolution QVGA(320X240)"
4. Instalar la biblioteca de Deepface
    https://github.com/serengil/deepface   no es necesario clonarlo
    
    para ello se requiere Python3
    comprobar la instalacion
         python3 --version
         se requiere version 3.9 o inferior
     
    $pip install deepface   requiere al menos 2GB de espacio en disco duro
5. 
