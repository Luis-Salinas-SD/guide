# Docuemtación Pagina oficial guide.

##### Subir cambios al servidor remoto.

```
  $ hugo

  $ git add *; git commit -m "Actualización prueba"; git push origin master
```

##### Iniciar el servidor de manera local en segundo plano.

```
  $ hugo serve -D &
```

###### Para modificar aspectos del tema actual el archivo (theme.css) se encuentra en la siguiente ruta.

> guide/themes/hugo/static/css/theme.css

#### Clonar el repositorio en otro dispositivo

**Dispositivo local**

- Clonar el repositorio desde git

```
  $ git clone <dirección del repo>
```

- Una vez en el directorio **guide** debemos ejecutar el siguiente comando.

```
git submodule add git@github.com:matcornic/hugo-theme-learn.git theme/hugoo
```

- Debemos remplazar el archivo **theme.css** que se encuntra en la dirección **guide/theme/hugoo/static/static/css** por el archivo **_theme.css_** que se encutra en el repo **_hugoo-theme_**.

> _Una vez que se hayan hecho cambios solo se tienen que subir los archivos .md que se hayan editado los demas cambios del tema **no** ya que crearian conflicto._
