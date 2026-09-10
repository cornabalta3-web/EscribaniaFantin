# Módulos del sistema

Propuesta de cómo se parte el sistema y en qué orden lo construimos.
**Es un borrador para discutir**, no una decisión tomada.

## El mapa

```
                    ┌──────────────────┐
                    │   EXPEDIENTES    │   el centro de todo
                    └────────┬─────────┘
                             │
     ┌──────────┬────────────┼────────────┬──────────┐
     │          │            │            │          │
┌────┴────┐┌────┴────┐┌──────┴─────┐┌─────┴────┐┌────┴─────┐
│ PARTES  ││ OBJETOS ││ DOCUMENTOS ││ AGENDA Y ││PROTOCOLO │
│personas ││inmuebles││ archivos y ││VENCIMIEN.││escrituras│
│empresas ││ rodados ││ plantillas ││  plazos  ││ y folios │
└─────────┘└─────────┘└────────────┘└──────────┘└──────────┘
```

## Orden propuesto

### Fase 1 — El esqueleto
1. **Partes** — personas y empresas. Es la base de todo lo demás y el módulo
   más simple: buen lugar para aprender sin romper nada importante.
2. **Expedientes** — crear un trámite, asignarle partes, moverlo entre estados.

Con esto ya hay algo *usable*: saber qué trámites hay y en qué estado están.

### Fase 2 — El día a día
3. **Documentos** — subir y versionar archivos por expediente.
4. **Agenda y vencimientos** — plazos, certificados por vencer, alertas.

### Fase 3 — Lo notarial pesado
5. **Protocolo** — escrituras, numeración correlativa, folios. Se deja para
   después *a propósito*: es lo que más rigor exige y conviene llegar con
   experiencia.
6. **Objetos** — inmuebles y rodados como fichas reutilizables.

### Fase 4 — Lo que multiplica
7. **Generación de documentos** — armar minutas y borradores con datos ya
   cargados.
8. **Portal del cliente** — que el cliente consulte su trámite solo.

## Por qué este orden

- Cada fase deja algo que se puede usar de verdad, no un pedazo a medio hacer.
- Empieza por lo simple y de bajo riesgo, y deja el protocolo (donde un error
  tiene consecuencias legales) para cuando tengamos oficio.
- Nada de la fase 1 depende de decisiones que todavía no tomamos.

## Discusión abierta

- [ ] ¿El orden es el correcto desde el punto de vista de la escribanía?
- [ ] ¿Cuál es el dolor más grande hoy? Quizá convenga atacar eso primero.
- [ ] ¿Hay algún módulo que falte en el mapa?
