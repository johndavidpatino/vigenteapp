# Arquitectura tecnica - Vigente App / Senior Connexion

## 1. Objetivo

Definir una arquitectura inicial para construir el MVP de Vigente App / Senior Connexion, manteniendo flexibilidad para decidir la tecnologia movil definitiva.

La arquitectura debe permitir:

- experiencia conversacional por voz
- agentes configurables
- actividades cognitivas
- contenidos culturales
- talleres y cursos
- agenda y bienestar
- soporte y contactos de confianza
- version futura de panel familiar

## 2. Principio arquitectonico principal

Separar claramente:

- frontend movil o web
- backend de negocio
- servicios de IA
- servicios de voz
- almacenamiento de datos
- contenido y multimedia
- observabilidad

La app movil no debe contener reglas criticas de negocio ni secretos de IA. La orquestacion sensible debe pasar por backend.

## 3. Opciones de frontend

### Opcion A: React Native + Expo

Recomendada para MVP si se busca velocidad y una sola base para iOS y Android.

Ventajas:

- desarrollo rapido
- experiencia mas nativa que una webview
- una sola base de codigo
- buen ecosistema
- posibilidad de evolucionar a modulos nativos

Riesgos:

- dependencia opcional de servicios Expo/EAS si se usan builds en la nube
- algunas integraciones nativas pueden requerir configuracion adicional

### Opcion B: React Native CLI

Adecuada si se quiere React Native pero con mayor control nativo desde el inicio.

Ventajas:

- mayor control de proyectos iOS/Android
- menos dependencia operativa de Expo

Riesgos:

- configuracion mas compleja
- curva mayor para builds y dependencias nativas

### Opcion C: SwiftUI + Kotlin/Jetpack Compose

Adecuada si se necesita maxima experiencia nativa.

Ventajas:

- maximo rendimiento e integracion nativa
- mejor control de accesibilidad avanzada

Riesgos:

- doble desarrollo
- mayor costo
- mayor tiempo de salida al mercado

### Opcion D: Web/PWA

Adecuada para validar rapido con cliente y usuarios.

Ventajas:

- menor costo inicial
- despliegue rapido
- compatible con AWS Amplify, S3 o CloudFront

Riesgos:

- experiencia movil menos nativa
- limitaciones en voz, notificaciones y capacidades del dispositivo

## 4. Recomendacion inicial

Para MVP se recomienda:

- Frontend movil: React Native + Expo o React Native CLI.
- Backend: .NET Core Web API.
- Infraestructura: AWS.
- Base de datos: SQL Server en RDS o PostgreSQL segun estrategia.
- Archivos: S3.
- Autenticacion: Cognito o autenticacion propia con .NET Identity.
- IA y voz: servicios externos orquestados por backend.

La decision final entre Expo y React Native CLI debe tomarse despues de validar:

- necesidades de voz en tiempo real
- avatar animado
- notificaciones push
- presupuesto de builds
- requerimientos de publicacion
- nivel de control nativo requerido

## 5. Componentes logicos

### Frontend App

Responsabilidades:

- interfaz senior-friendly
- navegacion
- captura de audio
- reproduccion de voz
- visualizacion de agente
- actividades interactivas
- agenda local visual
- consumo de APIs backend

No debe guardar secretos ni llamar directamente APIs sensibles de IA si implican llaves privadas.

### Backend API

Responsabilidades:

- autenticacion y autorizacion
- perfiles de usuario
- configuracion de agentes
- orquestacion de conversacion
- memoria conversacional
- historial
- recomendaciones
- agenda
- talleres
- contenidos
- contactos de confianza
- integracion con IA, voz y notificaciones

### Servicio de conversacion

Responsabilidades:

- recibir texto transcrito o mensaje del usuario
- enriquecer con contexto permitido
- seleccionar personalidad del agente
- generar respuesta
- registrar conversacion
- retornar texto, intencion y metadata

### Servicio de voz

Responsabilidades:

- speech-to-text
- text-to-speech
- manejo de errores de audio
- configuracion de voz por agente

Puede ser externo, pero debe integrarse desde backend o mediante tokens temporales controlados.

### Servicio de agentes

Responsabilidades:

- definir nombre, rol, personalidad y tono
- reglas de conversacion
- voz asociada
- avatar asociado
- limites de seguridad
- temas sugeridos

### Servicio de contenidos

Responsabilidades:

- historias y cultura
- recomendaciones
- audios
- videos cortos
- categorias
- favoritos

### Servicio de actividades

Responsabilidades:

- juegos cognitivos
- progreso
- puntajes no competitivos
- beneficios del ejercicio
- recomendaciones de continuidad

### Servicio de agenda y bienestar

Responsabilidades:

- recordatorios
- agenda diaria
- hidratacion
- caminatas
- actividades sociales
- sueno y animo si se decide capturar
- logros de la semana

### Servicio de soporte

Responsabilidades:

- ayuda y apoyo
- contactos de confianza
- llamadas o mensajes
- directorio de apoyo
- solicitudes de acompanamiento

## 6. Arquitectura AWS sugerida

### MVP simple

- App movil o web
- Amazon API Gateway o Application Load Balancer
- .NET Core Web API en ECS, Lambda o Elastic Beanstalk segun decision
- Amazon RDS
- Amazon S3
- Amazon CloudWatch
- Amazon SNS o Pinpoint para notificaciones futuras
- AWS Secrets Manager o SSM Parameter Store

### Serverless parcial

- API principal en .NET Core
- Lambdas para eventos asincronos
- S3 para audios e imagenes
- EventBridge para recordatorios y tareas programadas
- SQS para trabajos de procesamiento

## 7. Modelo inicial de dominios

Entidades sugeridas:

- User
- UserProfile
- Agent
- AgentPersonality
- Conversation
- ConversationMessage
- VoiceSession
- Activity
- CognitiveGame
- GameSession
- ContentItem
- ContentFavorite
- Workshop
- WorkshopEnrollment
- Reminder
- WellbeingCheck
- TrustedContact
- SupportRequest
- FamilyMember

## 8. Integraciones potenciales

### IA conversacional

- generacion de respuestas
- clasificacion de intenciones
- resumen de memoria
- recomendaciones

### Voz

- transcripcion
- sintesis de voz
- voces por agente

### Avatar

Fase inicial:

- imagen estatica o video corto del agente

Fase futura:

- avatar animado
- sincronizacion de labios
- expresiones faciales

### Notificaciones

- recordatorios
- talleres
- agenda
- mensajes familiares

## 9. Seguridad y privacidad

Requisitos:

- HTTPS obligatorio
- autenticacion segura
- autorizacion por rol
- cifrado de datos sensibles
- proteccion de llaves de IA
- control de acceso a audios, imagenes y archivos
- politicas claras de retencion de conversaciones
- consentimiento informado

## 10. Observabilidad

Se deben registrar:

- errores de API
- latencia de conversacion
- fallos de voz
- uso de agentes
- eventos de actividades
- errores de autenticacion
- costos estimados de servicios IA y voz

## 11. Decisiones pendientes

- React Native con Expo o sin Expo.
- Base de datos SQL Server vs PostgreSQL.
- Autenticacion Cognito vs .NET Identity.
- Proveedor de voz.
- Proveedor de avatar.
- Nivel de memoria conversacional permitido.
- Estrategia de consentimiento y privacidad.
- Si el panel familiar entra en MVP o fase 2.

## 12. Recomendacion de MVP tecnico

Construir primero:

1. Prototipo UI navegable.
2. Backend minimo con usuarios, agentes y conversaciones mockeadas.
3. Integracion IA textual.
4. Entrada y salida de voz.
5. Persistencia de conversaciones.
6. Juego de memoria local.
7. Agenda y recordatorios basicos.
8. Contenidos y talleres mockeados.

Luego evolucionar a:

- avatar animado
- panel familiar
- recomendaciones avanzadas
- integraciones institucionales
