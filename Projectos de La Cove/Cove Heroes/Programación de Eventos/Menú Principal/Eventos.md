# Info
Este es el código del menú principal entero de Cove Heroes, para leerlo con más comodidad, selecciona arriba para verlo en "Raw" u "Original"
# Pre-Carga
◆Comando de plugin：mv3d disable
◆Mensaje：Nada, Fondo oscuro, Central
：       ：<CENTER>\C[14]
：       ：\>Utiliza las teclas Z o Enter o Espacio para interactuar
：       ：\>Usa las flechas del teclado para moverte por los menús, el mouse no funciona
◆Mensaje：Nada, Fondo oscuro, Central
：       ：<CENTER>\C[14]
：       ：\>Ten en cuenta que los programas de grabación no se llevan
：       ：\>bien con Cove Heroes, habrán bajones de FPS con Movavi Screen Recorder,
：       ：\>Bandicam y Action. OBS Parece ser compatible
◆Mostrar imagen：#1, Nada, Centro (640,620), (75%,75%), 255, Normal
◆Script：Galv.PIC.anim(1,121);
◆Mensaje：Nada, Fondo oscuro, Central
：       ：<CENTER>\C[14]
：       ：\>Cuando aparezca el Kirby fachero en la pantalla significa
：       ：\>que la canción que estás escuchando es temporal
：       ：\>\}(La del menú principal también es temporal, pero no puedo poner al kirby ahi xd)
◆Script：Galv.PIC.stopAnim(1)
◆Esperar：1 fotograma
◆Borrar imagen：#1
◆Reproducir BGM：BETA_Casin_That_ass (100, 100, 0)
◆Mensaje：Nada, Fondo oscuro, Central
：       ：<CENTER>\C[14]
：       ：\>Recuerda que estas versiones son versiones In-Dev
：       ：\>\C[10]Todo el contenido puede ser y será modificado en un futuro\.\.\.\.\.\.\.\.\.\.\.\.\.\.\^
◆Control de interruptores：#0007 CURVA DE ANIMÁTICA = OFF
◆Transportar al jugador：MENÚ PRINCIPAL (7,5)
	
	
	
# Carga de la interfaz del menú principal
◆Mostrar imagen：#99, ui_black, Superior izquierda (0,0), (100%,100%), 255, Normal
◆Cambiar fondo del mapa：Ocean1 (Bucle horizontal)
◆Mover imagen：#99, Superior izquierda (0,0), (100%,100%), 0, Normal, 60 fotogramas
◆Mostrar imagen：#1, ui_selected_1, Superior izquierda (-30,350), (100%,100%), 0, Normal
◆Mostrar imagen：#2, ui_story_1, Superior izquierda (-30,350), (100%,100%), 0, Normal
◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-30,400), (100%,100%), 0, Normal
◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-30,450), (100%,100%), 0, Normal
◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-30,500), (100%,100%), 0, Normal
◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-30,550), (100%,100%), 0, Normal
◆Mostrar imagen：#7, ui_logo, Superior izquierda (0,8), (100%,100%), 0, Normal
◆Mover imagen：#7, Superior izquierda (0,0), (100%,100%), 255, Normal, 50 fotogramas
◆Mover imagen：#1, Superior izquierda (0,350), (100%,100%), 255, Normal, 60 fotogramas
◆Mover imagen：#2, Superior izquierda (0,350), (100%,100%), 255, Normal, 60 fotogramas
◆Esperar：10 fotogramas
◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 60 fotogramas
◆Esperar：10 fotogramas
◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 60 fotogramas
◆Esperar：10 fotogramas
◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 60 fotogramas
◆Esperar：10 fotogramas
◆Mover imagen：#7, Superior izquierda (0,10), (100%,100%), 255, Normal, 60 fotogramas
◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 60 fotogramas (Esperar)
◆Borrar imagen：#99
◆Mostrar imagen：#27, current_version, Superior izquierda (0,0), (100%,100%), 0, Normal
◆Mover imagen：#27, Superior izquierda (0,0), (100%,100%), 255, Normal, 60 fotogramas
◆Mostrar imagen：#52, gr_1, Superior izquierda (0,0), (100%,100%), 0, Aditivo
◆Mostrar imagen：#53, gr_2, Superior izquierda (0,0), (100%,100%), 0, Aditivo
◆Control de interruptores：#0001 MENU PRINCIPAL CARGADO = ON



# Bucle infinito de la animación del logo
◆Mover imagen：#7, Superior izquierda (0,0), (100%,100%), 255, Normal, 40 fotogramas (Esperar)
◆Mover imagen：#7, Superior izquierda (0,8), (100%,100%), 255, Normal, 40 fotogramas (Esperar)
◆Comentario：Son 60 fotogramas
	

	
# Revelar interfaz
◆Esperar：200 fotogramas
◆Mover imagen：#25, Superior izquierda (0,20), (100%,100%), 0, Normal, 30 fotogramas (Esperar)
◆Borrar imagen：#25



# Bucle infinito de la animación de los rayos solares
◆Mover imagen：#52, Superior izquierda (0,0), (100%,100%), 255, Aditivo, 75 fotogramas
◆Mover imagen：#53, Superior izquierda (0,0), (100%,100%), 0, Aditivo, 75 fotogramas (Esperar)
◆Mover imagen：#52, Superior izquierda (0,0), (100%,100%), 0, Aditivo, 75 fotogramas
◆Mover imagen：#53, Superior izquierda (0,0), (100%,100%), 255, Aditivo, 75 fotogramas (Esperar)
◆Comentario：Son 150 Fotogramas



# Limitador para evitar que se salga de los valores máximos y mínimo el selector de UI
◆Si：Menú seleccionado ≤ 0
  ◆Control de variables：#0001 Menú seleccionado = 1
  ◆
：Fin
◆Si：Menú seleccionado ≥ 6
  ◆Control de variables：#0001 Menú seleccionado = 5
  ◆
：Fin



# Renderizado del botón seleccionado
◆Si：Se ha pulsado el botón [Arriba]
  ◆Control de variables：#0001 Menú seleccionado -= 1
  ◆Reproducir SE：Cursor2 (90, 100, 0)
  ◆Si：Menú seleccionado = 1
    ◆Mostrar imagen：#2, ui_story_1, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (0,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 2
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_1, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (0,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 3
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_1, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (0,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 4
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_1, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (0,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 5
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_1, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (0,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Esperar：10 fotogramas
  ◆
：Fin
◆Si：Se ha pulsado el botón [Abajo]
  ◆Control de variables：#0001 Menú seleccionado += 1
  ◆Reproducir SE：Cursor2 (90, 100, 0)
  ◆Si：Menú seleccionado = 1
    ◆Mostrar imagen：#2, ui_story_1, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (0,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 2
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_1, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (0,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 3
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_1, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (0,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 4
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_1, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_0, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (0,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (-25,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 5
    ◆Mostrar imagen：#2, ui_story_0, Superior izquierda (-25,350), (100%,100%), 255, Normal
    ◆Mostrar imagen：#3, ui_multiplayer_0, Superior izquierda (-25,400), (100%,100%), 255, Normal
    ◆Mostrar imagen：#4, ui_options_0, Superior izquierda (-25,450), (100%,100%), 255, Normal
    ◆Mostrar imagen：#5, ui_extra_0, Superior izquierda (-25,500), (100%,100%), 255, Normal
    ◆Mostrar imagen：#6, ui_exit_1, Superior izquierda (-25,550), (100%,100%), 255, Normal
    ◆Mover imagen：#2, Superior izquierda (-25,350), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#3, Superior izquierda (-25,400), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#4, Superior izquierda (-25,450), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#5, Superior izquierda (-25,500), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#6, Superior izquierda (0,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆Mover imagen：#1, Superior izquierda (0,550), (100%,100%), 255, Normal, 10 fotogramas
    ◆
  ：Fin
  ◆Esperar：10 fotogramas
  ◆
：Fin



# Procesado del menú
◆Si：Se ha pulsado el botón [Aceptar]
  ◆Si：Menú seleccionado = 1
    ◆Control de interruptores：#0002 Interfaz Bloqueada = ON
    ◆Mostrar elecciones：\I[2245]Campañas guardadas, \I[70]Nueva Campaña, \I[74]Atrás (Fondo oscuro, En el centro, #1, #3)
    ：Cuando \I[2245]Campañas guardadas 
      ◆Script：SceneManager.push(Scene_Load)
      ◆
    ：Cuando \I[70]Nueva Campaña 
      ◆Mensaje：Nada, Fondo oscuro, Central
      ：       ：¿Seguro que quieres crear una nueva campaña?
      ：       ：
      ：       ：No se sobreescribirá ninguna partida anterior
      ◆Mostrar elecciones：\I[90]Sí, \I[91]No (Fondo oscuro, En el centro, #1, #2)
      ：Cuando \I[90]Sí 
        ◆Mostrar imagen：#99, ui_black, Superior izquierda (0,0), (100%,100%), 0, Normal
        ◆Iniciar transición
        ◆Mover imagen：#99, Superior izquierda (0,0), (100%,100%), 255, Normal, 60 fotogramas (Esperar)
        ◆Esperar：60 fotogramas
        ◆Borrar imagen：#1
        ◆Borrar imagen：#2
        ◆Borrar imagen：#3
        ◆Borrar imagen：#4
        ◆Borrar imagen：#5
        ◆Borrar imagen：#6
        ◆Borrar imagen：#7
        ◆Borrar imagen：#99
        ◆Borrar imagen：#52
        ◆Borrar imagen：#53
        ◆Transportar al jugador：CREACIÓN DE NUEVA PARTIDA (8,6)
        ◆
      ：Cuando \I[91]No 
        ◆
      ：Fin
      ◆
    ：Cuando \I[74]Atrás 
      ◆
    ：Fin
    ◆Esperar：10 fotogramas
    ◆Control de interruptores：#0002 Interfaz Bloqueada = OFF
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 2
    ◆Control de interruptores：#0002 Interfaz Bloqueada = ON
    ◆Mensaje：ui_icons(4), Fondo oscuro, Central
    ：       ：Menú pendiente
    ◆Esperar：10 fotogramas
    ◆Control de interruptores：#0002 Interfaz Bloqueada = OFF
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 3
    ◆Control de interruptores：#0002 Interfaz Bloqueada = ON
    ◆Etiqueta：opciones
    ◆Mostrar elecciones：\I[2323]Jugabilidad, \I[91]Opciones de Sonido, \I[2344]Configuración de Red, \I[74]Atrás (Fondo oscuro, En el centro, #1, #4)
    ：Cuando \I[2323]Jugabilidad 
      ◆
    ：Cuando \I[91]Opciones de Sonido 
      ◆Mensaje：Nada, Fondo oscuro, Central
      ：       ：No se puede configurar aún ewe
      ◆Ir a etiqueta：opciones
      ◆
    ：Cuando \I[2344]Configuración de Red 
      ◆Mensaje：Nada, Fondo oscuro, Central
      ：       ：No se puede configurar aún ewe
      ◆Ir a etiqueta：opciones
      ◆
    ：Cuando \I[74]Atrás 
      ◆
    ：Fin
    ◆Esperar：10 fotogramas
    ◆Control de interruptores：#0002 Interfaz Bloqueada = OFF
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 4
    ◆Control de interruptores：#0002 Interfaz Bloqueada = ON
    ◆Mostrar elecciones：\I[193]Créditos, \I[121]Logros, \I[84]Contactar, \I[74]Atrás (Fondo oscuro, En el centro, #1, #4)
    ：Cuando \I[193]Créditos 
      ◆Mostrar imagen：#88, ui_black, Superior izquierda (0,0), (100%,100%), 0, Normal
      ◆Mover imagen：#88, Superior izquierda (0,0), (100%,100%), 200, Normal, 60 fotogramas
      ◆Texto(s)：Velocidad 2
      ：        ：Créditos \}(Puedes acelerarlos con el enter)\{
      ：        ：
      ：        ：Historia
      ：        ：      Nadie qwq
      ：        ：
      ：        ：Programación de eventos
      ：        ：      FoxyThePirate2704 (Fox Zarz)
      ：        ：
      ：        ：Diseño de Mapas
      ：        ：      FoxyThePirate2704 (Fox Zarz)
      ：        ：
      ：        ：Testeo de In-Devs
      ：        ：      Nadie qwq
      ：        ：
      ：        ：Música
      ：        ：      Menú Principal
      ：        ：            Casin that ass, glue70 vs Eminem
      ：        ：
      ：        ：Agradecimientos especiales
      ：        ：      Creadores de Plugins
      ：        ：            Alpha1128
      ：        ：            GALV's
      ：        ：            HIME
      ：        ：            Attelier Rigss
      ：        ：            OcRam
      ：        ：            SumRandomDude
      ：        ：            Yanfly
      ：        ：      Amigos y familiares de:
      ：        ：            KinG
      ：        ：            KinS
      ：        ：            ComandanteAnime
      ：        ：            AlphaGamer
      ：        ：            TheGoLdZWarrior
      ：        ：            Mangle
      ：        ：            Izael
      ：        ：            WilliamAfton
      ：        ：            Bonnes
      ：        ：            MakoWa
      ：        ：            LilPizza
      ：        ：            DreamBoy
      ：        ：            Joseivan
      ：        ：            KazuhoRen
      ：        ：            Faz
      ：        ：            Samy
      ：        ：            
      ：        ：            Y todos aquellos que alguna vez
      ：        ：            supieron del proyecto y me apoyaron
      ：        ：            
      ：        ：      Desarrollador del motor "RPG Maker MV 1.6.1"
      ：        ：            KADOKAWA™\}
      ：        ：
      ：        ：     Parte de las assets de este videojuego, como sonidos y
      ：        ：     texturas son provenientes de los recursos por defectos
      ：        ：                 ofrecidos por RPG Maker MV 1.6.1
      ：        ：
      ：        ：
      ：        ：       \{\{\{     ¡Gracias por jugar!
      ◆Mover imagen：#88, Superior izquierda (0,0), (100%,100%), 0, Normal, 60 fotogramas (Esperar)
      ◆Borrar imagen：#88
      ◆
    ：Cuando \I[121]Logros 
      ◆Mensaje：ui_icons(4), Fondo oscuro, Central
      ：       ：Eso no ha sido programado aún :I
      ◆
    ：Cuando \I[84]Contactar 
      ◆Mensaje：ui_icons(5), Fondo oscuro, Central
      ：       ：Puedes contactar con el equipo de desarrolladores y testers
      ：       ：a través de \C[10]Joven Club\C[0] en el TeamSpeak Esteria no Sekai
      ：       ：
      ：       ：¿Quieres que se abra tu TeamSpeak automáticamente en ese servidor?
      ◆Mostrar elecciones：\I[90]Conectarse a Esteria no Sekai, \I[91]No conectarse (Fondo oscuro, En el centro, #1, #2)
      ：Cuando \I[90]Conectarse a Esteria no Sekai 
        ◆Mensaje：ui_icons(5), Fondo oscuro, Central
        ：       ：Se vá a abrir una ventana en blanco y luego te conectarás
        ：       ：a Esteria, puedes cerrar la ventana una vez te conectes
        ：       ：Si no sabes en específico quien de los desarrolladores hizo
        ：       ：algo, consulta los créditos para conocer que hace cada quién.
        ◆Mostrar elecciones：¡Vale! (Fondo oscuro, En el centro, #1, -)
        ：Cuando ¡Vale! 
          ◆Comando de plugin：OpenNewWindow ts3server://10.96.65.3?port=5555
          ◆
        ：Fin
        ◆
      ：Cuando \I[91]No conectarse 
        ◆
      ：Fin
      ◆
    ：Cuando \I[74]Atrás 
      ◆
    ：Fin
    ◆Esperar：10 fotogramas
    ◆Control de interruptores：#0002 Interfaz Bloqueada = OFF
    ◆
  ：Fin
  ◆Si：Menú seleccionado = 5
    ◆Control de interruptores：#0002 Interfaz Bloqueada = ON
    ◆Mensaje：Nada, Fondo oscuro, Central
    ：       ：¿Seguro que quieres salir del juego?
    ◆Mostrar elecciones：\I[90]Sí, \I[91]No (Fondo oscuro, En el centro, #1, #2)
    ：Cuando \I[90]Sí 
      ◆Finalizar BGM：1 segundo
      ◆Mostrar imagen：#99, ui_black, Superior izquierda (0,0), (100%,100%), 0, Normal
      ◆Mover imagen：#99, Superior izquierda (0,0), (100%,100%), 255, Normal, 60 fotogramas (Esperar)
      ◆Esperar：20 fotogramas
      ◆Comando de plugin：ForceClose
      ◆
    ：Cuando \I[91]No 
      ◆
    ：Fin
    ◆Esperar：10 fotogramas
    ◆Control de interruptores：#0002 Interfaz Bloqueada = OFF
    ◆
  ：Fin
  ◆
：Fin
