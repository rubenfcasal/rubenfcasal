# R Machinery

Código fuente para generar mi página personal y blog (sobre R) 
[https://rubenfcasal.github.io](https://rubenfcasal.github.io),
empleando blogdown con Hugo.

NOTA: Esta web se generó empleando la versión 0.49.2 de Hugo, se debería poder reproducir ejecutando:

```
install.packages("blogdown")
# En lugar de descargar e instalar directamente desde R:
# blogdown::install_hugo("0.49.2")
# Yo prefiero descargar la versión de hugo a una carpeta local (e.g. "C:\\util"):
#   https://github.com/gohugoio/hugo/releases/download/v0.49.2/hugo_extended_0.49.2_Windows-64bit.zip
# y posteriormente instalarlo:
blogdown::install_hugo("C:/util/hugo_extended_0.49.2_Windows-64bit.zip")
# Si se instala una nueva versión actualizar .Rprofile
#   blogdown::install_hugo("0.54.0") # 
```

Para generar (en nuevas versiones de blogdown) ejecutar:

```
# blogdown::build_site()
blogdown::build_site(build_rmd = 'timestamp') 
```

Para previsualizar ejecutar:

```
blogdown::serve_site()
# blogdown::stop_server()
```

El sitio web (carpeta *public* de Hugo) está en el repositorio
[rubenfcasal/rubenfcasal.github.io](https://github.com/rubenfcasal/rubenfcasal.github.io).

Para más detalles visitar la [web de blogdown](https://pkgs.rstudio.com/blogdown).

NOTAS: 

- Si aparecen problemas (como *Error: logged 2 error(s)*) probar a ejecutar `blogdown::check_site()`.

- ["You'll see this message but it's harmless and can be ignored: Error: logged 1 error(s)"](https://community.rstudio.com/t/yaml-error-on-blogdown-update/86903) 

- `packageVersion("blogdown")`: 1.19, *C:/Users/ruben.fcasal/AppData/Roaming/Hugo/0.49.2/hugo.exe*

```
devtools::install_version("blogdown", version = "1.11", repos = "https://ftp.cixug.es/CRAN")
```
