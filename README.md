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
     
    $pip install deepface   
    
    requiere al menos 2GB de espacio en disco duro
    si el pip no esta instalado,ejecutar
          sudo apt install python3-pip
5. instalar el plugin de python para Visual Studio Code  solo "Python"
6. correr ejemplo de caractaristicas faciales
    crear un directorio para el ejemplo
          obtener la IP de la camara y tomar una fotografia de 320X240 pixeles
               acceder al IP de la camara
               tomar la foto
               sobre la foto dar clic derecho "Save image As..." guardar la imagen ".jpg"
    crear un archivo facialr.py
         from deepface import DeepFace
              obj = DeepFace.analyze(img_path = "hugo1.jpg", actions = ['age', 'gender', 'race', 'emotion'])
         print (obj)
7. 
