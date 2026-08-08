Sistema Inteligente de Triaje Médico Operativo 🏥🤖
Asignatura: Tecnologías de la Inteligencia Artificial (INF-4350)  
Institución: Universidad Federico Henríquez y Carvajal (UFHEC)  
Profesor: Luis Fortuna  
Estudiante: Oliver Alexander Lantigua Alberto  
Matrícula: SD-19-30423
---
📌 Descripción del Proyecto
Este prototipo es una solución en C# (.NET) integrada con la plataforma de IA Local Ollama para la clasificación automatizada de urgencias médicas en áreas de atención inicial (triaje).
El sistema utiliza técnicas de Prompt Engineering —específicamente Chain-of-Thought (Cadena de Pensamiento)— para garantizar un análisis estructurado de los síntomas del paciente, determinando:
Nivel de Urgencia: ROJO (Prioridad Alta), AMARILLO (Prioridad Media), VERDE (Prioridad Baja).
Especialidad Médica Sugerida.
Justificación Clínica Breve.
Al ejecutarse localmente, garantiza 100% de privacidad de datos de salud (HIPAA-friendly) y funcionamiento offline.
---
🛠️ Requisitos del Sistema
Antes de ejecutar la aplicación, asegúrate de contar con los siguientes elementos instalados en tu equipo:
.NET SDK 8.0 (o posterior): Descargar .NET SDK
Ollama: Descargar Ollama
Modelo de Lenguaje (Llama 3 o similar):
Abre una terminal/PowerShell y ejecuta:
```bash
   ollama pull llama3
   ```
---
🚀 Pasos para Ejecutar el Proyecto
1. Iniciar el Servicio de Ollama
Asegúrate de que Ollama esté ejecutándose en tu sistema. Puedes verificar abriendo tu navegador y visitando:
```text
http://localhost:11434
```
Debe mostrar el mensaje: "Ollama is running".
Si no está corriendo, abre una terminal y ejecuta:
```bash
ollama serve
```
2. Clonar o Descargar el Repositorio
```bash
git clone https://github.com/TU_USUARIO/TriajeMedicoOllama.git
cd TriajeMedicoOllama
```
3. Compilar y Ejecutar la Aplicación C#
Abre la terminal en la carpeta raíz del proyecto y ejecuta:
```bash
dotnet run
```
---
🧪 Casos de Prueba Recomendados
Nivel de Urgencia	Síntomas de Entrada
🟢 VERDE (Baja)	"Tengo 3 días con un ojo rojo que me pica y secreción amarillenta en las mañanas, sin dolor grave."
🟡 AMARILLO (Media)	"Dolor punzante en la parte inferior derecha del abdomen desde anoche, náuseas y fiebre leve de 38 °C."
🔴 ROJO (Alta)	"Opresión fuerte en el centro del pecho que se extiende al brazo izquierdo y mandíbula, dificultad para respirar y sudor frío."
---
🛡️ Consideraciones Éticas (Human-in-the-Loop)
Este software es una herramienta de soporte asistencial para personal administrativo y sanitario. No emite diagnósticos médicos definitivos ni sustituye el juicio de un profesional de la salud calificado.
