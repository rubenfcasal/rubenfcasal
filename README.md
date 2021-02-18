# R Machinery

Código fuente para generar mi página personal y blog (sobre R) 
[https://rubenfcasal.github.io](https://rubenfcasal.github.io),
empleando blogdown con Hugo.

NOTA: Esta web se generó empleando la versión 0.49.2 de Hugo, se debería poder generar ejecutando:

```
install.packages(blogdown)
blogdown::install_hugo("0.49.2")
# blogdown::install_hugo("0.54.0") # Actualizar .Rprofile
```

Para previsualizar ejecutar:

```
blogdown::serve_site()
# blogdown::stop_server()
```

El sitio web (carpeta *public* de Hugo) está en el repositorio
[rubenfcasal/rubenfcasal.github.io](https://github.com/rubenfcasal/rubenfcasal.github.io).

NOTA: En (las nuevas versiones de) blogdown hay que ejecutar `blogdown::build_site()` para generarlo. 