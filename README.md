<p align="center">
  <img src="./media/d00f3a1f-c7e0-4a5b-943b-3bc872e4740e.webp" alt="Banner Laboratorio de Innovación"/>
  <img src="./media/GITHUB-6.png" alt="Banner Laboratorio de Innovación"/>
</p>


# 🤖 Repositorio de Agentes en Copilot Studio

![License](https://img.shields.io/badge/license-MIT-informational) 
![Contributions](https://img.shields.io/badge/contributions-welcome-success) 
![Built with](https://img.shields.io/badge/built%20with-Microsoft%20Copilot%20Studio-0078D4) 
![Issues](https://img.shields.io/github/issues/lab-innovacion-caf/Agentes) 
![Stars](https://img.shields.io/github/stars/lab-innovacion-caf/Agentes)


---

## 📌 ¿Qué es este repositorio?

Este repositorio centraliza todos los **agentes desarrollados en Microsoft Copilot Studio**.  
Cada agente vive en su **propia rama** y contiene:

- 📄 Una descripción clara de lo que hace.  
- 🔗 Un **link para probarlo directamente**.  
- 📝 Ejemplos de uso y buenas prácticas.  

👉 Si quieres **descargar un agente y editarlo en tu propio Copilot Studio**, por favor escribe a **innovacion@caf.com**. El equipo de Innovación te compartirá los archivos y la configuración necesarios.  

---

## 🧭 Cómo navegar entre los agentes

1. Abre el menú de ramas en GitHub (arriba a la izquierda, junto al botón verde “Code”).  
2. Selecciona la **rama** del agente que quieras explorar (`lya`, `agente-x`, etc.).  
3. Dentro de esa rama encontrarás:
   - Un **README específico** con su descripción.  
   - Un **enlace para probarlo** en línea.  
   - Ejemplos de preguntas y respuestas.  
   - Guías de prompts.  

💡 *Tip*: Cambia de rama para comparar diferentes agentes.  

---

## 🛠️ Arquitectura general

```mermaid
flowchart LR
    U[Usuario] --> A[Agente]
    A --> F[Flujo Copilot Studio]
    F --> C[Conectores / Acciones]
    C --> D[Fuentes de Datos]
    A --> R[Respuesta]
    R --> U
```

Hecho con ❤️ por Raymond y colaboradores de la comunidad.
