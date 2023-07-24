# marfeel-app

Aplicacion estructurada de acuerdo a lo requerido para el test sysops de Marfeel.

`/enviroments/apps/static:` Imagen nginx con un alb.ingress que re direcciona todos los request / a la pagina estatica /static.html, que cambia el texto de acuerdo al branch.

`/enviroments/apps/api`: Imagen ehosever con alb.ingress que re direcciona todos los request /api al service.

## ingress

Es necesario modificar las subnets de acuerdo al cluster donde pertenece.

    alb.ingress.kubernetes.io/subnets: subnet-0c820c04ce5d9e310, subnet-0777ffd8b26161b38
