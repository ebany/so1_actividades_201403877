# Tipos de kernel y sus diferencias

- kernel monolítico: Un kernel grande para todas las tareas. Es el único responsable de la gestión de la memoria y de los procesos, de la comunicación entre procesos y proporciona funciones de soporte de drivers y hardware. Los sistemas operativos que usan el kernel monolítico son Linux, OS X y Window.

- Microkernel: El microkernel se ha diseñado intencionadamente de un tamaño pequeño para que en caso de fallo no paralice todo el sistema operativo. No obstante, para que pueda asumir las mismas funciones que un kernel grande, está dividido en varios módulos. Como ejemplo de aplicación solo existe el componente Mach de OS X, ya que hasta ahora no hay ningún sistema operativo con microkernel.

- kernel híbrido: La combinación del kernel monolítico y el microkernel se denomina kernel híbrido. En este caso, el kernel grande se hace más compacto y modulable. Otras partes del kernel pueden cargarse dinámicamente. Esto ya ocurre en cierta medida en Linux y OS X.

#User vs Kernel Mode

- User Mode: cuando se inicia un programa en un sistema operativo, Windows por ejemplo, se inicia el programa en modo de usuario. Y cuando un programa en modo usuario solicita ejecutarse, Windows crea un proceso y un espacio de direcciones virtuales (espacio de direcciones para ese proceso). Los programas de modo de usuario tienen menos privilegios que las aplicaciones de modo de usuario y no se les permite acceder a los recursos del sistema directamente.

- Kernel Mode: El kernel es el programa central en el que se basan todos los demás componentes del sistema operativo, se utiliza para acceder a los componentes de hardware y programar qué procesos deben ejecutarse en un sistema informático y cuándo, y también administra la interacción entre el software y el hardware de la aplicación. . Por lo tanto, es el programa más privilegiado, a diferencia de otros programas, puede interactuar directamente con el hardware.

Diferencias:

- En modo kernel, el programa tiene acceso directo y sin restricciones a los recursos del sistema.

- En modo usuario, el programa de aplicación se ejecuta y se inicia.