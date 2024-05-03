# Plataformas de desarrollo web
Las aplicaciones web se pueden desarrollar con cualquier lenguaje de programación del lado del servidor.
Samarint es una plataforma universal para el desarrollo de aplicaciones híbridas, se escribia en C# y compilaba para IOS y para Android.

# Manejador de paquetes
Necesitamos aprender el proceso para construir aplicaciones.
Un manejador de paquetes nos permite gestionar la empaquetación de la aplicación, y gestionar el arbol de dependencias.

Un árbol de dependencias es la definición de como se utilizan todas las librerías que utiliza la aplicación.

Para Java un gestor de paquetes es Maven.
Para Python tenemos pop.
Para Ruby tenemos RubyGems

Scala es un lenguaje de programación que vive en la máquina virtual de Java. Es un lenguaje funcional y sirve para el análisis de datos, es más potente que python.
Erlak es un lenguaje de programación altamente funcional y altamente concurrente.
Las personas que dejaron Ruby, hicieron un compilador con una sintaxis similar a Ruby, es decir Elixir, y Elixir compila a Erlak.

En desarrollo de software decimos que refresco en caliente es cuando la aplicación muestra los cambios mientras sigue activa. Refresco en frio es cuando debemos apagar la aplicación y volverla a prender para ver los cambios de la aplicación.

# Pruebas
En el mundo de pruebas de software tenemos diferentes tipos de pruebas.
- **Unitarias**: aquellas que se encargan de probar la unidad mínima definida dentro de nuestra aplicación. Si nuestra unidad minima es una función, debemos probar funcion por funcion, si debemos probar clases, probaremos clase por clase.
- **Funcionales (end to end)**: que los componentes interactuen como se espera, si un boton debe realizar una tarea, debemos verificar que el resultado sea este.
- **Integración**: si 2 o más clases o funciones trabajan en conjunto, para verificar que la integración sea la esperada.
- **Rendimiento**: establecer los tiempos que tarda la aplicación en realizar tareas. Comúnmente consisten en revisar el performancede las funcionales. Telemetría.

Por esto es necesario agregar un framework de pruebas al proyecto.
Mocha se utiliza solo o con Shine para hacer pruebas unitarias.