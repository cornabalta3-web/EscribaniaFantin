# Registro de decisiones

Cada decisión importante se anota acá: **qué** decidimos, **cuándo** y sobre
todo **por qué**. Dentro de seis meses, cuando alguno pregunte "¿por qué
hicimos esto así?", la respuesta está escrita.

Formato: una decisión por sección, en orden cronológico. No se borran ni se
editan las viejas; si cambiamos de idea, se agrega una decisión nueva que
reemplaza a la anterior y se marca la vieja como *Reemplazada*.

---

## D-001 — Documentar antes de programar

**Fecha:** 2026-09-10
**Estado:** Vigente

**Decisión:** Antes de escribir código, escribimos qué tiene que hacer el
sistema (visión, glosario, módulos).

**Por qué:** Ninguno de los dos programa todavía. Escribir la definición nos
sirve para dos cosas al mismo tiempo: aclarar el sistema y aprender a trabajar
juntos con Git y GitHub sobre algo donde un error no rompe nada.

---

## D-002 — Sistema web en la nube

**Fecha:** 2026-09-10
**Estado:** Vigente

**Decisión:** El sistema va a ser una aplicación web alojada en la nube, a la
que se entra desde el navegador.

**Por qué:** Varias personas en la escribanía tienen que ver los mismos datos
actualizados. Una web centralizada evita instalar y sincronizar en cada PC, y
permite corregir un error una vez para todos.

**Pendiente:** definir dónde se alojan los datos y qué exige la normativa de
protección de datos y de secreto profesional. **Esto hay que consultarlo antes
de guardar un solo dato real de un cliente.**

---

## D-003 — Tecnología: sin decidir

**Fecha:** 2026-09-10
**Estado:** Abierta

Todavía no elegimos con qué se construye. Se decide cuando estén acordados los
módulos de la fase 1.

---

## Plantilla para decisiones nuevas

```
## D-00X — Título corto

**Fecha:** AAAA-MM-DD
**Estado:** Vigente | Reemplazada por D-00Y

**Decisión:** qué acordamos.

**Por qué:** las razones, incluidas las alternativas que descartamos.
```
