# Actividad entregable POO 19 de febrero de 2025.
# Realizado por Rafael David Palau.
# Archivo en .md para visualizar el diagrama en Mermaid.
# Ejercicio número 4: Tienda de música.

```
classDiagram
    class Album {
        - String codigo
        - String titulo
        - Date fechaLanzamiento
        + getCodigo()
        + setCodigo()
        + getTitulo()
        + setTitulo()
        + getFechaLanzamiento()
        + setFechaLanzamiento()
    }

    class Cliente {
        - String id
        - Date fechaRegistro
        + getId()
        + setId()
        + getFechaRegistro()
        + setFechaRegistro()
    }

    class Compra {
        - Date fechaCompra
        - Boolean devuelto
        + getFechaCompra()
        + setFechaCompra()
        + setDevuelto()
        + registrarCompra()
        + registrarDevolucion()
    }

    Cliente "1" --> "0..*" Compra : se-asocia
    Album "1" o-- "0..*" Compra : se-agrega
```
