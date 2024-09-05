## CLASIFICACIÓN DE OBJETOS USANDO TÉCNICAS DE DEEP LEARNING CON YOLOv10
Emplear una red YOLOv10  o similar a la que se haya
realizado un proceso de transfer learning para reconocer 5 tipos de objetos del
Ecuador con imágenes captadas con la cámara del computador. Deberá realizar
pruebas de rendimiento usando GPUs vs CPU. El entrenamiento y validación de
resultados de la red puede hacerlo en Google Colab o en cualquier entorno de su
preferencia. Por ejemplo, podría realizar el reconocimiento de especies endémicas
(iguana marina, tortugas gigantes, rana enana de colorado, colibrí de Esmeraldas
y Viscacha Ecuatoriana).

Dataset utilizado es uno propio, le llamamos “Dataset Ecuador”, en ella hicimos un
repositorio de animales endémicos y únicos a nuestro Ecuador y estas conforman 5
clases:

0: cóndor andino

1: iguana marina

2: lobo marino

3: pinzón de Darwin

4: tortuga gigante de galápagos

Esta dataset contiene 50 imágenes por cada clase de animal, las imágenes las dividimos
en 80% para entrenamiento y 20% para validación. Luego necesitábamos las
anotaciones de cada una de esas imágenes respectivamente, con el uso de ‘labelImg’, en
formato YOLO, creamos los labels de las imágenes y las dividimos tal igual como para
las imágenes. 

![image](https://github.com/user-attachments/assets/bbc831d7-5d47-4852-8f90-33fc59986749)

Con el código implementado en Python en un Entorno Local en Jupyter Notebook con acceso a la camera de la computadora y para evaluar el rendimiento del uso del
CPU dieron los siguientes resultados:

![image](https://github.com/user-attachments/assets/5610b4ec-9edf-465e-b7cf-9315b43635cd)

Con el código Implementado en Python en un Entorno de Google Colab para evaluar el
rendimiento del uso del GPU dieron los siguientes resultados:

![image](https://github.com/user-attachments/assets/a043a670-2e85-4560-af11-9b3f2743f212)

Lo que podemos llegar a concluir es que se evidencia que las etiquetas del propio
YOLOv10 ganan a las nuevas que queríamos implementar, lo cual es entendido por la
cantidad de entrenamiento que tuvo cada clase, pero podemos evidenciar, dentro de la
carpeta ‘runs’ que si se realiza los entrenamientos correctamente y como las
validaciones realizan sus intentos. En el futuro sería de trabajar con un dataset mucho
más grande con más imágenes posibles y trabajar sobre el GPU ya que sobre ella el
entrenamiento en el YOLOv10 no pasa la hora (dependiendo el número de epochs).

![image](https://github.com/user-attachments/assets/32f2f514-63b9-4cb5-8eb5-e0443f97c3a1)

![image](https://github.com/user-attachments/assets/27cb2048-8d4b-4557-a417-5bdc47ea2632)

![image](https://github.com/user-attachments/assets/96a14b6c-9857-4151-9b73-d2cb03f8920f)

![image](https://github.com/user-attachments/assets/6008d79a-142a-4410-8a25-08b194a0c90d)




