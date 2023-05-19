<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="fade-down-right")
      .titulo-principal__numero.text-white
        span 1
      h1 Verificación y optimización de <em>assets</em>
    .row.justify-content-center(data-aos="fade-down-right")
      .col-lg-10.col-md-12
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img.cambioimg(
            :style="{'background-image': `url(${require('@/assets/curso/tema1/img1.jpg')})`}"
          )
          .bloque-texto-g__texto.cambiotexto.px-4.py-5
            p.mb-0 Las partes gráficas de un videojuego  pueden tener injerencia en dos sistemas del cómputo: el GPU o el CPU; y  la primera regla de optimización es en encontrar dónde está el problema de rendimiento para determinar las estrategias que se utilizarán en la optimización de todos los recursos del videojuego.
    Separador
    #t_1_1.titulo-segundo.color-acento-contenido(data-aos="fade-down-right")
      h2 1.1 Métricas de rendimiento
    p(data-aos="fade-down-right") En términos generales, las métricas de rendimiento involucran procedimientos, técnicas y tecnologías que permiten realizar seguimiento del rendimiento del sistema, entendiendo este último, en el desarrollo de videojuegos, como el videojuego en sí mismo, como aplicación de <em>software</em>.
    p.mb-4(data-aos="fade-down-right") En el motor de videojuegos Unity3D, se puede encontrar una herramienta global denominada #[b Unity Profiler] que reúne diferentes subherramientas para determinar métricas de rendimiento en tiempo real, mientras se ejecuta un videojuego en tiempo de ejecución en modo edición. Cada una de estas herramientas brindan información detallada del comportamiento de diversos elementos y aspectos a manera de indicadores que permiten determinar un perfil general de rendimiento.
    .row.justify-content-center.mb-4(data-aos="fade-down-right")
      .col-lg-10.col-md-12
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5.mb-4
          .bloque-texto-g__img.cambioimg(
            :style="{'background-image': `url(${require('@/assets/curso/tema1/img2.jpg')})`}"
          )
          .bloque-texto-g__texto.cambiotexto.px-4.py-5
            span.mb-0.text-bold Unity Profiler: 
            span es una herramienta que se puede utilizar para obtener información sobre el rendimiento de la aplicación. Se puede conectar a dispositivos en la red o conectados a la máquina para probar cómo se ejecuta la  aplicación en la plataforma de lanzamiento prevista. También puede ejecutarlo en el editor para obtener una descripción general de la asignación de recursos mientras desarrolla la aplicación.
    .tarjeta--container.row.mb-5
      .col-md.tarjeta.color-primario.p-5(data-aos="fade-down-right")
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema1/fig1.svg')
          
        p.text-dark #[b.text-dark Unity Profiler] recopila y muestra datos sobre el rendimiento de su aplicación en áreas como la CPU, la memoria, el renderizador y el audio. Es una herramienta útil para identificar áreas de mejora del rendimiento en su aplicación e iterar en esas áreas. Puede identificar cosas como su código, recursos activos, configuraciones de escena, renderizado de cámara y configuraciones de compilación que pueden y afectan el rendimiento de su aplicación. Muestra los resultados en una serie de gráficos para visualizar dónde ocurren los picos en el rendimiento de su aplicación.

      .col-md.tarjeta.color-acento-contenido.p-5(data-aos="fade-down-left")
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema1/fig2.svg')
        p.text-white Además de utilizar #[b Unity Profiler] integrado, puede utilizar la #[b API Profiler] de complemento nativo de bajo nivel para exportar datos de creación de perfiles a herramientas de creación de perfiles de terceros, y el paquete #[b Profiling Core] para personalizar su análisis de creación de perfiles. También puede agregar potentes herramientas de creación de perfiles, como #[b Memory Profiler] y #[b Profile Analyzer] a su proyecto para analizar los datos de rendimiento con más detalle.
    p(data-aos="fade-down-right") Para acceder a la ventana Unity Profiler vaya al menú: 
    p.mb-4(data-aos="fade-down-right") <em>Window > Analysis > Profiler</em>
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b #[i Figura 1]]
      p.mb-0 Ventana Profiler
    img(data-aos="fade-down-right").mb-5(src='@/assets/curso/tema1/img3.jpg')
    .tarjeta--container.row.mb-5
      .col-md.tarjeta.color-primario.p-5(data-aos="fade-down-right")
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema1/fig3.png')
        p.text-dark.text-center El generador de perfiles registra varias áreas del rendimiento de su aplicación y le muestra esa información. Puede utilizar esta información para tomar decisiones informadas sobre lo que podría necesitar optimizar en su aplicación y para confirmar que sus optimizaciones producen los resultados que espera.
      .col-md.tarjeta.color-acento-contenido.p-5(data-aos="fade-down-left")
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema1/fig4.svg')
        p.text-white.text-center De forma predeterminada, Unity Profiler registra y mantiene los últimos 300 fotogramas del juego y muestra información detallada sobre cada fotograma. Puede aumentar el número de fotogramas que registra en la ventana de Preferencias (menú: <em>Edit > Preferences</em>), hasta 2.000 fotogramas. 
    .cajon.color-primario.fondo-cajon.p-4.mb-4(data-aos="fade-down-right")
      h4 Nota:
      p si aumenta esta configuración a una gran cantidad de fotogramas, la sobrecarga del generador de perfiles y el uso de la memoria pueden aumentar el rendimiento.
    .row.justify-content-center.mb-4(data-aos="fade-down-right")
      .col-lg-10.col-md-12
        p Puede inspeccionar el código de la secuencia de comandos y cómo su aplicación usa ciertos activos y recursos que podrían estar ralentizándola. También puede comparar el rendimiento de su aplicación en diferentes dispositivos. Esta herramienta tiene varios Módulos de Perfilado diferentes que puede agregar a su sesión de creación de perfiles para obtener más información sobre áreas como renderizado, memoria y audio.
    p.mb-5(data-aos="fade-down-right") Para saber más acerca de la ventana de Unity Profiler, se invita a ver el siguiente video.
    .row.justify-content-center
      .col-lg-10
        figure.mb-5(data-aos="fade-down")
          .video
            iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    ol.lista-ol--cuadro.mb-5
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span a
        | #[b Diseño de la ventana del generador de perfiles]
    ImagenInfografica.color-acento-botones.mb-5(data-aos="fade-down-right")
      template(v-slot:imagen)
        figure
          img(src='@/assets/curso/tema1/img3.png')
      .tarjeta.fondo-4.p-3(x="8.3%" y="2.3%" numero="A")
        .h5.mb-2 A: Módulos de perfilado. 
        p Esta es una lista de todos los módulos que puede perfilar en su aplicación. Utilice el menú desplegable en la parte superior de esta área para agregar y eliminar módulos de la ventana.
      .tarjeta.fondo-4.p-3(x="17.6%" y="2.3%" numero="B")
        .h5.mb-2 B: Controles del generador de perfiles. 
        p Utilice estos controles para establecer desde qué dispositivo crear un perfil y qué tipo de creación de perfiles debe realizar Unity, navegar entre los fotogramas y comenzar a registrar datos.
      .tarjeta.fondo-4.p-3(x="13%" y="7%" numero="C")
        .h5.mb-2 C: Diagramas de cuadros. 
        p Esta área contiene gráficos de cada módulo, los perfiles de Unity Profiler. Esta área está en blanco cuando abre el generador de perfiles por primera vez y se llena de información cuando comienza a crear perfiles de su aplicación.
      .tarjeta.fondo-4.p-3(x="10.4%" y="72%" numero="D")
        .h5.mb-2 D: Panel de detalles del módulo. 
        p La información en esta área de la ventana cambia según el módulo que haya seleccionado. Por ejemplo, cuando selecciona el módulo CPU Usage Profiler, contiene una línea de tiempo detallada y la opción de cambiar a una vista de jerarquía. Cuando selecciona el módulo Rendering Profiler, esta área muestra una lista de información de depuración. Esta área está en blanco cuando abre el generador de perfiles por primera vez y se llena de información al crear perfiles de su aplicación.
    ol.lista-ol--cuadro.mb-5
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span b
        | #[b Preferencias del generador de perfiles]
    p.mb-4(data-aos="fade-down-right") La ventana Preferencias contiene configuraciones adicionales de la ventana <i>Unity Profiler</i> de la siguiente manera:
    .titulo-sexto.color-acento-contenido.mb-3(data-aos="fade-down-right")
      p.mb-0 #[b #[i Tabla 1]]
      p.mb-0 Ventana de preferencias
    .tabla-c.mb-5(data-aos="fade-down-right")
      table
        tr.fondo-5.text-white.text-center
          td.ancho-col 
            h4.mb-0 Preferencia
          th 
            h4.mb-0 Descripción
        tr
          td.text-center <em>Frame count</em>
          td Establece el número máximo de fotogramas que debe capturar <i>Profiler</i>, que puede ser entre 300 y 2.000.
        tr
          td.text-center <i>Show stats for 'current frame'</i>
          td De forma predeterminada, cuando se selecciona el botón Cuadro actual e ingresa al modo Cuadro actual, la línea indicadora del cuadro no tiene anotaciones con las estadísticas del cuadro actual. Esto se debe a que las anotaciones de estadísticas pueden dificultar la visualización de datos en tiempo real. Para mostrar las anotaciones, se debe habilitar esta configuración.
        tr
          td.text-center <i>Default recording state</i>
          td Se selecciona en qué estado de grabación debe abrirse el generador de perfiles, se puede elegir entre Activado, Desactivado o Recordar. Habilitado mantiene el botón Grabar habilitado entre sesiones, mientras que Deshabilitado lo deshabilita, independientemente de si se enciende o apaga durante la sesión de creación de perfiles. El estado Recordar indica si se ha habilitado o deshabilitado el botón Grabar durante la sesión y lo mantiene en su último estado la próxima vez que se abra la ventana del Generador de perfiles.
        tr
          td.text-center <i>Default editor target mode</i>
          td Se establece el modo al que debe dirigirse el menú desplegable Adjuntar al jugador de forma predeterminada. Elegir entre el Modo de reproducción o el Editor.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span c
        | #[b Módulos de perfilador]
    p(data-aos="fade-down-right") La parte superior de la ventana Profiler está dividida en módulos de perfilador que perfilan áreas específicas de tu juego. Cuando crea un perfil de la aplicación, Unity muestra los datos relacionados con cada módulo en los gráficos correspondientes.
    p(data-aos="fade-down-right") El módulo de uso de CPU proporciona la mejor descripción general de cuánto tiempo pasa la aplicación en cada marco. Los otros módulos recopilan datos más específicos y pueden ayudar a inspeccionar áreas más específicas o monitorear los aspectos vitales de la aplicación, como el consumo de memoria, la representación o las estadísticas de audio.
    p.mb-4(data-aos="fade-down-left") A continuación, se presentan estos módulos en la siguiente tabla.
    .titulo-sexto.color-acento-contenido.mb-3(data-aos="fade-down-right")
      p.mb-0 #[b #[i Tabla 2]]
      p.mb-0 Módulos
    .tabla-c.mb-5(data-aos="fade-down-right")
      table
        tr.fondo-5.text-white.text-center
          td.ancho-col 
            h4.mb-0 <i>Profiler Module</i>
          th 
            h4.mb-0 Función
        tr
          td.text-center 
            h5 CPU Usage
          td Muestra una descripción general de dónde pasa la mayor parte del tiempo la aplicación, en áreas como física, <i>scripts</i>, animación y recolección de basura. Este módulo contiene información amplia de perfiles sobre la aplicación y se puede usar para decidir qué módulos adicionales usar para investigar problemas más específicos en la aplicación. Este módulo siempre está activo, incluso si se cierra; se debe consultar el módulo de perfilador de uso de CPU.
        tr
          td.text-center 
            h5 GPU Usage
          td Muestra información relacionada con el procesamiento de gráficos. De forma predeterminada, este módulo no está activo, porque tiene una sobrecarga alta.
        tr
          td.text-center 
            h5 Rendering
          td Muestra información sobre cómo Unity renderiza gráficos en la aplicación, incluida información sobre lotes estáticos y dinámicos, llamadas SetPass y Draw, triángulos y vértices.
        tr
          td.text-center 
            h5 Memory
          td Indica la información sobre cómo Unity asigna memoria en la aplicación. Esto es particularmente útil para ver cómo las asignaciones de secuencias de comandos (GC.Alloc) conducen a la recolección de basura, o cómo las tendencias de uso de la memoria de activos de la aplicación a lo largo del tiempo.
        tr
          td.text-center 
            h5 Audio
          td Muestra información relacionada con el audio en la aplicación, como cuándo y cuántas fuentes de audio se reproducen, cuánto uso de CPU requiere el sistema de audio y cuánta memoria le asigna Unity.
        tr
          td.text-center  
            h5 Video
          td Muestra información relacionada con el video en la aplicación.
        tr
          td.text-center  
            h5 Physics
          td Brinda información sobre la física de la aplicación que ha procesado el motor de física.
        tr
          td.text-center  
            h5 Physics (2D)
          td Similar al módulo Physics Profiler, este módulo muestra información sobre dóndel motor de física ha procesado la física 2D en la aplicación.
        tr
          td.text-center  
            h5 Network Messages (#[i deprecated])
          td Da información sobre paquetes y mensajes de nivel inferior enviados o recibidos por la API de alto nivel multijugador.
        tr
          td.text-center  
            h5 Network Operations (#[i deprecated])
          td Muestra información detallada sobre qué tipos de operaciones se encuentran en los mensajes enviados y recibidos por la API de alto nivel multijugador, como cuántas SyncVars o Comandos se han transferido.
        tr
          td.text-center  
            h5 UI
          td Muestra información sobre cómo Unity maneja el procesamiento por lotes de la interfaz de usuario para la aplicación, incluido por qué y cómo Unity procesa los elementos por lotes.
        tr
          td.text-center  
            h5 UI Details
          td De manera similar al módulo de la interfaz de usuario, el gráfico de este módulo agrega datos sobre el recuento de lotes y vértices, así como marcadores que incluyen información sobre los eventos de entrada del usuario que activan los cambios de la interfaz de usuario.
        tr
          td.text-center  
            h5 Global Illumination
          td Evidencia la información sobre la cantidad de recursos de CPU que Unity gasta en el subsistema de iluminación de iluminación global de la aplicación.
        tr
          td.text-center  
            h5 Virtual Texturing
          td Muestra estadísticas sobre la transmisión de texturas virtuales en la aplicación.
    .cajon.color-primario.fondo-cajon.p-4.mb-4(data-aos="fade-down-right")
      p.m-0 Cada módulo tiene su propio gráfico. Cuando selecciona un módulo, aparece un panel Detalles del módulo en la sección inferior de la ventana que se puede usar para inspeccionar los datos detallados que recopila el módulo.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span d
        | #[b Método de perfilación de una aplicación]
    p.m-4(data-aos="fade-down-right") Cuando se usa Unity Profiler para perfilar la aplicación, hay dos formas principales de registrar datos:
    .tarjeta.tarjeta--azul.fondo-6.p-4.mb-5(data-aos="fade-down-right") 
      SlyderA
        .row.justify-content-center
          .col-lg-5.col-md-10.col-sm-10.col-10.mb-4.mb-md-0
            p Para perfilar su aplicación en su plataforma de lanzamiento de destino, conecte el dispositivo de destino a su red o directamente a su computadora mediante un cable. También puede conectarse a un dispositivo a través de la dirección IP, solo puede crear un perfil de su aplicación como una compilación de desarrollo. 
            p Para configurar esto, vaya a Configuración de compilación (menú: <i>File > Build Settings</i>) y seleccione la plataforma de destino de su aplicación. Habilite la configuración de Development Build. Cuando habilita esta configuración, dos configuraciones relacionadas con Profiler están disponibles: Autoconnect Profiler y Deep Profiling Support.
            a.boton.color-acento-botones.indicador__container.mb-4(@click="modal1 = true")
              span Ampliar imagen
              i.fas.fa-magnifying-glass
              .indicador--click(v-if="mostrarIndicador")
          .col-lg-5.col-md-11.col-sm-12.col-12.mb-5
            .row.justify-content-center
              .col-auto.fondo-7.px-4.py-2
                .titulo-sexto.color-acento-contenido.mb-0
                  p.mb-0 #[b #[i Figura 2]]
                  p.mb-0 Ventana de dialogo Build Settings
            figure.mb-4
              img(src='@/assets/curso/tema1/img4.png')
        .row.justify-content-center
          .col-lg-5.col-md-10.col-sm-10.col-10.mb-4.mb-md-0.ps-4.ps-sm-0
            p Cuando cambia el objetivo de Profiler a Editor, todas las muestras que estaban previamente ocultas bajo el marcador EditorLoop contribuyen a sus respectivas categorías. Esto significa que la información en el panel de detalles del módulo CPU Profiler y sus gráficos cambia significativamente. Para perfilar los tiempos de inicio del Editor, inicie el Editor con la opción de línea de Comando > Profiler > Enable.
            p Para reducir el impacto que tiene la ventana del generador de perfiles en el rendimiento del editor, puede utilizar el generador de perfiles independiente, que abre la ventana del generador de perfiles en su propio proceso. Esto es especialmente útil si selecciona el Editor como el objetivo de creación de perfiles, o si está creando perfiles profundos en su aplicación, porque la ventana del generador de perfiles, normalmente, utiliza recursos que pueden sesgar los datos de rendimiento.
            a.boton.color-acento-botones.indicador__container.mb-4(@click="modal2 = true")
              span Ampliar imagen
              i.fas.fa-magnifying-glass
              .indicador--click(v-if="mostrarIndicador")
          .col-lg-5.col-md-11.col-sm-12.col-12.mb-5
            .row.justify-content-center
              .col-auto.fondo-7.px-4.py-2
                .titulo-sexto.color-acento-contenido.mb-0(data-aos="fade-down-right")
                  p.mb-0 #[b #[i Figura 3]]
                  p.mb-0 Ventana Editor <i>Features</i>
            figure.mb-4
              img(src='@/assets/curso/tema1/img5.png')
      ModalA(:abrir-modal.sync="modal1")
        .row.align-items-center
          .col-md-10.col-12.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema1/img4.png')
      ModalA(:abrir-modal.sync="modal2")
        .row.align-items-center
          .col-md-10.col-12.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema1/img5.png')
    p.mt-4(data-aos="fade-down-right") La mejor manera de obtener tiempos precisos sobre la aplicación es perfilarla en la plataforma final en la que se desea publicar, así se sabrá lo que puede afectar el rendimiento de la aplicación.
    p.mb-5(data-aos="fade-down-right") Sin embargo, puede llevar mucho tiempo crear la aplicación cada vez que se deseen mejorar elementos del rendimiento, por lo tanto, para evaluar rápidamente el rendimiento de la aplicación, se puede perfilar directamente en el modo Reproducir en el Editor. La creación de perfiles en el modo de reproducción no brinda un reflejo preciso de cómo se ve el rendimiento de la aplicación en un dispositivo real, pero sí es útil para verificar rápidamente si los cambios que realiza mejoran el rendimiento de la aplicación después de la creación de perfiles inicialmente en la plataforma final.
    .cajon.color-primario.fondo-cajon.p-4.mb-5(data-aos="fade-down-right")
      p.m-0 Unity Editor puede afectar el rendimiento de la aplicación, ya que usa los mismos recursos que la aplicación cuando se ejecuta en modo Play, por lo que también puede crear un perfil del Editor por separado para determinar qué recursos usa. Esto es particularmente útil si la aplicación solo ha sido diseñada para funcionar en el modo Reproducir, como para hacer películas.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span e
        | #[b  Mejores prácticas para perfilar la aplicación]
    p.mb-4(data-aos="fade-down-right") Cuando se crea un perfil de la aplicación, hay algunas cosas que puede hacer para garantizar la coherencia entre las sesiones de creación de perfiles y para asegurarse de que los procesos que utiliza Unity no afecten los datos de creación de perfiles:
    AcordionA(data-aos="fade-down-right").mb-5(tipo="a" clase-tarjeta="tarjeta fondo-8 otrofondo")
      .row.justify-content-around(titulo="Configuración de los módulos de perfilado")
        .col-lg-11.mb-4
          figure
            img(src='@/assets/curso/tema1/img6.png')
        .col-lg-11.mb-4.mb-md-0
          p Agregue los módulos de Unity Profiler relacionados con el área que desea investigar a la ventana de la herramienta. Para agregar y quitar módulos al generador de perfiles, seleccione el menú desplegable en la parte superior izquierda de la ventana del generador de perfiles Profiler Modules. Se desplegará un cuadro de opciones donde podrá habilitar o deshabilitar los módulos que se deseen.

      .row.justify-content-around(titulo="Habilitación de la configuración de pilas de llamadas")
        .col-lg-5.mb-4.mb-md-0
          p Evite el uso de perfiles profundos, ya que crea una gran sobrecarga cuando lo usa. Si desea ver más detalles sobre muestras con marcadores como GC.Alloc o JobFence.Complete, navegue hasta la barra de herramientas de la ventana Profiler y habilite la configuración de Pilas de llamadas. Esto proporciona la pila de llamadas completa de la muestra que le brinda la información que necesita sin incurrir en la sobrecarga de la creación de perfiles profundos.
        .col-lg-6
          figure
            img(src='@/assets/curso/tema1/img7.png')
      .row.justify-content-around(titulo="Habilitar o deshabilitar Profiler")
        .col-lg-11.mb-4.mb-md-0
          p Utilice el acceso directo F9 para habilitar o deshabilitar Profiler. Puede utilizar este acceso directo para capturar datos de rendimiento sin necesidad de abrir la ventana. Si tiene abierto el generador de perfiles independiente y al usar este acceso directo se inicia la grabación en esta ventana.
    p.mb-4(data-aos="fade-down-right") Se puede conocer más acerca de la configuración del Profiler en el siguiente video.
    figure.mb-5(data-aos="fade-down")
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)    
    Separador
    #t_1_2.titulo-segundo.color-acento-contenido(data-aos="fade-down-right")
      h2 1.2 Optimización de archivos de salida
    .row.justify-content-center.mb-4(data-aos="fade-down-right")
      .col-lg-10.col-md-12
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img.cambioimg(
            :style="{'background-image': `url(${require('@/assets/curso/tema1/img8.jpg')})`}"
          )
          .bloque-texto-g__texto.cambiotexto.px-4.py-5
            p.mb-0 La optimización comprende tanto técnicas como procedimientos, que deben hacerse desde el momento mismo de diseño y construcción de los elementos del videojuego. Como es sabido, los elementos del videojuego comprenden elementos gráficos y visuales en 2D y 3D, elementos de sonido, como voces de diálogos, efectos de sonido, música y sonido ambiente, elementos de código, que son los conjuntos de archivos de código escritos por el desarrollador y los comprendidos en los paquetes de librerías importadas o integradas previamente al proyecto de videojuego.
    .cajon.color-primario.fondo-cajon.p-4.mb-4(data-aos="fade-down-right")
      h4 Los archivos de salida
      p.m-0 Son esencialmente los archivos finales que, en definitiva, formarán parte del videojuego, y que, en el entorno de desarrollo de Unity, están almacenados al interior de la carpeta de proyecto, organizados en subcarpetas según su categoría o función.
    p.mb-4(data-aos="fade-down-right") Para este apartado, trataremos los archivos de salida, de los elementos característicamente más influyentes en el rendimiento.
    //-titulo
    .row.align-items-center(data-aos="fade-down-right")
      .col-sm-1.col-2.p-0.p-lg-3.p-xl-4.pad1
        img.p-2(src='@/assets/curso/tema1/mando.svg')
      .col-auto.col-10.ps-0
        h3.mb-0.correr-izq Optimización del rendimiento gráfico
    p.mb-4(data-aos="fade-down-right") La optimización del rendimiento gráfico comprende el reto más importante del trabajo de optimización, siendo el aspecto gráfico el que puede tener el mayor nivel de exigencia en procesamiento, consumo de memoria y cálculo matemático. Los elementos gráficos tienen gran impacto de rendimiento en dos sistemas fundamentales: el GPU y el CPU. El primer principio de optimización de gráficos es la detección del problema de rendimiento en estas dos dimensiones, teniendo en cuenta que el proceso de optimización puede ser diferente.
    .tarjeta--container.row.mb-5
      .col-md.tarjeta.color-acento-contenido.p-5(data-aos="fade-down-right")
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema1/fig5.svg')
        h2.text-center.text-white El sistema de GPU  
        p.text-center.text-white Está limitado por el #[i fillrate] o tasa de relleno que determina, en esencia, la cantidad de píxeles que la tarjeta gráfica es capaz de dibujar o renderizar, procesar y almacenar, por cada unidad de tiempo.
      .col-md.tarjeta.color-primario.p-5(data-aos="fade-down-left")
        .row.justify-content-center.mb-4
          .col-6
            figure
              img(src='@/assets/curso/tema1/fig6.svg')
        h2.text-center.text-dark El sistema de CPU  
        p.text-center.text-dark Está limitado por el número de <i>batches</i> o lotes de información gráfica que necesita ser renderizada. En términos generales, se remite al cálculo por el procesador de la máquina y el almacenamiento de información en memoria RAM.
    //-titulo
    .row.align-items-center(data-aos="fade-down-right")
      .col-sm-1.col-2.p-0.p-lg-3.p-xl-4.pad1
        img.p-2(src='@/assets/curso/tema1/mando.svg')
      .col-auto.col-10.ps-0
        h3.mb-0.correr-izq Optimización del CPU
    p.mb-5(data-aos="fade-down-right") El problema de rendimiento, en el CPU, se da por el número o cantidad de elementos presentes en la cola de renderizado (<i>render queue</i>). El proceso de optimización consiste en el control de la complejidad de los siguientes elementos gráficos:
    AcordionA(data-aos="fade-down-right").mb-5(tipo="a" clase-tarjeta="tarjeta fondo-8 otrofondo")
      .row.justify-content-around(titulo="Resolución de mapa de bits")
        .col-lg-11.mb-4.mb-md-0
          p El tamaño en resolución de las imágenes pueden optimizarse de acuerdo con las necesidades gráficas. Se debe controlar el tamaño de resolución hasta un nivel que compense la calidad de apariencia y su peso en procesamiento.
      .row.justify-content-around(titulo="Dibujo de mallas poligonales")
        .col-lg-5.mb-4.mb-md-0
          p La complejidad en objetos de malla poligonal es proporcional al número de triángulos que poseen y que deben ser calculados, procesados y dibujados. Es necesario, entonces, reducir el número de polígonos/triángulos de una malla, y a la vez mantener el menor número posible de mallas poligonales en escena. Por otro lado, es necesario agrupar o unir mallas poligonales con pocos triángulos, dado que en el procesamiento por CPU resulta ser un mayor esfuerzo el cálculo de múltiples mallas con un solo triángulo, que múltiples triángulos presentes en pocas mallas.
        .col-lg-6
          figure
            img(src='@/assets/curso/tema1/img9.png')
      .row.justify-content-around(titulo="Dibujo de materiales y texturas")
        .col-lg-5.mb-4.mb-md-0
          p Es importante reducir el número de materiales, en objetos o elementos similares en apariencia, tratando de generar atlas de imágenes de textura que puedan ser utilizados en un mismo material por diferentes objetos.
        .col-lg-6
          figure
            img(src='@/assets/curso/tema1/img10.png')
      .row.justify-content-around(titulo="Efectos de sombreado, reflexión y luces")
        .col-lg-5.mb-4.mb-md-0
          p El cálculo de sombras, luces y efectos de reflexión, supone el cálculo matemático de cada uno de estos, en tiempo real, cada vez por segundo. En este tipo de optimización se utiliza el quemado de texturas (<i>baking texture</i>), que permite generar imágenes con el dibujado de píxeles de sombras, luces, y reflexiones en la imagen de textura, evitando el cálculo en tiempo real de estos efectos.
        .col-lg-6
          figure
            img(src='@/assets/curso/tema1/img11.png')
    //-titulo
    .row.align-items-center(data-aos="fade-down-right")
      .col-sm-1.col-2.p-0.p-lg-3.p-xl-4.pad1
        img.p-2(src='@/assets/curso/tema1/mando.svg')
      .col-auto.col-10.ps-0
        h3.mb-0.correr-izq Optimización del GPU
    p.mb-4(data-aos="fade-down-left") En el GPU el problema de rendimiento se da por el ancho de banda que posee el sistema para procesar, analizar y dibujar o renderizar en pantalla (<i>fillrate</i>). El proceso de optimización consiste en el control de la complejidad de los siguientes elementos gráficos:
    AcordionA(data-aos="fade-down-right").mb-5(tipo="a" clase-tarjeta="tarjeta fondo-8 otrofondo")
      .row.justify-content-around(titulo="Rendimiento de iluminación estática")
        .col-lg-5.mb-4.mb-md-0
          p De una forma similar con la técnica de quemado de texturas, puede optimizarse desde el editor de <i>Unity 3D</i> los efectos de iluminación. En este proceso se busca generar iluminación sin la necesidad de cálculos matemáticos, a partir del uso de la herramienta de <i>lightmapping</i> que permite hacer el quemado de texturas, al interior del motor, calculando sus propiedades una sola vez en elementos estáticos, haciendo más rápido el procesamiento general y alivianando la cantidad de información en el procesador y memoria.
          a.boton.color-acento-botones.indicador__container.mb-4(@click="modal3 = true")
            span Ampliar imagen
            i.fas.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
        .col-lg-6.col-md-11.col-sm-12.col-12.mb-5
          .row.justify-content-center
            .col-auto.fondo-7.px-4.py-2
              .titulo-sexto.color-acento-contenido.mb-0
                p.mb-0 #[b #[i Figura 4]]
                p.mb-0 Rendimiento de iluminación estática
          figure
            img(src='@/assets/curso/tema1/img12.png')
      .row.justify-content-around(titulo="Compresión de texturas y <em>mipmaps</em>")
        .col-lg-5.mb-4.mb-md-0
          p En términos generales la carga del procesamiento de imágenes lo determina las resoluciones de estas. El proceso de optimización puede involucrar dos técnicas principales: en primer lugar, la configuración de la propiedad de Compresión, desde el editor Unity 3D y, en segundo lugar, la activación de Generación de <i>mipmaps</i> para realizar un decrecimiento de la resolución de aquellas imágenes que se renderizarán en triángulos pequeños.
          a.boton.color-acento-botones.indicador__container.mb-4(@click="modal4 = true")
            span Ampliar imagen
            i.fas.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
        .col-lg-6.col-md-11.col-sm-12.col-12.mb-5
          .row.justify-content-center
            .col-auto.fondo-7.px-4.py-2
              .titulo-sexto.color-acento-contenido.mb-0
                p.mb-0 #[b #[i Figura 5]]
                p.mb-0 Proceso de optimización de texturas en el panel Inspector
          figure
            img(src='@/assets/curso/tema1/img13.png')
      .row.justify-content-around(titulo="Complejidad de la geometría de un modelo 3D")
        .col-lg-5.mb-4.mb-md-0
          p La complejidad de un modelo tridimensional radica en la cantidad de triángulos que posea. En este sentido es necesario mantener un número reducido de triángulos, procurando no afectar su apariencia. Por otro lado, los vértices presentes en un modelo difieren en cantidad a los renderizados por el GPU. La razón es que los vértices, reales o geométricos, tienden a duplicarse según se encuentren en las costuras del modelo o posean múltiples normales o coordenadas UV.
          a.boton.color-acento-botones.indicador__container.mb-4(@click="modal5 = true")
            span Ampliar imagen
            i.fas.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
        .col-lg-6.col-md-11.col-sm-12.col-12.mb-5
          .row.justify-content-center
            .col-auto.fondo-7.px-4.py-2
              .titulo-sexto.color-acento-contenido.mb-0
                p.mb-0 #[b #[i Figura 6]]
                p.mb-0 Proceso optimización densidad de malla poligonal
          figure
            img(src='@/assets/curso/tema1/img14.png')
    ModalA(:abrir-modal.sync="modal3")
      .row.align-items-center
        .col-md-10.col-12.mb-4.mb-md-0
          figure
            img(src='@/assets/curso/tema1/img12.png')
    ModalA(:abrir-modal.sync="modal4")
      .row.align-items-center
        .col-md-10.col-12.mb-4.mb-md-0
          figure
            img(src='@/assets/curso/tema1/img13.png')
    ModalA(:abrir-modal.sync="modal5")
      .row.align-items-center
        .col-md-10.col-12.mb-4.mb-md-0
          figure
            img(src='@/assets/curso/tema1/img14.png')
    p.mb-4 Mediante el siguiente video, se verán algunos elementos clave para el proceso de optimización de assets.
    figure(data-aos="fade-down")
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    Separador
    #t_1_3.titulo-segundo.color-acento-contenido(data-aos="fade-down-right")
      h2 1.3 Optimización de archivos de código
    p(data-aos="fade-down-right") La optimización de código se lleva a cabo en el mismo proceso de escritura del código fuente, buscando obtener el mayor rendimiento en el procesamiento de instrucciones, además del peso de los archivos. Por otro lado, es necesario analizar la necesidad o no de crear varios #[i scripts] para cada acción o implementarlas en un solo #[i script]. 
    p.mb-4(data-aos="fade-down-right") De cualquier forma, desde el diseño algorítmico se comienza a definir el esquema lógico y las relaciones entre diferentes funciones, clases, eventos y variables.
    .bloque-texto-a.color-primario.p-4.p-md-5.mb-5(data-aos="fade-down-right") 
      .row.m-0.align-items-center.justify-content-between
        .col-lg-4.mb-4.mb-lg-0
          h2.mb-0 Optimización de <i>scripts</i> en juegos de Unity.
        .col-lg-8
          .bloque-texto-a__texto.p-4
            p Cuando el juego se ejecuta, la unidad central de procesamiento (CPU) del dispositivo ejecuta las instrucciones. Cada fotograma del juego requiere que se ejecuten millones de estas instrucciones de CPU y para mantener una velocidad de fotogramas uniforme, la CPU debe llevar a cabo sus instrucciones dentro de un período de tiempo establecido. Cuando la CPU no puede llevar a cabo todas sus instrucciones a tiempo, el  juego puede ralentizarse, entrecortarse o congelarse.
    p.mb-4(data-aos="fade-down-right") Muchas cosas pueden hacer que la CPU tenga demasiado trabajo por hacer. Los ejemplos podrían incluir código de renderizado exigente, simulaciones físicas muy complejas o demasiadas devoluciones de llamada de animación. Este apartado se centra solo en una de estas razones: problemas de rendimiento de la CPU causados por el código que se escribe en los <i>scripts</i>.
    .cajon.color-primario.fondo-cajon.p-4.mb-4(data-aos="fade-down-right")
      p.m-0 Se aprenderá cómo los #[i scripts] se convierten en instrucciones de la CPU, qué puede hacer estos generen una cantidad excesiva de trabajo para la CPU y cómo solucionar los problemas de rendimiento causados por el código en los #[i scripts].
    //-titulo
    .row.align-items-center(data-aos="fade-down-right")
      .col-sm-1.col-2.p-0.p-lg-3.p-xl-4.pad1
        img.p-2(src='@/assets/curso/tema1/mando.svg')
      .col-auto.col-10.ps-0
        h3.mb-0.correr-izq Diagnóstico de problemas de código
    .row.justify-content-center
      .col-lg-7.col-md-12.mb-4.mb-lg-0(data-aos="fade-down-right")
        p Los problemas de rendimiento causados por demandas excesivas en la CPU pueden manifestarse como velocidades de cuadro bajas, rendimiento desigual o congelamientos intermitentes. Sin embargo, otros problemas pueden causar síntomas similares. Si el juego tiene problemas de rendimiento como este, lo primero que debemos hacer es usar la ventana Profiler de Unity para establecer si los problemas de rendimiento se deben a que la CPU no puede completar sus tareas a tiempo. Una vez establecido esto, debemos determinar si los <i>scripts</i> de usuario son la causa del problema, o si el problema es causado por alguna otra parte del juego, física compleja o animaciones, por ejemplo.
      .col-lg-5.col-md-6.col-sm-7.col-8(data-aos="fade-down-left")
        img.p-2(src='@/assets/curso/tema1/fig7.svg')
    //-titulo
    .row.align-items-center(data-aos="fade-down-right")
      .col-sm-1.col-2.p-0.p-lg-3.p-xl-4.pad1
        img.p-2(src='@/assets/curso/tema1/mando.svg')
      .col-auto.col-10.ps-0
        h3.mb-0.correr-izq Modo de compilación en Unity 3D
    p.mb-5(data-aos="fade-down-right") Para comprender por qué el código puede no estar funcionando bien, primero se debe entender qué sucede cuando Unity compila el juego. Saber lo que sucede detrás de escena ayudará a tomar decisiones informadas sobre cómo se puede mejorar el rendimiento del juego, a saber:
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span a
        | #[b  El proceso de compilación]
    .row.justify-content-center.mb-5
      .col-lg-6.col-md-12.mb-4.mb-lg-0(data-aos="fade-down-right")
        p Cuando se construye el juego, Unity empaqueta todo lo necesario para ejecutarlo en un programa que puede ser ejecutado por el dispositivo objetivo. Las CPU solo pueden ejecutar código escrito en lenguajes muy simples conocidos como código máquina o código nativo; no pueden ejecutar código escrito en lenguajes más complejos como C#. Esto significa que Unity debe traducir el código a otros idiomas, a este proceso se le llama compilación.
        .cajon.color-primario.fondo-cajon.p-4.mb-4
          p.m-0 #[b Unity] primero compila los #[i scripts] en un lenguaje llamado Common Intermediate Language (CIL) que es fácil de compilar en una amplia gama de diferentes lenguajes de código nativo. Luego, el CIL se compila en código nativo para el dispositivo de destino específico. Este segundo paso ocurre cuando se construye el juego (conocido como compilación anticipada o compilación AOT), o en el dispositivo de destino, justo antes de que se ejecute el código (conocido como compilación justo a tiempo o compilación JIT). Si el juego usa compilación AOT o JIT generalmente depende del <i>hardware</i> de destino.
      .col-lg-6.col-md-7.col-8(data-aos="fade-down-left")
        img(src='@/assets/curso/tema1/img15.jpg')
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span b
        | #[b  Relación entre el código fuente y el código compilado]
    .row.justify-content-center.mb-5
      .col-lg-6.col-md-12.mb-4.mb-lg-0(data-aos="fade-down-right")
        p El código que aún no ha sido compilado se conoce como código fuente, este determina la estructura y el contenido del código compilado.
        p En su mayor parte, un código fuente bien estructurado y eficiente dará como resultado un código compilado bien estructurado y eficiente. Sin embargo, es útil saber un poco sobre el código nativo para entender mejor por qué algunos códigos fuente se compilan en un código nativo más eficiente.
        p En primer lugar, algunas instrucciones de la CPU tardan más en ejecutarse que otras. Un ejemplo de esto es calcular una raíz cuadrada. Este cálculo requiere más tiempo para que la CPU se ejecute que, por ejemplo, multiplicar dos números. La diferencia entre una sola instrucción de CPU rápida y una sola instrucción de CPU lenta es realmente muy pequeña, pero es útil para nosotros entender que, fundamentalmente, algunas instrucciones son simplemente más rápidas que otras.
      .col-lg-6.col-md-7.col-8(data-aos="fade-down-left")
        img(src='@/assets/curso/tema1/img15.jpg')
    .row.justify-content-center.mb-5
      .col-lg-6.col-md-7.col-8.mb-4.mb-lg-0.order-lg-first.order-last(data-aos="fade-down-right")
        img(src='@/assets/curso/tema1/fig8.svg')
      .col-lg-6.col-md-12.order-lg-last.order-first(data-aos="fade-down-left")
        p Lo siguiente que se debe entender es que algunas operaciones que parecen muy simples en el código fuente pueden ser sorprendentemente complejas cuando se compilan en código. Un ejemplo de esto es insertar un elemento en una lista, pues se necesitan muchas más instrucciones para realizar esta operación que, por ejemplo, acceder a un elemento de una matriz por índice. Nuevamente, cuando se considera un ejemplo individual, se habla de una pequeña cantidad de tiempo, pero es importante entender que algunas operaciones dan como resultado más instrucciones que otras.
        .cajon.color-primario.fondo-cajon.p-4.mb-4
          p.m-0 Comprender estas ideas ayudará a entender por qué algunos códigos funcionan mejor que otros, incluso cuando ambos ejemplos hacen cosas bastante similares. Un conocimiento previo limitado de cómo funcionan las cosas en un nivel bajo puede ayudar a escribir juegos que funcionen bien.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span c
        | #[b Comunicación en tiempo de ejecución entre el código de Unity Engine y el código de secuencia de comandos]
    p.mb-4(data-aos="fade-down-right")  Es útil comprender que las secuencias de comandos escritas en C# se ejecutan de una manera ligeramente diferente al código que forma gran parte de Unity Engine. La mayor parte de la funcionalidad principal de Unity Engine está escrita en C++ y ya se ha compilado en código nativo. Este código de motor compilado es parte de la instalación de Unity.
    .row.justify-content-center.mb-5
      .col-lg-5.col-md-6.col-sm-8.col-10
        img(src='@/assets/curso/tema1/fig9.svg')
    p(data-aos="fade-down-right")  El código compilado en CIL, como el código fuente, se conoce como código administrado. Cuando el código administrado se compila en código nativo, se integra con algo llamado tiempo de ejecución administrado. El tiempo de ejecución administrado se encarga de cosas como la administración automática de la memoria y las verificaciones de seguridad para garantizar que un error en el código resulte en una excepción en lugar de que el dispositivo se bloquee.
    p.mb-4(data-aos="fade-down-right")  Cuando la CPU cambia entre el código del motor en ejecución y el código administrado, se debe trabajar para configurar estas comprobaciones de seguridad. Cuando se devuelven datos del código administrado al código del motor, es posible que la CPU deba realizar un trabajo para convertir los datos del formato utilizado por el tiempo de ejecución administrado al formato que necesita el código del motor.
    .cajon.color-primario.fondo-cajon.p-4.mb-5
      p.m-0 Esta conversión se conoce como clasificación y aquí una vez más, la sobrecarga de una sola llamada entre el código administrado y el del motor no es particularmente costosa, pero es importante entender que este costo existe.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span d
        | #[b Causas del código de bajo rendimiento]
    p.mb-4(data-aos="fade-down-right")  Ahora que se comprende lo que le sucede a el código cuando Unity compila y ejecuta el juego, se puede entender que cuando el código funciona mal es porque crea demasiado trabajo para la CPU en tiempo de ejecución. A continuación, se consideran las diferentes razones de esto:
    .row.justify-content-center.mb-5
      .col-lg-7.col-md-12.mb-4.mb-lg-0(data-aos="fade-down-right")
        LineaTiempoD.color-secundario
          p(numero="1" titulo="La primera posibilidad") Que el código sea un desperdicio o esté mal estructurado. Un ejemplo de esto podría ser el código que realiza la misma llamada de función repetidamente cuando solo podría realizar la llamada una vez con lo que se cubrirán varios ejemplos comunes de estructura deficiente y mostrará soluciones de ejemplo.
          
          p(numero="2" titulo="La segunda posibilidad") Que el código parece estar bien estructurado, pero hace llamadas innecesariamente costosas en rendimiento a otro código. Un ejemplo de esto podría ser el código que da como resultado llamadas no necesarias entre el código administrado y el del motor. 
          
          p(numero="3" titulo="La tercera posibilidad") Que el código sea eficiente, pero que se llame cuando no es necesario. Un ejemplo de esto podría ser el código que simula la línea de visión de un enemigo. El código en sí puede funcionar bien, pero es un desperdicio ejecutar este código cuando el jugador está muy lejos del enemigo. 
          
          p(numero="4" titulo="La cuarta posibilidad") Que el código sea simplemente demasiado exigente. Un ejemplo de esto podría ser una simulación muy detallada en la que una gran cantidad de agentes utilizan IA compleja. Si se han agotado otras posibilidades y optimizado este código tanto como se puede, es posible que simplemente se necesite rediseñar el juego para hacerlo menos exigente: por ejemplo, falsificar elementos de la simulación en lugar de calcularlos.
      .col-lg-5.col-md-6.col-sm-7.col-8(data-aos="fade-down-left")
        img(src='@/assets/curso/tema1/img16.jpg')
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span e
        | #[b Mejorar el rendimiento del código]
    p.mb-4(data-aos="fade-down-right")  Una vez que se ha establecido que los problemas de rendimiento en el juego se deben al código, se debe pensar detenidamente cómo resolver estos problemas. La optimización de una función exigente puede parecer un buen punto de partida, pero es posible que la función en cuestión ya sea óptima como puede ser y simplemente sea cara por naturaleza. En lugar de cambiar esa función, puede haber un pequeño ahorro de eficiencia que podemos hacer en un <i>script</i> que usan cientos de GameObjects y que da un aumento de rendimiento mucho más útil. Además, mejorar el rendimiento de la CPU del código puede tener un costo: los cambios pueden aumentar el uso de la memoria o descargar el trabajo a la GPU.
    .cajon.color-primario.fondo-cajon.p-4.mb-5(data-aos="fade-down-right") 
      p.m-0 Por estos motivos, se define una serie de sugerencias para mejorar el rendimiento del código, con ejemplos de situaciones en las que se pueden aplicar. Al igual que con toda la optimización del rendimiento, no existen reglas estrictas y rápidas. Lo más importante que se debe hacer es perfilar el juego, comprender la naturaleza del problema, experimentar con diferentes soluciones y medir los resultados de los cambios.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span f
        | #[b Escribir código eficiente]
    p.mb-5(data-aos="fade-down-right") Escribir y estructurar sabiamente el código eficiente puede conducir a mejoras en el rendimiento del juego. Si bien los ejemplos que se muestran están en el contexto de un juego de Unity, estas sugerencias de mejores prácticas generales no son específicas de los proyectos de Unity o las llamadas a la API de Unity.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span g
        | #[b Código fuera de bucles]
    p.mb-4(data-aos="fade-down-right")  Los bucles son un lugar común para que se produzcan ineficiencias, especialmente cuando están anidados. Las ineficiencias pueden sumarse si están en un bucle que se ejecuta con mucha frecuencia, especialmente si este código se encuentra en muchos GameObjects del juego. En el siguiente ejemplo simple, el código itera a través del ciclo cada vez que se llama a Update(), independientemente de si se cumple o no la condición.
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig10.svg')
    p.mb-4(data-aos="fade-down-right") Con un simple cambio, el código itera a través del ciclo solo si se cumple la condición.
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig11.svg')
    p.mb-5(data-aos="fade-down-right") Este es un ejemplo simplificado, pero ilustra un ahorro real que se puede hacer. Se debería examinar el código en busca de lugares en los que se han estructurado mal nuestros bucles.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span h
        | #[b Considerar si el código debe ejecutar cada cuadro]
    p.mb-5(data-aos="fade-down-right") Update() es una función que Unity ejecuta una vez por cuadro. Update() es un lugar conveniente para colocar el código que debe llamarse con frecuencia o el código que debe responder a cambios frecuentes. Sin embargo, no es necesario que todo este código ejecute todos los fotogramas. Sacar el código de Update() para que se ejecute solo cuando sea necesario puede ser una buena forma de mejorar el rendimiento.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span i
        | #[b Ejecute código solo cuando las cosas cambien]
    p.mb-4(data-aos="fade-down-right")  Ahora se verá un ejemplo muy simple de optimización del código para que solo se ejecute cuando las cosas cambien. En el siguiente código, DisplayScore() se llama en Update(). Sin embargo, es posible que el valor de la puntuación no cambie con cada fotograma. Esto significa que estamos llamando innecesariamente a DisplayScore().
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig12.svg')
    p.mb-4(data-aos="fade-down-right")  Con un simple cambio, ahora se asegura que <i>DisplayScore</i> () se llame solo cuando el valor de la puntuación haya cambiado.
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig13.svg')
    p.mb-5(data-aos="fade-down-right")  De nuevo, el ejemplo anterior está deliberadamente simplificado, pero el principio es claro: si se aplica este enfoque en todo el código, es posible ahorrar recursos de CPU.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span j
        | #[b Ejecutar código cada &lbrack;x&rbrack; fotogramas]
    p(data-aos="fade-down-right")  Si el código necesita ejecutarse con frecuencia y no puede ser activado por un evento, eso no significa que deba ejecutar cada fotograma. En estos casos, podemos optar por ejecutar código cada [x] fotogramas.
    p.mb-4(data-aos="fade-down-right")  En este código de ejemplo, una función costosa se ejecuta una vez por cuadro.
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig14.svg')
    p(data-aos="fade-down-right")  De hecho, sería suficiente para las necesidades ejecutar este código una vez cada 3 fotogramas. En el siguiente código, se usa el operador de módulo para asegurarse que la función costosa se ejecute solo en cada tercer fotograma.
    p.mb-4(data-aos="fade-down-right")  intervalo int privado = 3;
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig15.svg')
    p(data-aos="fade-down-right") Un beneficio adicional de esta técnica es que es muy fácil distribuir un código costoso en marcos separados, evitando picos. En el siguiente ejemplo, cada una de las funciones se llama una vez cada 3 fotogramas y nunca en el mismo fotograma.
    p.mb-4(data-aos="fade-down-right") intervalo int privado = 3;
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig16.svg')  
    p.mb-4(data-aos="fade-down-right") De hecho, sería suficiente para las necesidades ejecutar este código una vez cada 3 fotogramas. En el siguiente código, se usa el operador de módulo para asegurarse que la función costosa se ejecute solo en cada tercer fotograma.
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig17.svg')
    p.mb-4(data-aos="fade-down-right") Un beneficio adicional de esta técnica es que es muy fácil distribuir el código costoso en marcos separados, evitando picos. En el siguiente ejemplo, cada una de las funciones se llama una vez cada 3 fotogramas y nunca en el mismo fotograma.
    .row.justify-content-center.mb-5
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig18.svg')
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span k
        | #[b Utilizar el almacenamiento en caché]
    .row.justify-content-center
      .col-lg-6.col-md-12.mb-4.mb-lg-0(data-aos="fade-down-right")
        p Si el código llama repetidamente a funciones costosas que devuelven un resultado y luego descarta esos resultados, esta puede ser una oportunidad para la optimización. El almacenamiento y la reutilización de referencias a estos resultados pueden resultar más eficaz. Esta técnica se conoce como almacenamiento en caché.
        p En Unity es común llamar a GetComponent() para acceder a los componentes. En el siguiente ejemplo, se llama a GetComponent() en Update() para acceder a un componente de Renderer antes de pasarlo a otra función. Este código funciona, pero es ineficaz debido a la llamada repetida a GetComponent().
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left")
        img(src='@/assets/curso/tema1/fig19.svg')
    p.mb-4(data-aos="fade-down-left") El siguiente código llama a GetComponent() solo una vez, ya que el resultado de la función se almacena en caché. El resultado almacenado en caché se puede reutilizar en Update() sin más llamadas a GetComponent().
    .row.justify-content-center.mb-4
      .col-lg-6.col-md-8.col-sm-10.col-12(data-aos="fade-down-left") 
        img(src='@/assets/curso/tema1/fig20.svg')
    p.mb-5(data-aos="fade-down-left") Se debería examinar el código en busca de casos en los que se hacen llamadas frecuentes a funciones que devuelven un resultado. Es posible, entonces, reducir el costo de estas llamadas utilizando el almacenamiento en caché.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span l
        | #[b Usar agrupación de objetos]
    p.m-4(data-aos="fade-down-right") Generalmente es más costoso crear instancias y destruir un objeto que desactivarlo y reactivarlo. Esto es especialmente cierto si el objeto contiene código de inicio, como llamadas a GetComponent() en una función Awake() o Start(). Si se necesita generar y deshacerse de muchas copias del mismo objeto, como balas en un juego de disparos, entonces se puede obtener beneficios de la agrupación de objetos.
    .cajon.color-primario.fondo-cajon.p-4.mb-5(data-aos="fade-down-right")
      p La agrupación de objetos es una técnica en la que, en lugar de crear y destruir instancias de un objeto, los objetos se desactivan temporalmente y luego se reciclan y reactivan según sea necesario. Aunque es una técnica muy conocida para administrar el uso de la memoria, la agrupación de objetos también puede ser útil como técnica para reducir el uso excesivo de la CPU.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span m
        | #[b Ejecutar código solo cuando es necesario ejecutarlo]
    p.mb(data-aos="fade-down-right")  Hay un dicho en programación: “el código más rápido es el código que no se ejecuta”. A menudo, la forma más eficaz de resolver un problema de rendimiento es no utilizar una técnica avanzada, es simplemente eliminar el código que no necesita estar allí en primer lugar.
    .row.justify-content-center.mb-5
      .col-lg-10.col-md-12
        .row.align-items-center(data-aos="fade-down-right")
          .col-sm-1.col-2.p-0.p-lg-3.p-xl-4.pad1
            img.p-2(src='@/assets/curso/tema1/fig21.svg')
          .col-auto.col-10.ps-0
            p.mb-0.correr-izq Eliminación (<i>Culling</i>)
        p.mb-4(data-aos="fade-down-right") Unity contiene un código que comprueba si los objetos están dentro del cono de vista de una cámara. Si no están dentro del cono de vista de una cámara, el código relacionado con la representación de estos objetos no se ejecuta; el término para esto es sacrificio "frustum".
        .cajon.color-primario.fondo-cajon.p-4.mb-4(data-aos="fade-down-right")
          p Se puede adoptar un enfoque similar al código en los <i>scripts</i>. Si se tiene un código que se relaciona con el estado visual de un objeto, es posible que no se necesite ejecutar este código cuando el jugador no pueda ver el objeto. En una escena compleja con muchos objetos, esto puede resultar en ahorros de rendimiento considerables.
        p.mb-4(data-aos="fade-down-right") En el siguiente código de ejemplo simplificado, se tiene un ejemplo de un enemigo patrullando. Cada vez que se llama a Update(), el script que controla a este enemigo llama a dos funciones de ejemplo: una relacionada con el movimiento del enemigo y otra relacionada con su estado visual.
        .row.justify-content-center
          .col-lg-8
            img.mb-4(src='@/assets/curso/tema1/fig22.svg')
        p.mb-4(data-aos="fade-down-right") En el siguiente código, ahora se verificará si el renderizador del enemigo está dentro del <i>frustum</i> de cualquier cámara. El código relacionado con el estado visual del enemigo se ejecuta solo si el enemigo es visible.
        .row.justify-content-center
          .col-lg-8
            img.mb-4(src='@/assets/curso/tema1/fig23.svg')
        .row.align-items-center(data-aos="fade-down-right")
          .col-sm-1.col-2.p-0.p-lg-3.p-xl-4.pad1
            img.p-2(src='@/assets/curso/tema1/fig21.svg')
          .col-auto.col-10.ps-0
            p.mb-0.correr-izq Deshabilitar el código de objetos no visibles
        p.mb-4(data-aos="fade-down-right") si se sabe que determinados objetos de la escena no son visibles en un punto concreto del juego, se pueden desactivar manualmente. Cuando se tenga menos certeza y se necesite calcular la visibilidad, se podría usar un cálculo aproximado (por ejemplo, verificar si el objeto detrás del reproductor), funciones como OnBecameInvisible() y OnBecameVisible(), o un <i>raycast</i> más detallado. La mejor implementación depende en gran medida del juego, y la experimentación y la creación de perfiles son esenciales.
    ol.lista-ol--cuadro.mb-4
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span n
        | #[b Nivel de detalle]
    .row.justify-content-center(data-aos="fade-down-right")
      .col-lg-10.col-md-12.mb-4
        .bloque-texto-g.color-acento-contenido.p-3.p-sm-4.p-md-5
          .bloque-texto-g__img(
            :style="{'background-image': `url(${require('@/assets/curso/tema1/img17.jpg')})`}"
          )
          .bloque-texto-g__texto.px-4.py-5
            p También conocido como LOD, es otra técnica común de optimización de renderizado. Los objetos más cercanos al jugador se renderizan con total fidelidad utilizando mallas y texturas detalladas; los objetos distantes las utilizan menos detalladas. 
            br
            br
            p Se puede usar un enfoque similar con el código. Por ejemplo, al tener un enemigo con un #[i script] de IA que determina su comportamiento. Parte de este comportamiento puede involucrar operaciones costosas para determinar qué puede ver y escuchar, y cómo debería reaccionar a esta entrada. Se podría usar un sistema de nivel de detalle para habilitar y deshabilitar estas costosas operaciones en función de la distancia del enemigo al jugador.
    .cajon.color-primario.fondo-cajon.p-4.mb-4(data-aos="fade-down-right")
      p En una escena con muchos de estos enemigos, se haría un ahorro de rendimiento considerable si solo los enemigos más cercanos realizan las operaciones más costosas.
    p(data-aos="fade") La API CullingGroup de Unity permite conectarse al sistema LOD de Unity para optimizar el código. La página del manual de la API de CullingGroup contiene varios ejemplos de cómo se puede utilizar en el juego. Como siempre, se debe probar, perfilar y encontrar la solución adecuada para el juego.
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
  data: () => ({
    // variables de vue
    modal1: false,
    modal2: false,
    modal3: false,
    modal4: false,
    modal5: false,
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
