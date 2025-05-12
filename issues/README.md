# 1. Subimos el codigo Java con los errores (Falta un ";" y el comentario)

![](/issues/fotos/1.png)

# 2. En GitHub creamos lo issues
Esto se hace en la pestaña de issues junto a ***code*** y le damos a ***new issues***

![](/issues/fotos/2.png)

Despues introducimos los datos del como el titulo y una descripcion si qeremos

Selecionamos el label de ***bug*** ya que es un error lo qe causa la falta de un ";"

Al finalizal le damos a create, ya ya podemos verlo

![](/issues/fotos/3.png)
![](/issues/fotos/4.png)

Realizamos lo misma para otro con el label de ***Documentation*** que es por falta de ducumentacion y no causa errores

![](/issues/fotos/5.png)

# 3. Solucionar el issues
En git clonamos el repositorio y editamos con el que mas comodos estemos (nano en mi caso) el archivo con el issues

![](/issues/fotos/6.png)

Le agregamos el ";" que es lo qeu issues nos decia que le ocurria y guardamos los cambios

![](/issues/fotos/7.png)

Añadimos los cambios con ```git add . ```

![](/issues/fotos/10.png)

# 4. Cerrar el issues
En vez de hacer un commit normal se la añade ***Closes #[numero del issues]*** y con esto lo cerrarias en el repositorio
Que dando el siguiente comando ```git commit -m "Closes #4: ; Añadido"```
Despues de eso se hace un ```git push origin main``` para subir los cambios a GitHub

![](/issues/fotos/8.png)

# 5. resolver el otro issues
Primero tendremos que hacer un ```git pull origin main``` para descargar los cambios que se hayan realizado en el repositorio

![](/issues/fotos/pull.png)

Despues de esto volvemos a realizar los mismos pasos solo que cuando se realice el commit se pondra el numero que le corresponde a este issues
![](/issues/fotos/6.png)

![](/issues/fotos/9.png)
![](/issues/fotos/10.png)
![](/issues/fotos/11.png)
![](/issues/fotos/12.png)
