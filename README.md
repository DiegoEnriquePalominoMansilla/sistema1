## Requerimientos

+ Platforma: Windows / Linux
+ Procesador con soporte SSE2
+ PHP ≥ 5.5.1
+ MySQL ≥ 5.1.0
+ Servidor HTTP Apache

## Instalación
Puede instalar y acceder a él StockAPP súper fácil. Recuerde que debe eliminar la carpeta "instalar" después de terminada la instalación. (Instalación "Paso a Paso" se encuentra desactualizada, intalación manual )

Ejemplo
```
# Copyright (C) 2015 StockApp <http://qualtivacr.com>
# nginx configuration
location / {
if (!-e $request_filename){
rewrite ^(.*)$ /$1.php break;
}
}
location /reimprimir {
rewrite ^/reimprimir/(.+)$ /re-imprimir.php?id=$1;
}
location /estado {
rewrite ^/estado-de-cuenta/(.+)/(.+)$ /estadodecuenta.php?id=$1&title=$2;
}
```
## Lista Desarrollo :octocat:
- [x] Módulo Multi-usuario 
- [x] Módulo Multi-Caja
- [x] Módulo Multi-establecimiento
- [x] Módulo de Productos
- [x] Módulo de Ventas
- [x] Módulo de Clientes
- [x] Módulo de Proveedores
- [x] Módulo de Categorías (Departamentos)
- [x] Módulo de Kardex (General/Productos)
- [x] Módulo de Notificaciones
- [x] Módulo de Inventario
- [x] Módulo de Entradas y Salidas de Dinero
- [x] Módulo de Caja Chica
- [x] Módulo de Cortes de Caja
- [ ] Módulo de Multi-Tabs Caja Temporal(Multiples clientes, Bares, Restaurantes, entre otros)
- [ ] Generación de reportes por rango de fecha
- [ ] Impresión de reportes en Word, Excel & PDF
