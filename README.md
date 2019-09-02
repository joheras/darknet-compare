Pasos previos:
1. Crear una carpeta
2. Dentro de esta carpeta crear dos carpetas una llamada labels y otra llamada detection
3. Dentro de la carpeta labels almacenar los .txt (formato YOLO) con la anotación manual
4. Dentro de la carpeta detection almacenar los .txt (formato YOLO) con la anotación generada. 
5. En la carpeta principal crear un fichero (test.txt) que contenga la lista de ficheros contenidos en la carpeta labels (se tiene que proporcionar la ruta completa).
6. En la carpeta principal crear un fichero (names.txt) que contenga la lista de clases.

Para realizar la comparación dentro de la carpeta ejecutar
./darknet detector compare test.txt names.txt

donde test.txt es la ruta completa al fichero creado en el paso 5 y names.txt la ruta completa al fichero creado en el paso 6. 

Para usar el ejemplo de la carpeta prueba2 ejecutar:
./darknet detector compare prueba2/test.txt prueba2/names.txt
