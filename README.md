# HLS-IA

Proyecto como practicante

Proyecto de Generacion de EPICRISIS
Objetivo: Con documentos medicos generar una epicrisis usando IA

Epicrisis: es un resumen clínico que se entrega al paciente al alta hospitalaria, y resume los aspectos 
más relevantes de su hospitalización, incluyendo el motivo de ingreso, diagnóstico, tratamiento, evolución
y recomendaciones para el paciente.
Es una herramienta importante para la continuidad del cuidado del paciente.

### ¿Como se genera?
Elaboración y Contenido:
Elaboración: La epicrisis es elaborada por el médico tratante o el equipo médico responsable de la atención del paciente.
Contenido: Debe incluir información clave como:
- Motivo de ingreso.
- Diagnóstico principal.
- Antecedentes relevantes del paciente.
- Procedimientos médicos realizados.
- Evolución de la enfermedad durante la hospitalización.
- Tratamiento recibido.
- Complicaciones presentadas.
- Indicaciones para el paciente al alta (medicamentos, dieta, controles, etc.)

## ¿Qué herramientas de IA se pueden usar?
Objetivo: Automatizar la generación con una plantilla.

Librerias importantes:
Modelos entrenados para salud
En un entorno hospitalario se podrías usar:
- scispaCy (NLP biomédico)
- ClinicalBERT (para texto clínico)
- Modelos de HuggingFace como [clinical-T5, biogpt, medalpaca]

## Requisitos comunes
transformers: para cargar los modelos
torch: para usar PyTorch (backend)
(opcional) accelerate, bitsandbytes, cuda: para mejorar rendimiento o cargar modelos grandes

### Riesgos
Datos altamente sensibles
Si el modelo se corre localmente, los datos no salen de tu máquina.
Si se usa Hugging Face o cualquier nube, debes verificar los términos de uso y protección de datos (crucial en salud).

#### ¿Usarlos localmente?
Costo: 💸 Gratis
Requisitos: una buena PC (idealmente con GPU)
Los modelos de Hugging Face no se pagan licencias.
Si el modelo es grande podria necesitar mucha RAM o una GPU

## Version 1.0 
Objetivo: Crear el modelo localmente

Paso 1: Crear entorno virtual limpio en el terminal
python -m venv venv
venv\Scripts\activate

Paso 2: Notebook para cada modelo
Modelos útiles para epicrisis
- gpt2
- BioGPT: Generación de texto biomédico
- medAlpaca: IA generativa tipo Chat en salud #requiere mucha RAM o GPU potente

Paso 3: clinical-T5


































