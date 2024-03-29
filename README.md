# Docuemtación Guide.

##### Subir cambios al servidor remoto.

```bash
  $ hugo

  $ git add *; git commit -m "Actualización prueba"; git push origin master
```

##### Iniciar el servidor de manera local en segundo plano.

```bash
  $ hugo serve -D &
```
> El proyecto corre en *localhost:1313*

###### Para modificar aspectos del tema actual el archivo (theme.css) se encuentra en la siguiente ruta.

> guide/themes/hugo/static/css/theme.css

## Clonar el repositorio en otro dispositivo

**Dispositivo local**

- Clonar el repositorio desde git

```git
git clone https://github.com/Luis-Salinas-SD/guide.git
```

- Una vez en el directorio **guide** debemos ejecutar el siguiente comando.

```git
git submodule add https://github.com/Luis-Salinas-SD/hugoo.git themes/hugo
```

- Debemos remplazar el archivo **theme.css** que se encuntra en la dirección **guide/themes/hugoo/static/static/css** por el archivo **_theme.css_** que se encutra en el home del directorio **guide**.
- Para finalizar solo debemos editar el archivo **config.toml**, remplazando el parametro theme por `hugoo`
## ¡Importante!
> _Una vez que se hayan hecho cambios solo se tienen que subir los archivos **.md** que se hayan editado los demas cambios del tema **no** ya que crearian conflicto._
