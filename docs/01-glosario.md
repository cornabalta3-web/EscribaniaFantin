# Glosario

Para que los dos (y el sistema) usemos las mismas palabras con el mismo
significado. Cada término de acá va a terminar siendo una tabla, un campo o una
pantalla del sistema.

> **Importante:** estas definiciones son un punto de partida y la terminología
> varía según la jurisdicción. Vos conocés el oficio: corregí lo que esté mal y
> agregá lo que falte. Ese es el primer trabajo real del proyecto.

## Términos del oficio

| Término | Definición de trabajo | Consecuencia en el sistema |
|---|---|---|
| **Expediente** / Trámite | Todo el trabajo asociado a un encargo concreto de un cliente, de principio a fin | Es la entidad central; casi todo cuelga de acá |
| **Escritura** | Documento matriz autorizado por el escribano e incorporado al protocolo | Registro con número, fecha y folio; único e inalterable una vez firmado |
| **Protocolo** | Colección ordenada de escrituras de un escribano en un año | Numeración correlativa sin huecos; el sistema debe garantizarlo |
| **Folio** | Hoja del protocolo donde se asienta la escritura | Rango de folios por escritura (desde–hasta) |
| **Parte** / Interviniente | Persona o empresa que participa en un acto (comprador, vendedor, apoderado…) | Una persona se carga una vez y participa en muchos expedientes con distinto rol |
| **Rol** | El papel que cumple una parte en ese acto puntual | El rol pertenece a la relación parte–expediente, no a la persona |
| **Poder** | Documento que habilita a alguien a actuar por otro | Tiene vigencia y alcance; el sistema debe alertar si está vencido |
| **Certificado** | Informe de un registro sobre el estado de un bien o persona | Tiene fecha de emisión y **plazo de validez**: fuente principal de vencimientos |
| **Inscripción** | Registro del acto ante el organismo correspondiente | Trámite con plazo legal; si se vence hay consecuencias reales |
| **Minuta** | Formulario de rogación para inscribir | Documento generado a partir de datos ya cargados |
| **Objeto** | El bien sobre el que versa el acto (inmueble, rodado, sociedad) | Entidad reutilizable: un inmueble aparece en varias operaciones a lo largo del tiempo |

## Términos del sistema

| Término | Qué queremos decir |
|---|---|
| **Estado** | En qué punto del circuito está un expediente (ej.: *en estudio de títulos*, *listo para firma*, *en inscripción*) |
| **Vencimiento** | Cualquier fecha límite que, si pasa, genera un problema |
| **Alerta** | Aviso automático del sistema antes de un vencimiento |
| **Usuario** | Quien entra al sistema (escribano, empleado) |
| **Permiso** | Qué puede ver y hacer cada usuario |

## Términos pendientes de definir

Anotá acá lo que aparezca y todavía no tenga definición acordada.

- [ ] (ejemplo) ¿Qué diferencia hacemos entre *expediente* y *acto* cuando una misma carpeta genera dos escrituras?
