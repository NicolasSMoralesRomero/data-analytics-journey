# Data Audit — Day 1

## Dataset: [customer_support_tickets]
## Fecha: [18/5/2026]

## Grain
Cada Fila representa un ticket diferente, ya que esta guardado en un id diferente incremental empezando por id 1.

## Columnas encontradas

* `Ticket ID`: **Alta**. ID numérico generado por el sistema.
* `Customer Name`: **Sospechosa**. Nombre del cliente ingresado por el mismo cliente.
* `Customer Email`: **Sospechosa**. Email del cliente ingresado por el mismo cliente.
* `Customer Age`: **Media**. Edad del cliente ingresado por el mismo cliente.
* `Customer Gender`: **Media**. Genero del cliente ingresado por el mismo cliente.
* `Product Purchased`: **Media**. Producto comprado por el cliente.
* `Date of Purchase`: **Media**. Fecha de la compra indicada por el cliente.
* `Ticket Type`: **Alta**. Tipo de motivo de contacto del cliente.
* `Ticket Subject`: **Alta**. Motivo de contacto del cliente.
* `Ticket Description`: **Alta**. Descripción del contacto del cliente.
* `Ticket Status`: **Alta**. Estado actual del caso.
* `Resolution`: **Alta**. En caso de estar en proceso, la resolución esta vacia.
* `Ticket Priority`: **Alta**. Prioridad del caso.
* `Ticket Channel`: **Alta**. Medio por donde ingreso el reclamo del cliente.
* `First Response Time`: **Alta**. Fecha y hora de la primera respuesta.
* `Time to Resolution`: **Alta**. Fecha y hora de la resolucion.
* `Customer Satisfaction Rating`: **Alta**. Calificación que el cliente brinda a la atención.


## Anomalías detectadas

1. Vi casos donde el nombre empieza con su titulo profesional (ej. Dr. Charles Cameron), adicional el mail puede no estar vinculado al nombre (en el ejemplo del doctor Charles el mail brindado es yhamilton@example.org)

## Preguntas sin respuesta

1. ¿No se especifica la zona horaria de los casos?