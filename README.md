# AD-3_Tarea_UML
Repositorio destinado a la entrega de la AD-3 de la asignatura Entornos de desarrollo
Autor: David Fernández Martínez


![Diagrama sin título-Página-1 drawio](https://github.com/user-attachments/assets/658699dd-bd4c-45b7-8a25-8fe7871657e0)

Aquí muestro el diagrama de los casos de uso donde se puede ver, que he optado por mostrar a tres actores (Administrador, Entrenador y Jugador).
<br>
Los distintos casos de usos se ven claramente identificados ("Registrar equipo","Añadir jugadores a un equipo" y "Consultar lista de equipos y jugadores").
<br>
Los tres casos de uso, estan unidos al actor (Administrador) porque considero imprescindible un administrador para realizar los tres casos de uso.
Además, en el caso de uso "Registrar equipo" he hecho un "include" que lo he denominado "Comprobar que no esté inscrito ya" por si se diese la casuistica de que, al ir a registrar un equipo, crashee el sistema porque ya estuviese creado y lo he visto imprescindible.
<br>
También realicé, en el caso de uso "Añadir jugadores" otro "include" que compruebe que el jugador a inscribir, se encuentre libre de estar adjudicado en algún equipo.
<br>
Para finalizar, en el caso de uso "Consultar lista de equipos y jugadores", en este caso, he realizado un "extends" llamado "Ver estadísticas" para ampliar y, como su propio nombre indica, extienda el caso de uso principal. 
<br>
He de recalcar que, como se ve en la imagen, los actores "Entrenador" y "Jugador" están conectados al caso de uso "Consultar lista" porque así podrán, aparte de consultar la lista de jugadores y equipos inscritos, ver las estadísticas de cualquier jugador ya inscrito tras algún encuentro ya realizado. No he creido conveniente conectarles a los otros dos casos de uso porque no es de su competencia directa, sino de una persona administradora.




![Diagrama sin título-Página-2 drawio](https://github.com/user-attachments/assets/f486f80a-73b3-4527-97d5-02ad909ab1ec)



Aquí arriba está mi representación de la estructura del sistama con sus clases, atributos, métodos y relaciones entre sí.
<br>
Se pueden ver las tres clases principales (correlación con los casos de uso anteriormente vistos) y en ellas, desplegados sus atributos.
<br>
He creído conveniente la creación de una clase de control (o superclase) para poder gestionar bien todo lo que englobe y esté relacionado con el torneo en el que, el administrador, entrenador o jugador, no tengan las competencias para realizar cualquier acción, de ahi la creacion de un "supervisor" de todo el torneo. También se encuentran dentro de la clase de control los métodos para gestionar el torneo, asi como la creacion del propio torneo, de los equipos, la inscripción de los jugadores, el cálculo de las estadísticas ...
<br>
Las tres clases anteriores tienen una relación de asociación con la clase de control porque hay una relación general entre clases. 
<br>
Entre la clase "Administrador" y la superclase, podría caber la posibilidad de dependencia ya que podemos pensar que, sin torneo no existiría la figura del administrador pero he optado por la relacion de "Asociación".
<br>
En relación a las cardinalidades, tal y como se observa en la imagen, todas son de uno a muchos ya que, las tres clases pueden estar en 1 torneo o en muchos, bien sea en el papel de administradores, entrenadores o jugadores.


CONCLUSIONES DEL TRABAJO

Con la realización de esta tarea he podido comprender y aplicar el modelado UML asi como la representacion de su estructura con los distintos diagramas realizados.
<br>
Además he reforzado los conceptos de entidades y relaciones ya adquiridas en el módulo.



