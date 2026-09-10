# Cómo trabajamos

Guía desde cero. Si nunca usaste Git ni GitHub, empezá por acá.

## Las tres palabras que hay que entender

**Git** es un programa que guarda el historial de una carpeta. Cada vez que
decís "guardá este momento", Git anota qué cambió, quién lo cambió y cuándo.
Nunca se pierde nada y siempre se puede volver atrás.

**GitHub** es un sitio web donde vive una copia de esa carpeta con su historial,
para que los dos trabajemos sobre lo mismo desde computadoras distintas.

**Repositorio** (o *repo*) es esa carpeta con historial. Este proyecto es un
repositorio.

## Qué instalar

Instalá **GitHub Desktop**: https://desktop.github.com

Es Git con botones en vez de comandos. Para lo que necesitamos ahora alcanza y
sobra, y evita la parte más áspera del aprendizaje.

## El ciclo de trabajo

Cuatro pasos, siempre los mismos:

```
  1. RAMA          2. CAMBIOS        3. COMMIT         4. PULL REQUEST
  Crear una        Editar los        Guardar el        Pedirle al otro
  copia propia  →  archivos       →  momento con    →  que lo revise
  para trabajar    que haga falta    un mensaje        y lo incorpore
```

### 1. Rama (*branch*)

Una rama es una línea de trabajo paralela. Vos trabajás en la tuya, tu hermano
en la suya, y ninguno le rompe nada al otro hasta que decidan juntar.

Nombrala con lo que vas a hacer: `glosario-terminos-registrales`,
`corregir-definicion-de-protocolo`.

**Nunca trabajes directo sobre la rama `main`.** `main` es la versión buena,
la que los dos damos por válida.

### 2. Cambios

Editá los archivos con lo que sea: el Bloc de notas sirve. Los `.md` son texto
común con un poco de formato ([guía de Markdown](https://www.markdownguide.org/cheat-sheet/)).

### 3. Commit

Un *commit* es una foto del proyecto con un mensaje que explica qué cambiaste.

Mensajes útiles:
- ✅ `Corrijo la definición de folio: es un rango, no una hoja sola`
- ❌ `cambios`, `varias cosas`, `asdf`

Hacé commits chicos y frecuentes. Uno por idea, no uno por semana.

### 4. Pull Request (PR)

Un PR es: *"hice esto, ¿lo miramos y lo metemos en `main`?"*.

Es el corazón de trabajar de a dos. El otro ve exactamente qué líneas
cambiaron, comenta lo que no le cierra, se discute ahí mismo, y cuando los dos
están de acuerdo se aprueba y se incorpora.

Esa discusión queda guardada para siempre, atada al cambio que la generó.

## Reglas que nos ponemos

1. **Nadie escribe directo en `main`.** Todo entra por Pull Request.
2. **Un PR lo aprueba el otro**, no uno mismo. Aunque sea un cambio chico.
3. **Antes de empezar a trabajar, actualizá.** En GitHub Desktop: *Fetch origin*
   y luego *Pull*. Así arrancás desde lo último.
4. **Los desacuerdos se discuten en el PR o en un issue**, no por WhatsApp. Lo
   que se discute por chat se pierde; lo que se discute en GitHub queda.
5. **Nunca subas datos reales de clientes.** Ni nombres, ni documentos, ni
   escrituras. Para los ejemplos, inventá.

## Issues

Un *issue* es una anotación: algo que hay que hacer, algo que está mal, una
pregunta. Se le asigna a alguien y se cierra cuando se resuelve.

Úsenlo para todo lo que no sea obvio. Es la lista de pendientes compartida.

## Cuando algo sale mal

Se puede deshacer prácticamente todo. Git guarda el historial completo: si
borraste algo, si pisaste el trabajo del otro, si el archivo quedó hecho un
desastre — se recupera. **No tengas miedo de probar.**

La única forma real de romper algo es no usar el sistema.

## Primera prueba sugerida

Para ver si esto les sirve, antes de meterse con el sistema en serio:

1. Vos abrís una rama y corregís algo del [glosario](01-glosario.md) — seguro
   hay definiciones mal puestas.
2. Abrís un Pull Request.
3. Tu hermano lo revisa, comenta y lo aprueba.
4. Después él hace lo mismo con [los módulos](02-modulos.md) y vos revisás.

Si después de eso les resulta cómodo, seguimos. Si les resulta un estorbo, lo
hablamos y buscamos otra forma.
