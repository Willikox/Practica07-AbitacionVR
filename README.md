# Build an Apartment
Starter project for the Udacity [VR Developer Nanodegree](http://udacity.com/vr) program.

- Course: VR Scenes & Objects
- Project: Build an Apartment


### Versions Used
- [Unity LTS Release 2017.4.15](https://unity3d.com/unity/qa/lts-releases?version=2017.4)
- [GVR SDK for Unity v1.170.0](https://github.com/googlevr/gvr-unity-sdk/releases/tag/v1.170.0)


### Directory Structure
- The Unity project is the child directory of the repository and named according to the associated lesson.
- The Unity project is 'cleaned' and includes the `Assets` folder, the `ProjectSettings` folder, and the `UnityPackageManager` folder.


### GVR SDK for Unity
- `GoogleVR` > `Demos` is not included.
- `GoogleVR` > `GVRVideoPlayer.unitypackage` is included.
- Scripts applicable to the course have been updated to reflect Unity's API change from `UnityEngine.VR` to `UnityEngine.XR`.

>**Note:** If for any reason you remove and re-import GVR SDK for Unity v1.170.0, make sure you accept any API update pop-up prompts triggered by Unity. Alternatively, you can manually run the API updater (Unity menu `Assets` > `Run API Updater...`) after the import has completed.


### Related Repositories
- [VR Scenes and Objects - Game Objects](https://github.com/udacity/VR-Scenes-and-Objects_Game-Objects/releases)
- [VR Scenes and Objects - Animations](https://github.com/udacity/VR-Scenes-and-Objects_Animations/releases)
- [VR Scenes and Objects - Cameras](https://github.com/udacity/VR-Scenes-and-Objects_Cameras/releases)
- [VR Scenes and Objects - Lights](https://github.com/udacity/VR-Scenes-and-Objects_Lights/releases)
- VR Scenes and Objects - Build an Apartment
# Practica07-AbitacionVR
1.	El Apartamento debe tener al menos 25 modelos prefabs (objetos 3D) que deben
ser colocados apropiadamente dentro de la escena. Los objetos no pueden estar
flotando sin motivos reales.
 

Sala: 3 sillones, 1 mesa, 1 globo terráqueo, 1 reloj, 1 tablero de ajedrez, 1 TV, 1 mueble para la TV y 2 muebles laterales, 1 alfombra.

  

Comedor: 4 sillas, 1 mesa, 1 repostero de frutas
 

Cocina: 1 muble de cocina, 1 refrigeradora, 1 cocineta, 1 microondas, 1 piso, 3 módulos de cocina

 

Biblioteca: 1 escritorio, 1 silla giratoria, 1 monitor, 1 teclado, 1 ratón, 1 librero y varios libros. 


2.	Crear un tablero de ajedrez y colocarlo sobre un objeto (por ejemplo: mesa,
estante, etc) usando materiales y texturas.
 

Para el tablero de ajedrez se descarga una imagen; en este caso JPG; y se añade a la carpeta texturas; la misma que se encuentra dentro del proyecto. Una vez creado el cubo, lo vamos a dimensionar a escala de un tablero; para finalmente ya con la imagen presente lo único que hacemos es arrastrar la imagen al cubo de tal forma q se nos queda como el de la imagen. Lo único que nos queda es mover a una superficie, en este caso una mesa.  
3.	Crear al menos tres cuadros o portarretratos con imágenes del estudiante y su
familia.
 
Al igual que se hizo con la imagen del ajedrez, vamos a trasladar la imagen de una foto o imagen de nuestra familia en la misma carpeta de texturas y de igual manera un cubo con escala de un cuadro y al final lo arrastramos y colocamos de manera adecuada en nuestra casa. 
4.	Crear un globo terráqueo usando una textura con base a una imagen del mapa
del mundo
 

Para el globo terráqueo lo primero que hacemos es llevar el prefaps de globo y luego crear una esfera en donde que al igual que las imágenes le arrastramos hacia la esfera y se nos que da plasmado esa imagen de los continentes de nuestro planeta.  Posterior a ello ubicamos la esfera en el artefacto que sostiene a nuestro globo terráqueo. El paso dos sería darle movimiento.



5.	Crear al menos un shader que cambie el color de un objeto con base al tiempo
transcurrido desde la ejecución de la app.
  
En este caso el teclado se quiso hacer como iluminación al cambio de color, Creamos un Shader y vemos cómo cambia de color.

 
Así mismo creamos un material y en custom seleccionamos el shader que le creamos y finalmente arrastramos al objeto que queremos aplicar la animación y damos acorrer y observaremos como cambia de color.

6.	Animar las manecillas del reloj.
 

Para que gire nuestro reloj lo que tenemos q hacer es irnos a Animator y al igual que el globo terráqueo le hacemos que gire en Z de esta manera dando valores de 0, 180, 360 y así se nos mueve el reloj según las manecillas de reloj 
  
Para quitar el retraso le damos en lineal y en los puntos de extremos a extremos le seleccionamos en linear y se nos va arreglar a correr el programa. 

7.	 Crear un trigger que permita cambiar el sentido de una de las manecillas del
reloj.
 
Para ello creamos un nuevo archivo en donde nuestros valores será 360, 180, 0 y luego en las curvas le damos en linear. Ahora vamos a crear el trigger al igual que el globo terráqueo. 
 

En las dos líneas que conectan a ReversaSegundosAnimacion y la que conecta a exit le damos como Reversa el nombre que le dimos al trigger  y le mandamos a correr y lo tenemos ya creado a la hora de correr. 



8.	Animar el globo terráqueo para que gire horizontalmente.
  
Nuestra rotación será en Y en 3 tiempos le damos valores, el primero en 0, el segundo en 180 y el tercero en 360; de esta manera gira nuestro cubo; a este le dimos un nombre de Giro Y. Ahora creamos otro archivo de nombre Detener, a este no le damos valores para que se pueda detener nuestra esfera. 


9.	Crear un trigger que permita girar y detener la animación del globo terráqueo

 

De la misma forma creamos un archivo y los valores serán todos en 0 para que se detenga nuestro archivo al seleccionar 

 
Como el reloj las flechas blancas le damos en detener y a correr veremos cómo va detenerse el globo al tocar la misma.

10.	Añadir una cámara de realidad virtual (GoogleVR) y colocarla para que la aplicación inicie dentro de la escena del apartamento.
   
 Ya creado la cámara vamos a seleccionar en GoogleVR para poder ver la realidad virtual. Ahora colocamos la cámara dentro del la realidad virtual. Al colocar la misma posición de la cámara observamos que al darle a correr se nos muestra ya la realidad virtual. 








11.	Añadir luces a la escena 
  

Para ello colocamos 4 tipos de sol:
Directional light: Este se nos refleja como la luz del sol
Point light: Este es un foco que ilumina nuestra habitación
Spotlight: Este nos iluminara lugares específicos de acuerdo a la intensidad que le demos.
Area Light: este también es un tipo de foco de iluminación especifica.

 
 Cada uno de ellos podemos cambiar la intensidad de la iluminación e incluso el color que deseamos que se muestre.

12.	Colocación de música al archivo fondo del paisaje:
Descargamos la respectiva librería y luego la importamos a música o sonido de fondo. Una vez realizado dicho método le colocamos seleccionando en cámara. Finalmente le colocamos en la respectiva sección como es audioclip 

 







