# Fixtech — Prueba de Carga | JMeter

## Descripción
Prueba de carga sobre el flujo de compra de Fixtech (fixtech.com.ar),
simulando 10 usuarios simultáneos realizando 3 iteraciones cada uno.

## Objetivo
Evaluar el rendimiento y tiempo de respuesta del sitio bajo carga moderada,
identificando posibles cuellos de botella en el flujo de compra.

## Herramienta
- Apache JMeter 5.6.3

## Configuración del Test
- Usuarios simultáneos: 10
- Ramp-up: 10 segundos
- Iteraciones por usuario: 3
- Total de peticiones ejecutadas: 90

## Flujo Testeado
1. Página de Inicio
2. Página de Producto
3. Checkout

## Resultados

| Página | Tiempo Promedio | Tiempo Máximo | Error % |
|---|---|---|---|
| Página de Inicio | 73ms | 697ms | 0% |
| Página de Producto | 41ms | 60ms | 0% |
| Checkout | 3318ms | 7042ms | 0% |

## Conclusiones
- Página de inicio y producto responden de forma óptima bajo carga.
- El checkout presenta tiempos elevados (promedio 3.3s, máximo 7s),
  lo cual puede impactar negativamente la experiencia del usuario
  en momentos de mayor tráfico.
- Se recomienda investigar optimizaciones en el proceso de checkout.

## Archivos
- `Fixtech_LoadTest.jmx` — Test plan de JMeter
- `Fixtech_Resultados_LoadTest.csv` — Resultados exportados
