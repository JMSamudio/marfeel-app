# marfeel-app

Aplicacion estructurada de acuerdo a lo requerido para el test sysops de Marfeel.

/enviroments/apps/static: Imagen nginx con un alb.ingress que re direcciona todos los request / a la pagina estatica /static.html, que cambia el texto de acuerdo al branch.

/enviroments/apps/api: Imagen ehosever con alb.ingress que re direcciona todos los request /api al service.