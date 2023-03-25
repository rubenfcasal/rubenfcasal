# R Machinery

Código fuente para generar mi página personal y blog (sobre R) 
[https://rubenfcasal.github.io](https://rubenfcasal.github.io),
empleando blogdown con Hugo.

NOTA: Esta web se generó empleando la versión 0.49.2 de Hugo, se debería poder reproducir ejecutando:

```
install.packages("blogdown")
blogdown::install_hugo("0.49.2")
# Si aparecen problemas descargar a carpeta local (e.g. "C:/rtools42"):
#   https://github.com/gohugoio/hugo/releases/download/v0.49.2/hugo_extended_0.49.2_Windows-64bit.zip
#   blogdown::install_hugo("C:/rtools42/hugo_extended_0.49.2_Windows-64bit.zip")
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

NOTAS: 

- Si aparecen problemas probar a ejecutar `blogdown::check_site()`.

- ["You'll see this message but it's harmless and can be ignored: Error: logged 1 error(s)"](https://community.rstudio.com/t/yaml-error-on-blogdown-update/86903) 