# Diagrama IT/OT para Horizonte Azul

Este diagrama muestra cómo se integran las tecnologías de planta (OT) y negocio (IT) mediante el uso de Inteligencia Artificial.

```mermaid
graph TD
    %% Definir nodos principales
    A[Planta - Operaciones OT]
    B[Negocio - Gestión IT]

    %% Subprocesos en Planta
    A1[Monitoreo de calidad del agua con IoT]
    A2[Mantenimiento predictivo con IA]
    A3[Optimización energética]

    %% Subprocesos en Negocio
    B1[ERP predictivo]
    B2[Chatbots IA para atención al cliente]
    B3[Análisis de datos ambientales]

    %% Integración IT/OT
    C[Plataforma Analítica Central con IA]

    %% Conexiones en Planta
    A --> A1
    A --> A2
    A --> A3

    %% Conexiones en Negocio
    B --> B1
    B --> B2
    B --> B3

    %% Conexión entre IT y OT
    A -->|Datos en tiempo real| C
    B -->|Análisis y decisiones| C
    C -->|Optimización y reportes| A
    C -->|Mejoras en gestión| B
