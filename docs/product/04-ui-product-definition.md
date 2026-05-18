# Definicion UI/UX basada en mockups

## 1. Objetivo

Convertir los mockups visuales en reglas documentadas para que el equipo y Codex puedan implementar pantallas consistentes sin depender unicamente de imagenes.

## 2. Principios visuales

- La experiencia debe sentirse humana y cercana.
- Los agentes deben tener rostro y cuerpo humano, no forma robotica.
- El diseno debe ser premium, calido y simple.
- El usuario senior debe poder entender cada accion sin explicaciones tecnicas.
- La interfaz debe usar tarjetas grandes, esquinas redondeadas y tipografia amplia.
- Los colores deben respetar el sistema visual definido en `tokens.css`.

## 3. Pantallas definidas

### 3.1 Login / bienvenida

Proposito:

Dar una primera impresion de confianza, compania y facilidad.

Elementos:

- logo
- titulo `Bienvenido`
- subtitulo de acompanamiento
- retrato de agente Carolina
- mensaje de agente
- boton `Ingresar`
- boton `Continuar con celular`
- enlace `Necesito ayuda`
- tarjeta de privacidad

Reglas:

- No mostrar demasiadas opciones.
- La accion principal debe ser muy visible.
- El agente debe transmitir calidez.

### 3.2 Seleccion de agente

Proposito:

Permitir al usuario escoger con quien desea interactuar.

Agentes iniciales:

- Carolina: companera cercana.
- Javier: conversador cultural, apariencia aproximada de 40 anos.
- Lucia: relajacion y meditacion, apariencia adulta madura y serena.

Elementos:

- titulo `Elige quien te acompana hoy`
- descripcion corta
- tarjetas de agentes
- indicador seleccionado
- boton `Continuar`
- mensaje de privacidad

Reglas:

- Las fotos deben parecer humanas, naturales y no genericas.
- Carolina puede aparecer seleccionada por defecto.
- El usuario debe entender claramente que puede cambiar de acompanante.

### 3.3 Home principal

Proposito:

Ser el punto de entrada diario de la experiencia.

Elementos:

- saludo personalizado
- agente disponible
- grid de acciones principales
- resumen del dia
- clima
- recomendacion
- recordatorio
- navegacion inferior

Acciones principales:

- Conversar ahora
- Juegos cognitivos
- Talleres y cursos
- Historias y cultura
- Meditacion guiada
- Ayuda y apoyo

Reglas:

- Todas las acciones deben ser grandes y visuales.
- El home no debe sentirse como dashboard empresarial.
- Debe transmitir acompanamiento diario.

### 3.4 Conversacion

Proposito:

Ofrecer una conversacion vivencial con agente humano.

Elementos:

- estado `En conversacion en vivo`
- panel visual del agente
- mensajes tipo chat
- tarjeta de clima
- recomendacion del dia
- microfono grande
- ondas de voz
- sugerencias de conversacion
- accion para finalizar

Reglas:

- El microfono debe ser la accion principal.
- El usuario no debe sentirse obligado a escribir.
- Las respuestas deben ser cortas, claras y naturales.

### 3.5 Actividades y estimulacion cognitiva

Proposito:

Mostrar actividades que ejercitan la mente y promueven bienestar.

Elementos:

- titulo `Actividades y estimulacion cognitiva`
- tarjetas de juegos
- progreso
- banner motivacional
- talleres culturales
- navegacion inferior

Juegos:

- Memoria
- Trivia
- Sopa de letras
- Atencion

Reglas:

- Los progresos deben motivar, no presionar.
- El lenguaje debe evitar evaluacion negativa.

### 3.6 Juego memoria activa

Proposito:

Permitir una actividad cognitiva simple y agradable.

Elementos:

- titulo del juego
- progreso
- nivel
- tiempo
- grilla de cartas
- parejas encontradas
- botones pista, pausar y continuar
- beneficio del ejercicio

Reglas:

- El temporizador no debe sentirse competitivo.
- El juego debe usar iconos simples y reconocibles.
- Los aciertos deben reforzarse positivamente.

### 3.7 Historias y cultura

Proposito:

Ofrecer contenidos para leer, escuchar, recordar y conversar.

Elementos:

- contenido destacado
- botones leer y escuchar
- lista de contenidos
- guardar favoritos
- recomendacion de Carolina
- callout de bienestar cultural

Categorias:

- cronicas de ciudad
- historia de Colombia
- musica de epoca
- cine clasico
- museos
- club de lectura

Reglas:

- Los contenidos deben conectar con memoria, identidad y conversacion.
- Debe priorizarse audio para usuarios que no quieran leer mucho.

### 3.8 Talleres y cursos

Proposito:

Facilitar descubrimiento e inscripcion en actividades.

Elementos:

- taller destacado
- fecha y hora
- modalidad
- cupos
- filtros
- tarjetas de talleres
- calendario
- recomendacion de agente

Reglas:

- La disponibilidad de cupos debe ser clara.
- La accion `Inscribirme` debe ser visible.
- Los talleres deben sentirse sociales y seguros.

### 3.9 Ayuda y apoyo

Proposito:

Brindar orientacion rapida y emocionalmente segura.

Elementos:

- ayuda inmediata
- hablar con agente
- solicitar acompanamiento
- llamar familiar
- modulos de bienestar
- respiracion
- preguntas frecuentes
- soporte humano
- estado emocional
- contactos de confianza
- privacidad 24/7

Reglas:

- No usar lenguaje alarmista.
- Las opciones de ayuda deben estar visibles.
- Los contactos de confianza deben ser faciles de accionar.

### 3.10 Agenda y bienestar

Proposito:

Ayudar al usuario a organizar su dia y celebrar pequenos logros.

Elementos:

- agenda diaria
- medicamentos
- caminata
- conversacion con agente
- club de lectura
- hidratacion
- resumen de bienestar
- recomendacion de agente
- logros de la semana

Reglas:

- La agenda debe ser clara, no sobrecargada.
- Los logros deben sentirse amables y motivadores.

### 3.11 Panel familiar futuro

Proposito:

Permitir a familiares acompanamiento no invasivo.

Elementos:

- resumen de interacciones
- bienestar emocional
- proximas actividades
- recordatorios
- companera activa
- momento favorito
- acciones rapidas

Reglas:

- Debe respetar la privacidad del adulto senior.
- Debe evitar tono medico o de vigilancia.
- Debe centrarse en bienestar y conexion.

## 4. Componentes reutilizables

- Header
- Logo
- Icon button
- Primary button
- Secondary button
- Card
- Agent card
- Feature card
- Voice panel
- Chat bubble
- Weather card
- Recommendation card
- Reminder row
- Activity card
- Workshop card
- Culture item
- Mood selector
- Trusted contact row
- Bottom navigation

## 5. Reglas de contenido

- Todo texto debe estar en espanol.
- Usar frases cortas.
- Evitar tecnicismos.
- Usar tono cercano y respetuoso.
- No infantilizar al adulto senior.
- Evitar mensajes que generen ansiedad.

## 6. Reglas para implementacion con Codex

Cuando se cree una pantalla, el prompt debe incluir:

- nombre de pantalla
- objetivo funcional
- componentes que debe usar
- datos mockeados
- criterios visuales
- restriccion de no crear estilos inline
- restriccion de no modificar archivos no relacionados

Ejemplo:

`Crea la pantalla de seleccion de agente usando el sistema visual existente. Reutiliza sc-header, sc-card, sc-agent-card y sc-button. No inventes colores. Mantener textos en espanol.`
