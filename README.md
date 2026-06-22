# Chatbot para Solicitud de Vacaciones

## Descripción

Este proyecto corresponde al Trabajo Final Integrador de la carrera.

El objetivo es automatizar el proceso de solicitud de vacaciones mediante un chatbot capaz de validar empleados, consultar saldo disponible y registrar solicitudes.

## Objetivo

El objetivo de este proyecto es modelar y automatizar el proceso de solicitud de vacaciones mediante un chatbot, utilizando BPMN 2.0, una base de datos simulada en Excel y una máquina de estados para controlar el flujo de la conversación.

## Flujo del proceso

1. El usuario ingresa su legajo.
2. El sistema verifica si el empleado existe.
3. Se consulta el saldo de vacaciones disponible.
4. El usuario ingresa la fecha de inicio.
5. El usuario indica la cantidad de días solicitados.
6. El sistema valida la información.
7. La solicitud se registra.
8. Se informa el resultado al usuario.

## Máquina de Estados

- INICIO
- ↓
- ESPERANDO_LEGAJO
- ↓
- VALIDANDO_LEGAJO
- ↓
- CONSULTANDO_SALDO
- ↓
- ESPERANDO_FECHA
- ↓
- ESPERANDO_DIAS
- ↓
- VALIDANDO_SOLICITUD
- ↓
- REGISTRANDO_SOLICITUD
- ↓
- ENVIANDO_CONFIRMACION
- ↓
- FINALIZADO

## Casos contemplados

- Legajo inexistente.
- Saldo insuficiente.
- Fecha inválida.
- Texto en lugar de números.
- Cancelación de la operación.

## Decisiones del proceso (Gateways)

- ¿Empleado existe?
- ¿Tiene saldo suficiente?

Estas decisiones se encuentran representadas en el BPMN y son validadas por la lógica del chatbot.

## Tecnologías Propuestas

- Python
- Telegram Bot API
- Excel (Base de datos simulada)
- GitHub

## Estructura del Proyecto

```text
TFI_Chatbot_Vacaciones/
│
├── BPMN/
├── BaseDatos/
│   └── empleados.xlsx
├── Codigo/
│   └── chatbot.py
├── Documentacion/
│   └── TFI_Chatbot_Vacaciones.pdf
└── README.md
```

## Despliegue

1. Descargar el proyecto.
2. Abrir el archivo empleados.xlsx ubicado en la carpeta BaseDatos.
3. Ejecutar el archivo chatbot.py ubicado en la carpeta Codigo.
4. Seguir las instrucciones mostradas por el sistema.

## Funcionamiento

1. El usuario ingresa su legajo.
2. El sistema valida la existencia del empleado.
3. Se consulta el saldo disponible.
4. El usuario indica fecha y cantidad de días.
5. El sistema valida la solicitud.
6. La solicitud queda registrada.

## Autor

- Curell Dario
- Comision n°22

Trabajo Final Integrador - TUP
