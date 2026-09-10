# Prototipo — base del sistema

Un solo archivo, `index.html`. **Se abre con doble clic**, no hay que instalar nada.

Es el **esqueleto completo del sistema**: están los 7 módulos navegables, con la
identidad visual ya definida. Cada módulo se construye después por separado, pero
el marco donde encajan ya existe.

## Estado de cada módulo

| Módulo | Estado | Qué hace |
|---|---|---|
| Panel | funciona | Resumen del estudio: activos, listos para firma, vencidos, actividad reciente |
| Expedientes | funciona | Listado, búsqueda, filtro por estado, ficha con historial, alta, cambio de estado |
| Partes | funciona | Padrón de personas físicas y jurídicas, ficha con sus expedientes, alta |
| Vencimientos | funciona | Ordenado por urgencia, con vencidos marcados |
| Documentos | **falta** | La pantalla explica qué va a tener |
| Protocolo | **falta** | La pantalla explica qué va a tener |
| Reportes | **falta** | La pantalla explica qué va a tener |

## Decisiones de diseño

Están todas en el bloque `TOKENS` al principio del archivo. **Cambiar un color ahí
lo cambia en todo el sistema**, no hay que tocar nada más.

- **Neutros fríos y azul tinta.** Registro administrativo, no folleto.
- **Monoespaciada para números** de expediente, CUIT, fechas y folios: alinean en
  columna y se comparan de un vistazo.
- **El color dice algo.** Gris = en curso sin urgencia. Ámbar = requiere acción.
  Azul = trámite avanzando. Verde = terminado. Rojo = vencido.
- **Tema claro y oscuro**, según cómo tenga configurada la PC cada uno.

## Qué NO es

- Los datos quedan **solo en el navegador de esa computadora**. No se comparten
  entre PCs y no hay copia de seguridad.
- No hay usuarios ni contraseñas.
- **No cargar datos reales de clientes.** Es una maqueta.

## Cómo lo usamos para decidir

Abrilo, tocá todo, y por cada cosa que falte o sobre abrí un **Issue**. Ese es el
material con el que después se construye el sistema real.
