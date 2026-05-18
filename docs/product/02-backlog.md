# Backlog funcional - Vigente App / Senior Connexion

## Convenciones

Prioridad sugerida:

- P0: indispensable para MVP
- P1: importante para MVP ampliado
- P2: version futura

Formato:

- Epica
- Historia de usuario
- Criterios de aceptacion

---

## EP-01 Onboarding e ingreso

### HU-001 Pantalla de bienvenida

**Como** adulto senior  
**quiero** ver una pantalla de bienvenida clara y calida  
**para** entender rapidamente que la aplicacion me acompanara.

Prioridad: P0

Criterios de aceptacion:

- La pantalla muestra logo y nombre de producto.
- La pantalla muestra un mensaje de bienvenida.
- La pantalla muestra un agente humano destacado.
- Existe boton principal `Ingresar`.
- Existe opcion `Continuar con celular`.
- Existe opcion `Necesito ayuda`.
- Existe mensaje de privacidad y confianza.

### HU-002 Ingreso con celular

**Como** usuario senior  
**quiero** ingresar con mi numero celular  
**para** evitar recordar usuario y contrasena.

Prioridad: P1

Criterios de aceptacion:

- El usuario puede ingresar su numero celular.
- El sistema valida formato basico.
- El sistema puede enviar codigo OTP.
- El usuario puede confirmar el codigo.
- Si el codigo es incorrecto se muestra mensaje simple.

---

## EP-02 Seleccion de agente

### HU-003 Ver agentes disponibles

**Como** usuario senior  
**quiero** ver varios agentes humanos disponibles  
**para** elegir con quien me siento mas comodo.

Prioridad: P0

Criterios de aceptacion:

- Se muestran Carolina, Javier y Lucia.
- Cada agente tiene foto o avatar humano.
- Cada agente tiene nombre, rol y descripcion.
- Carolina aparece seleccionada por defecto.
- Javier debe verse aproximadamente de 40 anos.
- Lucia debe verse como adulta madura, cercana a finales de los 40 o 50.
- La pantalla mantiene tono humano y no robotico.

### HU-004 Seleccionar agente

**Como** usuario senior  
**quiero** seleccionar un agente  
**para** personalizar mi experiencia de compania.

Prioridad: P0

Criterios de aceptacion:

- Al tocar un agente cambia el estado seleccionado.
- Solo puede haber un agente seleccionado a la vez.
- El boton `Continuar` confirma la seleccion.
- La seleccion se conserva al volver al home.

---

## EP-03 Home principal

### HU-005 Ver home personalizado

**Como** usuario senior  
**quiero** ver un home con opciones claras  
**para** saber rapidamente que puedo hacer.

Prioridad: P0

Criterios de aceptacion:

- El home muestra saludo personalizado.
- Muestra agente disponible.
- Muestra acceso a conversacion.
- Muestra juegos cognitivos.
- Muestra talleres y cursos.
- Muestra historias y cultura.
- Muestra meditacion guiada.
- Muestra ayuda y apoyo.
- Muestra resumen del dia.
- Muestra navegacion inferior.

### HU-006 Ver recomendacion diaria

**Como** usuario senior  
**quiero** recibir una recomendacion simple del dia  
**para** sentir acompanamiento y orientacion.

Prioridad: P1

Criterios de aceptacion:

- El home muestra una tarjeta de recomendacion.
- La recomendacion usa lenguaje cercano.
- La recomendacion puede estar relacionada con clima, actividad o bienestar.

---

## EP-04 Conversacion con agente

### HU-007 Iniciar conversacion

**Como** usuario senior  
**quiero** iniciar una conversacion con mi agente  
**para** sentirme acompanado.

Prioridad: P0

Criterios de aceptacion:

- Existe boton `Conversar ahora`.
- Al entrar se muestra el panel visual del agente.
- Se muestra estado de conversacion en vivo.
- El agente saluda al usuario.
- Se muestran sugerencias de temas.

### HU-008 Hablar por voz

**Como** usuario senior  
**quiero** hablar en lugar de escribir  
**para** interactuar de forma natural.

Prioridad: P0

Criterios de aceptacion:

- Existe boton grande de microfono.
- La interfaz indica cuando esta escuchando.
- El audio se transcribe.
- El agente responde con texto y voz.
- Si no se entiende el audio se solicita repetir de forma amable.

### HU-009 Conversacion proactiva

**Como** usuario senior  
**quiero** que el agente tambien me haga preguntas  
**para** sentir una conversacion real.

Prioridad: P0

Criterios de aceptacion:

- El agente puede iniciar preguntas simples.
- El agente puede preguntar por el dia, clima, animo o intereses.
- La conversacion evita sonar robotica.
- La conversacion respeta ritmo pausado.

---

## EP-05 Juegos cognitivos

### HU-010 Ver juegos cognitivos

**Como** usuario senior  
**quiero** ver juegos de estimulacion mental  
**para** ejercitar mi mente de forma agradable.

Prioridad: P0

Criterios de aceptacion:

- Se muestran memoria, trivia, sopa de letras y atencion.
- Cada juego tiene icono, descripcion y progreso.
- La pantalla mantiene tarjetas grandes y legibles.

### HU-011 Jugar memoria activa

**Como** usuario senior  
**quiero** jugar memoria activa  
**para** encontrar parejas y ejercitar mi memoria.

Prioridad: P0

Criterios de aceptacion:

- Se muestra titulo `Juego cognitivo: Memoria activa`.
- Se muestra progreso de parejas encontradas.
- Se muestra nivel suave.
- Se muestra temporizador no estresante.
- Se muestra grilla 4x3 de cartas.
- Algunas cartas aparecen volteadas y otras ocultas.
- Las parejas encontradas se resaltan.
- Existe boton `Pista`.
- Existe boton `Pausar`.
- Existe boton `Continuar`.
- Se muestra beneficio del ejercicio.

---

## EP-06 Historias y cultura

### HU-012 Ver contenidos culturales

**Como** usuario senior  
**quiero** explorar historias y cultura  
**para** leer, escuchar y conversar sobre temas significativos.

Prioridad: P1

Criterios de aceptacion:

- Existe seccion `Historias y cultura`.
- Hay contenido destacado.
- Hay opciones de lectura, audio o video corto.
- Cada contenido tiene descripcion corta.
- El usuario puede guardar contenidos.

### HU-013 Recibir recomendacion cultural del agente

**Como** usuario senior  
**quiero** recibir recomendaciones de Carolina  
**para** descubrir contenidos acordes a mis intereses.

Prioridad: P1

Criterios de aceptacion:

- Se muestra una tarjeta `Carolina te recomienda`.
- La recomendacion tiene accion clara.
- El texto es cercano y breve.

---

## EP-07 Talleres y cursos

### HU-014 Ver talleres disponibles

**Como** usuario senior  
**quiero** ver talleres y cursos disponibles  
**para** aprender y compartir nuevas experiencias.

Prioridad: P1

Criterios de aceptacion:

- Se muestra taller destacado.
- Se muestran fecha, hora y modalidad.
- Se muestran cupos disponibles.
- Se muestran talleres en tarjetas.
- Existen filtros por proximos, en linea, presenciales y mis inscritos.

### HU-015 Inscribirme a taller

**Como** usuario senior  
**quiero** inscribirme a un taller  
**para** participar en actividades de aprendizaje y socializacion.

Prioridad: P1

Criterios de aceptacion:

- Existe boton `Inscribirme`.
- Al inscribirse se muestra confirmacion clara.
- El taller aparece en mis inscritos.
- Se puede agregar a la agenda.

---

## EP-08 Ayuda y apoyo

### HU-016 Acceder a ayuda inmediata

**Como** usuario senior  
**quiero** tener ayuda visible y cercana  
**para** sentirme seguro si necesito orientacion.

Prioridad: P0

Criterios de aceptacion:

- Existe seccion `Ayuda y apoyo`.
- Se muestran acciones: hablar con Carolina, solicitar acompanamiento, llamar a familiar.
- Las acciones son grandes y faciles de tocar.
- El lenguaje es tranquilizador.

### HU-017 Registrar como me siento

**Como** usuario senior  
**quiero** indicar como me siento  
**para** recibir apoyo o recomendaciones adecuadas.

Prioridad: P1

Criterios de aceptacion:

- Se muestran cinco estados emocionales.
- El usuario puede seleccionar uno.
- El sistema guarda el estado seleccionado.
- Si el estado es negativo, se sugieren recursos de apoyo.

### HU-018 Contactar personas de confianza

**Como** usuario senior  
**quiero** llamar o escribir a mis contactos de confianza  
**para** recibir ayuda de personas cercanas.

Prioridad: P1

Criterios de aceptacion:

- Se listan contactos de confianza.
- Cada contacto tiene relacion.
- Existen acciones de llamar y mensaje.
- Existe opcion de gestionar contactos.

---

## EP-09 Agenda y bienestar

### HU-019 Ver agenda diaria

**Como** usuario senior  
**quiero** ver mi agenda del dia  
**para** recordar actividades importantes.

Prioridad: P1

Criterios de aceptacion:

- Se muestra timeline diario.
- Se muestran medicamentos, caminata, conversacion, club de lectura e hidratacion.
- Cada item tiene hora, icono, descripcion y estado.
- Existe boton para ver agenda completa.
- Existe boton para agregar recordatorio.

### HU-020 Ver logros de la semana

**Como** usuario senior  
**quiero** ver pequenos logros  
**para** sentir motivacion y continuidad.

Prioridad: P1

Criterios de aceptacion:

- Se muestran logros con iconos.
- Los logros usan lenguaje positivo.
- Se evita un tono competitivo o estresante.

---

## EP-10 Panel familiar futuro

### HU-021 Ver resumen del adulto senior

**Como** familiar  
**quiero** ver un resumen general de bienestar e interacciones  
**para** acompanarlo sin invadir su privacidad.

Prioridad: P2

Criterios de aceptacion:

- Se muestra resumen de interacciones recientes.
- Se muestra tendencia de bienestar emocional.
- Se muestran actividades proximas.
- Se muestran recordatorios.
- Se muestra companera activa.
- Se muestran momentos favoritos.

## Orden sugerido de construccion MVP

1. Sistema visual base.
2. Home estatico.
3. Seleccion de agente.
4. Conversacion mockeada.
5. Entrada de voz mockeada.
6. Juego memoria activa.
7. Ayuda y apoyo.
8. Agenda y bienestar.
9. Historias y cultura.
10. Talleres y cursos.
11. Integracion real IA/voz.
12. Persistencia y autenticacion.
