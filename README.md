<p align="center">
  <img src="./media/banner.webp" alt="Banner Laboratorio de Innovación"/>
</p>

# 🤖 Gloria: Agente de Resúmenes Ejecutivos

![License](https://img.shields.io/badge/license-MIT-informational)
![Contributions](https://img.shields.io/badge/contributions-welcome-success)
![Built with](https://img.shields.io/badge/built%20with-Microsoft%20Copilot%20Studio-0078D4)
![Issues](https://img.shields.io/github/issues/OWNER/REPO)
![Stars](https://img.shields.io/github/stars/OWNER/REPO)

> **Gloria** es un **agente institucional desarrollado en Copilot Studio** para apoyar la generación, validación y estructuración de **resúmenes ejecutivos** en operaciones de cooperación técnica, comités y proyectos regionales.

---

## 📹 Demo rápida (Prueba del Agente)

* **Demo en vivo**: [URL_DEMO](https://teams.microsoft.com/l/app/f6405520-7907-4464-8f6e-9889e2fb7d8f?templateInstanceId=7e1845a7-b8e1-46e4-9cac-7e653f91ef5b&environment=Default-863e38af-aa47-45c7-a525-20465c654244)

---

## 🧭 Tabla de contenidos

* [¿Qué hace Gloria?](#-qué-hace-gloria)
* [Historia y desarrollo](#-historia-y-desarrollo)
* [Arquitectura y funcionamiento](#-arquitectura-y-funcionamiento)
* [Guía de prompts](#-guía-de-prompts)
* [Despliegue en Copilot Studio](#-despliegue-en-copilot-studio)
* [Pruebas y calidad](#-pruebas-y-calidad)
* [Roadmap](#-roadmap)
* [Contribuir](#-contribuir)
* [FAQ](#-faq)
* [Licencia](#-licencia)

---

## 🧩 ¿Qué hace Gloria?

* Extrae y organiza información clave de **documentos técnicos y operativos**.  
* Genera **resúmenes ejecutivos estandarizados** con campos como país, cliente, monto, plazo, modalidad, objetivos y situación actual.  
* Facilita la revisión por parte de **comités y gerencias**.  
* Se alimenta de documentos institucionales como *PE 1631-2025*, *8. RESUMEN EJECUTIVO OIM_vf* y *PE-1170-2024*.  
* Puede integrarse con **SharePoint** para flujos de validación y almacenamiento.  

---

## 🛠️ Historia y desarrollo

* Surge como parte del proyecto de **automatización de resúmenes ejecutivos**.  
* Se apoya en documentos redactados por **Gloria Betancourt**, quien ha generado múltiples resúmenes para operaciones regionales en temas de migración, género y licitaciones.  
* Su diseño y funcionalidades fueron discutidas en reuniones como *Proyecto Agente Copilot - Revisión Resumen Ejecutivo*.  
* Está vinculado a iniciativas de cooperación técnica y validación documental.  

---

## 🧠 ¿Qué lo hace especial?

* **Estandariza** la presentación de operaciones para facilitar su aprobación.  
* Permite generar resúmenes desde **documentos PDF** cargados por el usuario.  
* Puede adaptarse a diferentes sectores: **género, migración, licitaciones, cooperación técnica**.  
* Utiliza **plantillas institucionales** y puede integrarse con flujos de **validación automática** en SharePoint.  

---

## 🛠️ Arquitectura y funcionamiento

### Vista general

flowchart LR
    U[Usuario] --> D[Documento PDF]
    D --> G[Gloria]
    G --> F[Formulario estructurado]
    F --> R[Resumen Ejecutivo]
    R --> U

Secuencia
sequenceDiagram
    participant Usuario
    participant Gloria
    participant SP as SharePoint

    Usuario->>Gloria: Carga documento técnico
    Gloria->>SP: Consulta plantilla y campos requeridos
    SP-->>Gloria: Estructura oficial
    Gloria->>Usuario: Devuelve plantilla y datos extraídos
    Gloria-->>Usuario: Genera Resumen Ejecutivo final


    Usuario->>Gloria: Carga documento técnico
    Gloria->>SP: Consulta plantilla y campos requeridos
    SP-->>Gloria: Estructura oficial
    Gloria->>Usuario: Devuelve plantilla y datos extraídos
    Gloria-->>Usuario: Genera Resumen Ejecutivo final
✍️ Guía de prompts
Rol del sistema: Agente institucional para generación de resúmenes ejecutivos.

Rol del usuario: Carga documentos técnicos o solicita resumen ejecutivo.

Restricciones:

Solo responder con los campos oficiales de la plantilla institucional.

Para detalles adicionales, consultar SharePoint.

Plantilla ejemplo de prompt utilizado:

md
Copiar código
Eres Gloria, un agente institucional para resúmenes ejecutivos.
Objetivo: generar resúmenes claros y estructurados de operaciones CAF.
Formato: campos estandarizados + descripción técnica.
Fuentes: documentos institucionales y SharePoint.
🚀 Despliegue en Copilot Studio (M365 + Teams + SharePoint)
Crea o selecciona tu agente en Copilot Studio.

Configura flujo de carga de documentos.

Integra con SharePoint para plantillas y validación.

Prueba en Test Canvas, Teams y SharePoint.

Publica en canal institucional.

✅ Pruebas y calidad
Validación de campos obligatorios: país, cliente, monto, modalidad, objetivos.

Pruebas con documentos reales: PE 1631-2025 y 8. RESUMEN EJECUTIVO OIM_vf.

Revisión manual por el equipo de Gloria Betancourt para confirmar la fidelidad de la información.

🗺️ Roadmap
 Integrar con flujos de aprobación de comités.

 Añadir validación automática de campos.

 Generar salidas en Word y PDF.

 Medir tiempo de generación y precisión.

🤝 Contribuir
Haz un fork y crea rama: feature/mi-mejora

Asegúrate que las pruebas pasan

Abre un Pull Request con descripción y ejemplos

❓ FAQ
¿Qué tipo de documentos procesa Gloria?
Documentos técnicos, operativos y de cooperación técnica.

¿Puede generar resúmenes automáticamente?
Sí, a partir de documentos PDF estructurados.

¿Dónde se guarda la información?
En SharePoint institucional y en Copilot Studio.

📄 Licencia
Este proyecto está bajo la licencia MIT. Consulta LICENSE.

Créditos
Hecho con ❤️ por Raymond Arteaga, con apoyo de Alberto Leañez, Gloria Betancourt y el equipo institucional.
