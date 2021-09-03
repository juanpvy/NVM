# NVM
Cuando se trabaja con un proyecto SPFX es necesario instalar una serie de software extra, entre ellos node.js.

Si visitamos la pagina de Microsoft , "Como configurar el entorno de desarrollo" , nos mostrara la versión de node.js que se debe de instalar en ese momento ya que no todas las versiones de SPFX son compatibles con todas las  versiones de SPFX.

# SPFX y Node.js

Si llevamos un tiempo desarrollando con SPFX nos podríamos topar con el escenario de trabajar en varias proyectos donde necesitaríamos actualizar el SPFX y node.js  y al mismo tiempo hacer una modificación a un proyecto anterior que depende de otra versión de SPFX y node.js.

Es aquí donde nos surge la pregunta, ¿Cómo le puedo hacer parea desarrollar mis dos proyectos con diferente versión node.js? NVM

# Node Version Manager(NVM)
Es una herramienta que nos ayuda a instalar las versiones de node.js con las que queremos trabajar y  cambiar entre ellas, de esta manera cuando se necesite  desarrollar para una versión especifica de SPFX y node.js solo  puedo utilizar NVM para configurar/cambiar a la version que necesito y listo.

# Como utilizar NVM
Lo primero es desinstalar las versiones que tenga de node.js

![b58ac332-d721-4a27-b919-ede8ccd91a65](https://user-images.githubusercontent.com/50918464/132070823-0e396843-639a-4e02-af84-e9cb87fb7608.png)

Después hay que instalar NVM desde la siguiente ruta https://github.com/coreybutler/nvm-windows/releases con el archivo nvm-setup.zip.

Ya instalado podemos utilizar los siguientes comandos

```C:> nvm ls                  // Nos lista todos las versiones de node.js instaladas ```

```C:> nvm ls available        // Nos lista todos las versiones de node.js que se pueden instalar```

![3708d589-9850-46ed-9bd6-dc9aa9819bfe (1)](https://user-images.githubusercontent.com/50918464/132071101-b3ff3d7f-9b10-4d98-864b-4d9d5ed4d17b.png)

Para instalar las versiones de node.js que necesitamos, ejecutamos el comando.
```C:> nvm install [no.version]```

Aquí se instalaron dos versiones de node.js  10.18.1 y 14.17.1
![6f4e172a-40f0-4530-931c-e71d09bb5cc4](https://user-images.githubusercontent.com/50918464/132071291-a368c23a-5d21-4849-aeaa-f3491809fc57.png)

Recuerdan el comando 
```C:> nvm ls```

![791f179a-9656-4f36-b38e-e9062803672b](https://user-images.githubusercontent.com/50918464/132071351-d28277b5-d4a4-4343-a4c2-09d59c3208a0.png)

Para poder seleccionar o cambiar de versión de node.js  ejecutamos el comando.
```C:> nvm use [version]```

Ya para validar que versión tengo seleccionada actualmente ejecutamos el comando.
```C:> node -v```

![5a037b1e-51a4-48cf-9451-eb0d03ada2ae](https://user-images.githubusercontent.com/50918464/132071513-75a908c9-194d-428e-8480-6bbaf27f2c86.png)

Con la versión de node.js seleccionada podemos instalar las paquetes necesarios para trabajar.
![d6ce356d-e53d-44fc-ba17-2788228a9c65](https://user-images.githubusercontent.com/50918464/132071549-3ba3a106-5721-4629-bc9d-4b89f6b68c92.png)

