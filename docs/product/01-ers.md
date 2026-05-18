# ERS - Especificacion de Requisitos de Software

## 1. Nombre del producto

Vigente App / Senior Connexion.

## 2. Proposito

Construir una aplicacion multiplataforma orientada a adultos senior, inicialmente entre 60 y 74 anos, que ofrezca compania conversacional, interaccion por voz, actividades cognitivas, contenidos culturales, talleres, agenda, bienestar y apoyo.

La experiencia debe sentirse como una presencia cercana y humana, no como una herramienta tecnica ni como un robot.

## 3. Alcance inicial del MVP

El MVP debe permitir que el usuario:

- ingrese a la aplicacion de forma sencilla
- seleccione un agente humano de IA
- converse con el agente mediante una interfaz visual y de voz
- acceda a actividades cognitivas basicas
- consulte historias, cultura y contenidos recomendados
- vea talleres y cursos disponibles
- reciba ayuda y apoyo
- consulte una agenda simple de bienestar

## 4. Usuarios objetivo

### Usuario principal

Adulto colombiano senior, aproximadamente entre 60 y 74 anos, con interes en compania, cultura, entretenimiento, aprendizaje y bienestar.

### Usuario secundario futuro

Familiar o cuidador que desea conocer interacciones, bienestar general, agenda y momentos significativos del adulto senior.

### Administrador futuro

Equipo operativo encargado de configurar agentes, contenidos, talleres, cursos, recomendaciones y parametros de la plataforma.

## 5. Propuesta de valor

Vigente App ofrece acompanamiento conversacional y vivencial mediante agentes de IA con apariencia humana, voz natural, personalidad definida y capacidad de iniciar o sostener conversaciones significativas.

A diferencia de asistentes genericos, la aplicacion debe hablar en un tono cercano, entender contexto colombiano, ajustar ritmo y lenguaje, recordar conversaciones relevantes y sugerir actividades utiles.

## 6. Requisitos funcionales

### RF-001 Inicio y bienvenida

La aplicacion debe mostrar una pantalla de bienvenida clara, calida y de facil acceso.

Debe incluir:

- identidad visual de la marca
- mensaje de bienvenida
- agente destacado o acompanante visible
- accion principal de ingreso
- opcion de continuar con celular
- opcion de ayuda
- mensaje de privacidad y confianza

### RF-002 Seleccion de agente

La aplicacion debe permitir elegir entre varios agentes humanos de IA.

Inicialmente:

- Carolina: companera cercana
- Javier: conversador cultural, aproximadamente 40 anos
- Lucia: relajacion y meditacion, apariencia adulta madura pero un poco mas joven que la version inicial

Cada agente debe incluir:

- rostro humano
- nombre
- rol
- descripcion corta
- estado seleccionado o no seleccionado

### RF-003 Home principal

La aplicacion debe mostrar un home con acceso rapido a las funciones principales.

Debe incluir:

- saludo personalizado
- agente disponible
- acceso a conversacion
- juegos cognitivos
- talleres y cursos
- historias y cultura
- meditacion guiada
- ayuda y apoyo
- resumen del dia
- clima o recomendacion contextual
- recordatorios
- navegacion inferior

### RF-004 Conversacion con agente

La aplicacion debe permitir conversar con un agente humano de IA.

Debe incluir:

- panel visual del agente
- estado de conversacion en vivo
- historial de mensajes
- entrada por voz
- respuesta hablada
- sugerencias de conversacion
- tarjetas contextuales, como clima o recomendacion del dia
- opcion de finalizar o pausar conversacion

### RF-005 Interaccion por voz

La aplicacion debe permitir que el usuario hable y reciba respuestas habladas.

Debe contemplar:

- captura de audio
- transcripcion de voz a texto
- generacion de respuesta del agente
- sintesis de voz natural
- estado visual de escucha
- manejo de errores si no se entiende el audio

### RF-006 Juegos cognitivos

La aplicacion debe ofrecer juegos de estimulacion mental.

Juegos iniciales sugeridos:

- memoria activa
- trivia
- sopa de letras
- atencion

El detalle inicial del juego de memoria debe incluir:

- progreso
- nivel suave
- tiempo no estresante
- grilla de cartas
- parejas encontradas
- pista
- pausa
- continuar
- explicacion del beneficio del ejercicio

### RF-007 Historias y cultura

La aplicacion debe ofrecer contenidos para leer, escuchar o ver.

Debe incluir:

- cronicas o relatos culturales
- club de lectura
- historia de Colombia
- musica de epoca
- cine clasico
- museos recomendados
- opcion de guardar contenidos
- recomendaciones del agente

### RF-008 Talleres y cursos

La aplicacion debe mostrar talleres y cursos disponibles.

Debe incluir:

- taller destacado
- fecha y hora
- modalidad en linea o presencial
- cupos disponibles
- instructor o acompanante
- boton de inscripcion
- filtros por proximos, en linea, presenciales y mis inscritos
- calendario simple
- recomendacion del agente

### RF-009 Ayuda y apoyo

La aplicacion debe ofrecer una seccion de ayuda clara y tranquilizadora.

Debe incluir:

- hablar con el agente
- solicitar acompanamiento
- llamar a un familiar
- bienestar emocional
- guia de respiracion
- preguntas frecuentes
- directorio de apoyo
- soporte humano
- chequeo emocional simple
- contactos de confianza
- mensaje de privacidad y disponibilidad

### RF-010 Agenda y bienestar

La aplicacion debe permitir ver una agenda diaria y resumen de bienestar.

Debe incluir:

- medicamentos
- caminata
- conversacion con agente
- club de lectura
- hidratacion
- estado de animo
- sueno
- movimiento
- vida social
- recomendacion del agente
- logros de la semana

### RF-011 Panel familiar futuro

La aplicacion debe contemplar una version futura para familiares.

Debe incluir potencialmente:

- resumen de interacciones
- bienestar emocional
- actividades proximas
- recordatorios
- companera activa
- momentos favoritos
- acciones rapidas

## 7. Requisitos no funcionales

### RNF-001 Accesibilidad

La aplicacion debe tener tipografia grande, alto contraste, botones amplios y lenguaje claro.

### RNF-002 Usabilidad senior

La experiencia debe evitar saturacion, tecnicismos y flujos complejos.

### RNF-003 Disponibilidad

La propuesta debe contemplar disponibilidad 24/7 para interacciones basicas.

### RNF-004 Privacidad

La informacion personal, conversaciones, contactos y datos de bienestar deben tratarse como informacion sensible.

### RNF-005 Seguridad

Debe existir autenticacion, autorizacion, cifrado en transito y proteccion de datos almacenados.

### RNF-006 Escalabilidad

La arquitectura debe permitir crecer en usuarios, conversaciones, audios, agentes y contenidos.

### RNF-007 Observabilidad

Debe contemplar logs, metricas, trazabilidad de errores y monitoreo de servicios criticos.

### RNF-008 Modularidad

Las funcionalidades deben separarse por dominios: usuarios, agentes, conversacion, contenidos, actividades, agenda y soporte.

## 8. Supuestos

- El producto iniciara con un MVP.
- Los agentes seran representaciones humanas, no robots.
- La voz y la IA podran integrarse mediante servicios externos.
- El backend podra alojarse en AWS.
- La tecnologia movil definitiva aun esta en evaluacion.

## 9. Fuera de alcance inicial

- Avatar 3D avanzado en tiempo real.
- Panel administrativo completo.
- Integracion institucional real de talleres.
- Historia clinica o funcionalidades medicas reguladas.
- Monitoreo medico activo.
- Reemplazo de cuidadores humanos.
