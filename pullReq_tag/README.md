# Parte en parejas

## 1. Realicemos un fork del repositorio
![](/pullReq_tag/fotos/fork.jpg)
![](/pullReq_tag/fotos/1.png)

## 2. Clona el repositorio
```git clone [DIRECCIÓN HTTPS]```

![](/pullReq_tag/fotos/2.png)
![](/pullReq_tag/fotos/3.png)

## 3. Crea una rama
```git checkout -b [Nombre de la Rama]```

![](/pullReq_tag/fotos/4.png)

## 4. Realiza cambios y confírmalos

![](/pullReq_tag/fotos/5.png)

![](/pullReq_tag/fotos/6.png)

**Para ver los cambios usamos el comando:** ```git status```

![](/pullReq_tag/fotos/7.png)

**Para añadir los cambios usamos el comando:** ```git add .``` *El punto significa todos los cambios*

![](/pullReq_tag/fotos/8.png)

**Para cofirmar los cambios usamos el comando:** ```git commit -m "comentario del cambio"```
> [!CAUTION]
> Es obligatorio poner un comentario

![](/pullReq_tag/fotos/9.png)

## 5. Envía los cambios a GitHub
**Para enviar los cambios usamos el comando:** ```git remote```

**Y despues para subirlos cambios usamos el comando ya que sabemos el nombre para este repositorio (origin):** ```git push origin [Nombre de la Rama]```

![](/pullReq_tag/fotos/10.png)

## 6. Crea un pull request
![](/pullReq_tag/fotos/pullReq.jpg)
![](/pullReq_tag/fotos/11.png)
![](/pullReq_tag/fotos/12.png)

# Parte individual
## 1. Hacer un commit antes del tag
Hago un ```git log --oneline``` para ver los commits quese han hecho de manera simplificada

Despues veo lo que hay en el repositorio y edito el Readme.md con ```nano```

Al terminar realixo un ```git status``` para ver que ha detectado el cambio, lo añado todos con ```git add .```

Hago un commit ```git commit -m "descripcion del commit"``` para confirmar los cambios

Y vuelvo a hacer un ```git log --oneline``` paar ver que esta el commit en local

![](/pullReq_tag/fotos_individual/1.png)

## 2. Realizar el tag
Para realizar un tag usamos el sigiente comando: ```git tag -a v1.0 -m "descripcion del tag"```

Y posteriormente lo subimos con un ```git push origin v1.0```

> [!NOTE]
> A mi me diio un error porque lo estaba intentando hacer desde otra cuenta la cualno tenia permisos

![](/pullReq_tag/fotos_individual/2.png)

> [!TIP]
> Para solucionar este problema hay varias formas 2 serian:
> 
>   1.- Si las dos cuentas son tuyas dale permisos de escritura a la cuenta que esta intentando hacer el ***push*** y despues se los quitas si quieres
> 
>   2.- Otra forma de solucionarlo seria hacer un ***frok*** el la cuenta sin permisos y hacer un ***pull request*** despues de haver los cambios
> 
> Yo recomendaria la primera ya que es mas rapida y no necesitas estar haciendo pull request todo el tiempo si es algo que no controlas bien

![](/pullReq_tag/fotos_individual/4.png)
![](/pullReq_tag/fotos_individual/5.png)

Despues de dar los permisos volvemos a realizar el ```git push origin v1.0``` y vemos que se ha realizado

![](/pullReq_tag/fotos_individual/3.png)

## 3. Conectarse a tag
Primero nos salimos del repositorio y volvemos a clonarlo si queremos

Yo lo voy a hacer por tnerlos separados

Al realizar el ```git clone [DIRECCIÓN HTTPS]``` podemos añadir despues de la ***url*** un alias para que no se quede el nombre del repositosio

Yo lo voy hacer para que no haya 2 con el mismo nombre, despues de eso nos conectamos con un ```cd [nombre directorio]```

![](/pullReq_tag/fotos_individual/6.png)

Ahora realizamos un ```git checkout v1.0 -b "nombre rama"``` para conectarse al tag creandose una nuea rama con el nombre que lo pongamos 

> [!NOTE]
> Si no se pone -b y el nombre de la rama no pasa nada se pondra una solo en base a nombre del tag que es lo que me paso a mi

![](/pullReq_tag/fotos_individual/7.png)

