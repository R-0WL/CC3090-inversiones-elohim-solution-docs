---
sidebar_position: 7
---

# Tablero estilo Kanban 

Visualiza el proceso completo de las solicitudes de los clientes

## ¿Qué es?
Un board que ayuda visualizar la etapa actual en la que se encuentra las diferentes solicitudes de los clientes. 

Actualmente se encuentran 3 etapas diferentes: 
- Pendiente de pago: el pedido del cliente no realizo el pago virtual, puede que lo haga mas tarde, lo haga el pago contra entrega o bien cancele el pedido. 
- Pago verificado: el pedido del cliente ya fue pagado mediante stripe. 
- Despachado: el pedido del cliente ya fue entregado o bien empaquetado para enviarlo a otra direccion. 

## Para qué sirve
- Visualizar el estado actual de las solicitudes de los clientes dentro de las diferentes sucursales 
- Actualizar en cualquier momento el estado actual de la solicitud.
- Visualizar la cantidad de dinero que se encuentra en cada etapa mediante los contadores en la parte superior de la pantalla. 
- Buscar una solicitud especifica, al escribir el id del pedido en la barra de buscador.
- Filtrar la busqueda de solicitudes medainte sucursales existentes. 
- Filtrar los pedidos visibles por periodo: hoy, esta semana, este mes o todos.

## Casos de uso
1. **Revision de Auditoria**: al contar con los contadores de dinero que se encuentra en cada estado de los pedidos. 
2. **Busqueda inmediata de pedidos**: verificacion que realmente se registrara la venta dentro del sistema, por si existe una queja de clientes. 
3. **Organizar al equipo de inventario**: al tener una representacion visual del estado actual de cada pedido.  
4. **Revision del dia**: filtrar solo los pedidos de hoy para enfocarse en lo pendiente de la jornada.

## Características clave
- **Validacion entre estados**: un pedido solo puede pasar a estados validos, evitando cambios por error.
- **Indicaciones mejoradas**: cada columna explica que significa y como mover los pedidos; si una columna esta vacia muestra "Sin pedidos en esta fase".
- **Buscador mejorado**: busqueda mas precisa por codigo de pedido.
- **Filtro por sucursal y por periodo** (Hoy, Esta semana, Este mes, Todos).
- **Actualizacion en tiempo real**: cuando entra un pedido nuevo, el tablero se actualiza automaticamente y muestra una notificacion.

## Integración con otras funciones
- Trabaja en conjunto con **Reportes** y **Dashboard**, ya que todo cambio que se realize en esta funcionalidad se reflejaran en las graficas diarias y mensuales de las sucursales. 