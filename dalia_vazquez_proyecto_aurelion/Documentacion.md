# Problemática: Clasificación de clientes para estrategias comerciales

## Objetivo
Identificar y clasificar a los clientes en diferentes categorías según su comportamiento de compra, con el fin de aplicar **estrategias comerciales personalizadas** que aumenten la fidelidad, reduzcan el abandono y fortalezcan la captación.

## Categorías de clientes

1. **Clientes frecuentes**
   - Definición: Clientes con **2 o más compras** y cuya **última compra fue hace menos de 14 días**.
   - Estrategia: 
     - Implementar programas de fidelización (descuentos exclusivos, puntos, promociones VIP).
     - Incentivar compras adicionales con recomendaciones de productos complementarios.

2. **Clientes en riesgo de abandono**
   - Definición: Clientes con **2 o más compras** y cuya **última compra fue hace más de 14 días**.
   - Estrategia:
     - Aplicar campañas de recuperación (cupones de descuento, correos recordatorios).
     - Ofrecer beneficios por regresar (envío gratis, 2x1 en su categoría más comprada).

3. **Clientes únicos**
   - Definición: Clientes con **solo 1 compra** en el historial.
   - Estrategia:
     - Diseñar campañas de bienvenida y retención (agradecimiento + incentivo para su segunda compra).
     - Generar confianza con testimonios, garantías y promociones de bajo riesgo.

## Beneficio esperado
- Mejor segmentación de la base de clientes.  
- Mayor eficacia en las campañas de marketing.  
- Incremento en la recurrencia de compra y reducción de clientes perdidos.  

# Esquema de Tablas y Tipos de Datos (Python)

## Tabla: Ventas
| Columna         | Tipo de Dato Python |
|-----------------|----------------------|
| id_venta        | int                  |
| fecha           | datetime.date        |
| id_cliente      | int                  |
| nombre_cliente  | str                  |
| email           | str                  |
| medio_pago      | str                  |

---

## Tabla: Productos
| Columna         | Tipo de Dato Python |
|-----------------|----------------------|
| id_producto     | int                  |
| nombre_producto | str                  |
| categoria       | str                  |
| precio_unitario | float (o int)        |

---

## Tabla: Detalle_ventas
| Columna         | Tipo de Dato Python |
|-----------------|----------------------|
| id_venta        | int                  |
| id_producto     | int                  |
| nombre_producto | str                  |
| cantidad        | int                  |
| precio_unitario | float (o int)        |
| importe         | float (o int)        |

---

## Tabla: Clientes
| Columna         | Tipo de Dato Python |
|-----------------|----------------------|
| id_cliente      | int                  |
| nombre_cliente  | str                  |
| email           | str                  |
| ciudad          | str                  |
| fecha_alta      | datetime.date        |
