# Visión

> Borrador. Este documento lo acordamos entre los dos antes de escribir código.
> Si algo acá no te cierra, no lo cambies en silencio: abrí un issue y discutámoslo.

## El problema

Hoy la escribanía maneja la información repartida entre carpetas de papel,
planillas de cálculo, carpetas de Windows y la cabeza de quien lleva cada
trámite. Eso produce:

- Nadie sabe con certeza en qué estado está un trámite sin preguntar.
- Vencimientos e inscripciones que se pasan por alto.
- Datos de una misma persona cargados de nuevo en cada expediente.
- Documentos con varias versiones y ninguna claramente definitiva.
- Si falta la persona que lleva el trámite, se frena.

## Qué queremos

Un sistema **integral**: una sola base de datos donde vive toda la operación de
la escribanía, y desde la que se consulta y se produce todo lo demás.

La regla de diseño: **un dato se carga una sola vez**. El nombre de un cliente,
los datos de un inmueble o el número de una escritura se cargan una vez y se
reutilizan en todos los trámites y documentos donde hagan falta.

## Para quién

| Perfil | Qué necesita del sistema |
|---|---|
| Escribano/a | Ver el estado global, firmar, controlar el protocolo |
| Empleado/a | Cargar datos, avanzar trámites, preparar documentos |
| Cliente | Saber en qué anda su trámite y qué papeles tiene que traer |

## Qué NO es (por ahora)

Definir los límites es tan importante como definir el alcance.

- No es un sistema contable ni de facturación.
- No es un sistema de liquidación de sueldos.
- No reemplaza los sistemas oficiales de los registros; se integra con ellos si
  se puede, pero no los sustituye.

## Cómo sabremos que sirve

- Buscar un expediente y entender su estado: menos de 30 segundos.
- Ningún vencimiento se pasa sin que el sistema haya avisado.
- Cargar un cliente que ya existe: nunca hace falta.
