# Carta Abierta al DANE

Colombia, 19 de Enero de 2018

Señores
Departamento Administrativo Nacional de Estadística - DANE

E.        S.         D.

**Asunto:** Carta abierta al DANE de grupo de desarrolladores de software Colombianos, a propósito del pronunciamiento de la entidad con respecto a los hallazgos en materia de seguridad en la aplicación del eCenso, realizados por la ingeniera Juliana Peña.
De manera cordial los abajo firmantes, Desarrolladores de Software Colombianos, estamos de acuerdo en expresarles lo siguiente:


1. Apoyamos que el DANE haya construido una opción para realizar el censo de forma virtual.
2. Rechazamos cadenas malintencionadas y anónimas que sugieren que hay intento de fraude electoral y que parecen promovidas por sectores políticos especialistas en propaganda negra. En esto también apoyamos al DANE.
3. Aplaudimos la valentía, generosidad y deber cívico con los cuales la desarrolladora de software Juliana Peña publicó sus hallazgos de seguridad. [http://julip.co/2018/01/actualizacion-contrasenas-censo/](http://julip.co/2018/01/actualizacion-contrasenas-censo/)
4. Como profesionales de la industria de Software, rechazamos la posición del DANE en cuanto a los reportes de Juliana. Consideramos que las preguntas de Juliana son válidas y el comunicado de prensa no las responde de manera adecuada, por lo que aún cuestionamos la seguridad del eCenso web y *offline*.

[https://censo2018.dane.gov.co/el-dane-responde-afirmaciones-falsas-sobre-la-seguridad-del-ecenso](https://censo2018.dane.gov.co/el-dane-responde-afirmaciones-falsas-sobre-la-seguridad-del-ecenso)

En referencia al comunicado emitido por el DANE, que cita:


  *“Afirmaciones que son falsas, irresponsables y apresuradas, y han atentado contra la confianza que los colombianos han depositado en la operación estadística más grande e innovadora que ha realizado el país.”*

Se juzga como falsa la siguiente afirmación hecha por Juliana:


  “*las contraseñas no están precisamente guardadas en texto plano, pero es como si lo estuvieran*”

Argumentando:


  *“...mecanismos de encriptación con algoritmos que hacen parte de los estándares internacionales avalados por la Agencia Nacional de Seguridad de los Estados Unidos*”.

Sin mencionar que se permitía descargar una versión del código del sitio, en la opción para diligenciar el censo de forma offline. En el código (Juliana lo explicó y nosotros pudimos comprobarlo) se hace un “cifrado simétrico” conocido por ser inadecuado e inseguro para el cifrado de contraseñas, adicionalmente en el mismo código se incluye la llave que puede ser usada para descifrar las contraseñas.

Ella también aporta como evidencia el hecho de que es exactamente igual al publicado en el sitio [https://stackoverflow.com/](https://stackoverflow.com/questions/1289061#4875807) (red social para compartir y discutir código), que explícitamente indica que aunque funciona, no es seguro.

El sólo hecho de que declaren usar "mecanismos de encriptación" avalados, no garantiza su buen uso. Lo que se cuestiona no es la herramienta sino su aplicación y la consideración por las buenas prácticas de ingeniería.

Queremos señalar que tampoco es válido el siguiente argumento, donde también se afirma que Juliana “falta a la verdad”:


  *“Entre los mecanismos de seguridad implementados por el DANE para mitigar intentos de accesos no permitidos y minimizar el riesgo de presencia de incidentes que puedan afectar la seguridad de la información almacenada en las bases de datos institucionales, se cuenta con soluciones de protección tales como cortafuegos y sistemas de detección y prevención de intrusos (definidos de manera perimetral), así como con la protección a nivel de aplicación a través de un cortafuego web”*

De nada sirve que se tengan puertas con el blindaje de mayor nivel del mundo, ***si dejas la llave de la puerta debajo de la alfombra de bienvenida***. En este caso, permitir la descarga de una versión del código del servidor como opción de diligenciado *offline*, es un serio problema de seguridad que pone en peligro la información y las contraseñas de quienes hayan diligenciado el censo de forma virtual.


5. Nos sumamos al cuestionamiento iniciado por Juliana, y como ciudadanos esperamos que el software producido con recursos públicos con fines de recaudar información personal de ciudadanos colombianos sea de la más alta calidad.
6. Basados en los puntos anteriores, recomendamos que el DANE realice una evaluación profesional e independiente de la siguiente manera:
  1. Se evalúe la implementación de cifrado tanto en la aplicación de escritorio y la web según las recomendaciones de la [OWASP](https://www.owasp.org/index.php/About_The_Open_Web_Application_Security_Project).
  2. Se realicen pruebas de penetración en todos los sistemas de recolección o almacenamiento de información personal de acuerdo a las recomendaciones de la OWASP. [https://www.owasp.org/index.php/Testing_Guide_Introduction#Penetration_Testing](https://www.owasp.org/index.php/Testing_Guide_Introduction#Penetration_Testing)
  3. Se implementen todas las recomendaciones consideradas críticas.
  4. Se publique un reporte con los hallazgos de la evaluación y correcciones, respaldado por la firma evaluadora y de manera pública.


Nos reunimos y organizamos para proveer una posición independiente y libre de afiliaciones políticas, con el fin de hacer un llamado a prevenir desastres informáticos que causen perdida en la confianza de soluciones innovadoras en nuestro país.

**Atentamente:**

- Johann Paul Echavarría - [@abrupto](https://twitter.com/abrupto)
- Alvaro José Agámez Licha - [@codemaxter](https://twitter.com/codemaxter)
- Victor Miguel Rivera Morales
- Edgar López Rios
- Andres Vargas -  [@RogantCO](https://twitter.com/RogantCO)
- Juan C. Rodriguez - [@jcrodriguezu](https://twitter.com/jcrodriguezu)
- Maria Paz Muñoz Parra - [@pazupersonica](https://twitter.com/pazupersonica)
- Pedro Fernández Moreno - [@pedrito](https://twitter.com/pedrito)
- Leidy Daihana Mora Trujillo
- Carlos Manuel Vibanco Ospino
- Mauricio Marin Jimenez
- Daniel Augusto Amariles García - [@danipilze](https://twitter.com/danipilze)
- Ismael Ricardo Valencia Q. [@ricardovalquin](https://twitter.com/ricardovalquin)
- Luis Miguel Jiménez Restrepo - [@luismij](https://twitter.com/luismij)
- Juan Felipe Morales Castellanos
- Sergio Andres Fandiño Basto
- Gabriel De Jesus Goethe Mosquera
- Charly Rafael Palencia Yejas - [@_chalien](https://twitter.com/_chalien)
- Katy García Bedoya - [@kgb369y](https://twitter.com/kgb369y)
- Edgar Duvan Ortega Ramirez
- Richard David Roncancio Acendra - [@Sr_Batusai](https://twitter.com/Sr_Batusai)
- Diana Cadena Moreno
- Jorge Alejandro Rios Franco
- Sorey Bibiana García Zapata - [@soreygarcia](https://twitter.com/soreygarcia)
- Daniel García
- Juan Fernando Gaviria Sánchez
- Roberto Mario Rueda Quintero
- Andrés Ossa Arango
- Cleyber Dubian Rengifo Fonnegra
- Juliana Gomez
- Johny Alexander Varela Osorio
- Daniel Felicita
- Hernan Guzman - [@hernandgr](https://twitter.com/hernandgr)
- Cristian Camilo Moreno Zuluaga - [@khriztianmoreno](https://twitter.com/khriztianmoreno)
- Andres Felipe Cardona Castro
- Daniel Felipe Marulanda - [@Dfmarulanda](https://twitter.com/Dfmarulanda)
- Lina Maria Montaño Ramirez - [@calypso_bronte](https://twitter.com/calypso_bronte)
- Lewis Florez Renza - [@gasper_lf](https://twitter.com/gasper_lf)
- Jeison Higuita Sanchez
- Sebastian Castro Paz
- Germán David Potes Franco - [@manchoPotes](https://twitter.com/manchoPotes)
- Natalia Díaz Padilla
- Juan David Gómez Escobar
- Luis Carlos Rosas Orellano - [@LuisRosasO](https://twitter.com/LuisRosasO)
- Juan Pablo Giraldo - [@qjuanp](https://twitter.com/qjuanp)
- David Leonardo Nuñez - [@dlnunezr](https://twitter.com/dlnunezr)
- Diego Castro - [@diarcastro](https://twitter.com/diarcastro)
- Miguel Hincapié - [@miguel_hincapie](https://twitter.com/miguel_hincapie)
- Ricardo Franco Reyes
- Daniel Sanchez - [@EruJazz](https://twitter.com/EruJazz)
- Yeiner Fernández Bustos - [@yeinerf](https://twitter.com/yeinerf)
- Elba Patricia Sánchez Márquez - [@ElbaSanchezM](https://twitter.com/ElbaSanchezM)
- Jose Miguel García García - [@pingoz](https://twitter.com/pingoz)
- Juan Sebastian Velez
- Juan Felipe Bedoya Cardona - [@jfelipebc](https://twitter.com/jfelipebc)
- Manuel Fernando Sabogal Ocampo - [@ItsEdoren](https://twitter.com/ItsEdoren)
- Francisco Arley López Espinosa
- Sergio Andres Valencia Yepes
- Andrés Felipe Londoño Mesa - [@andreslon](https://twitter.com/andreslon)
- Jose Fabio Jaramillo Castro
- Laura Ciro - [@ltciro](https://twitter.com/ltciro)
- Diego Avila
- David Przybilla - [@dav009](https://twitter.com/dav009)
- Guillermo Daniel Iguaran Suarez - [@guilleiguaran](https://twitter.com/guilleiguaran)
- Luis Alberto Vélez Tascon - [@luchovelez](https://twitter.com/luchovelez)
- Juan Marín - [@jpmarindiaz](https://twitter.com/jpmarindiaz)
- Isabel Cristina Ruiz Buriticá
- Camilo Alexander Rodríguez
- Alejandro Villegas Carvajal - [@neopilatos](https://twitter.com/neopilatos)
- Jesse Javier Cogollo - [@jessecogollo](https://twitter.com/jessecogollo)
- Ernesto Nobmann Chávez - [@nobmann88](https://twitter.com/nobmann88)
- Sebastian Sogamoso - [@sebasoga](https://twitter.com/sebasoga)
- Juan Pablo Buriticá - [@buritica](https://twitter.com/buritica)
- Cristian Andrés Martínez - [@b3nkos](https://twitter.com/b3nkos)
- Hamilton Alvarez Mejia - [@mejialvarez](https://twitter.com/mejialvarez)
- Ernesto Nobmann Chávez - [@nobmann88](https://twitter.com/nobmann88)
- Camilo Aguilar Ramírez - [@c4milo](https://twitter.com/c4milo)
- Juan Gabriel Gutierrez - [@llanoxco](https://twitter.com/llanoxco)
- Emmanuel Deossa Hincapié - [@emmanuelsw](https://twitter.com/emmanuelsw)
- Federico López Gómez - [@FicoYPlaca](https://twitter.com/FicoYPlaca)
- Marcos Javier Alvarez - [@garusis](https://twitter.com/garusis)
- Andrés Bedoya Garces - [@angel_fire](https://twitter.com/angel_fire)
- Sebastián Arcila Valenzuela - [@sarcilav](https://twitter.com/sarcilav)
- Miguel Fernando Cabrera  - [@mfcabrera](https://twitter.com/mfcabrera)
- Angie Melissa Delgado - [@Meyito_](https://twitter.com/Meyito_)
- Federico Builes - [@febuiles](https://twitter.com/febuiles)
- Nicolás Hock Isaza - [@nhocki](https://twitter.com/nhocki)
- Hildebrando Rueda Quintero - [@theharq](https://twitter.com/theharq)
- Alejandro Cadavid López - [@acadavid](https://twitter.com/acadavid)
- Yeison Daza - [@yeion7](https://twitter.com/yeion7)
- Steven Augusto Villegas Castellanos - [@stifflerbassman](https://twitter.com/stifflerbassman)
- David Andres Roncancio Joya - [@kuryaki](https://twitter.com/kuryaki)
- Oscar Rendon - [@orendon](https://twitter.com/orendon)
- Pablo Vallejo - [@PabloVallejo_](https://twitter.com/PabloVallejo_)
- Juan Pablo Valencia Gómez - [@jpvg10](https://twitter.com/jpvg10)
- Adrian Estrada - [@edsadr](https://twitter.com/edsadr)Addi
- Alejo Yarce - [@AlejooYarce](https://twitter.com/AlejooYarce)
- Fredy E Mena Andrade - [@xfry](https://twitter.com/xfry)
- Juan David Gómez - [@judavi](https://twitter.com/judavi)
- Adrian Estrada - [@edsadr](https://twitter.com/edsadr)
- Carlos Daniel Muñoz Idarraga - [@cdmunozi](https://twitter.com/cdmunozi)
- Santiago M Zubieta Ortiz - [@zubie7a](https://twitter.com/zubie7a)
- Julian Betancourt - [@juliian41](https://twitter.com/juliian41)
- Andrey Ruíz Hincapié - [@davkorss](https://twitter.com/davkorss)
- Gustavo Andrés Angulo - [@woakas](https://twitter.com/woakas)
- Juan David henao - [@jhenaoz93](https://twitter.com/jhenaoz93)
- Juan Mateo Velilla Ospina - [@r3v3r5ing](https://twitter.com/r3v3r5ing)
- Juan David Sánchez - [@d4vsanchez](https://twitter.com/d4vsanchez)
- César Suárez T. [@cesarlarsson](https://twitter.com/cesarlarsson)
- Edward Alejandro Rayo Cortés - [@earayo0521](https://twitter.com/earayo0521)
- Alejandro Next - [@alejonext](http://github.com/alejonext/)
- Alejandro Ramírez - [@soyalejoramirez](https://twitter.com/soyalejoramirez)
- Mario Daniel Ruiz Saavedra - [@desiderantes](https://twitter.com/desiderantes)
- Rubén Darío Avila Home - [@rubenavilah](https://twitter.com/rubenavilah)
- Claudia Lagos Ruiz - [@ClaudiaLagosR](https://twitter.com/ClaudiaLagosR)
- John Fredy Baquero Celis - [@noverflow](https://twitter.com/noverflow)
- Ramiro Andrés Bedoya - [@imramiro](https://twitter.com/imramiro)
- Juan David Maldonado - [@jdmaldonado06](https://twitter.com/jdmaldonado06)
- Johana S. Rodriguez - [@Joha0](https://github.com/joha0)
- Marian Villa - [@marianvilla](https://twitter.com/Marianvilla)
- Alonso Montenegro [@alonsoenrique](https://github.com/alonsoenrique/)
- Jahir Fabian Fiquitiva Ricaurte - [@jahirfiquitiva](https://twitter.com/jahirfiquitiva)
- Byron Herrera - [@silenceway](https://twitter.com/silenceway)
- Neider Tapia Avila - [@nrtapia](https://twitter.com/nrtapia)
- Andres Zapata Cano - [@andfelzapata](https://twitter.com/andfelzapata)
- Steven Rafael Gonzalez Machado - [@srgm86](https://twitter.com/srgm86)
- Julian Duque - [@julian_duque](https://twitter.com/julian_duque)
- Daniel Estrada Aristizábal
