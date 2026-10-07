
## 1. Estructura de Carpetas del Repositorio

Puedes organizar tus archivos en GitHub de la siguiente manera:

```text
ari-news-opal-ai/
├── README.md
├── docs/
│   ├── pipeline-diagram.png        (Captura del pipeline visual en Opal)
│   └── dashboard-preview.png       (Captura de la página generada)
└── prompts/
    ├── 01_buscador_noticias.txt    (Prompt del agente de búsqueda)
    ├── 02_validador_links.txt      (Prompt del agente de validación)
    ├── 03_generador_imagen.txt     (Prompt del agente visual)
    └── 04_renderizador_html.txt    (Prompt de la interfaz/dashboard HTML)

```

# 🤖 ARI News — Dashboard de Inteligencia Estratégica con Agentes de IA

![Google Opal](https://img.shields.io/badge/Platform-Google%20Opal-blue?style=for-the-badge)
![Alura Latam](https://img.shields.io/badge/Course-Alura%20Imers%C3%A3o-orange?style=for-the-badge)
![No Code](https://img.shields.io/badge/Build-No--Code-green?style=for-the-badge)

**ARI News** es un pipeline automatizado de agentes de Inteligencia Artificial que rastrea noticias reales en la web, valida sus enlaces de origen, genera representaciones visuales conceptuales y renderiza un dashboard HTML profesional listo para la toma de decisiones estratégicas.

Proyecto construido durante la **Inmersión Agentes de IA para Negocios** de **Alura Latam**, utilizando **Google Opal**.

🔗 **Ver Aplicación en Google Opal:** [ARI News en Opal](https://opal.google/app/1fkby8tWfZsMY2PEpWPJ7hkf_SL8I-UJf)

---

## 🎯 Objetivos del Proyecto

- **Pipelines de IA vs. Chatbots tradicionales:** Superar la interacción básica por texto creando una secuencia de agentes especializados que colaboran secuencialmente y en paralelo.
- **Grounding Temporal:** Garantizar información actualizada filtrando noticias por sector, región y marco temporal.
- **Prevención de Alucinaciones:** Implementar un nodo de validación de URLs para asegurar que todos los enlaces entregados sean reales y accesibles.
- **Generación Visual & HTML:** Producir imágenes conceptuales abstractas y un panel web en HTML/CSS estructurado sin escribir código manual.

---

## 🧠 Arquitectura del Pipeline de Agentes

El flujo de trabajo en Google Opal se compone de los siguientes agentes:


```

[Entradas de Usuario]
(Sector, Región, Fecha, Nº Noticias)
│
▼
┌───────────────────────────┐
│  Agente 1: Búsqueda Web   │ ──► Filtra y extrae noticias reales
└─────────┬─────────────────┘
│
▼
┌───────────────────────────┐
│  Agente 2: Validador URLs │ ──► Elimina alucinaciones de links
└─────────┬─────────────────┘
│
├────────────────────────────────┐
▼                                ▼
┌───────────────────────────┐    ┌───────────────────────────┐
│ Agente 3: Arte & Branding │    │  Agente 4: Renderizador   │
│   (Prompt de Imagen)      │    │         HTML/CSS          │
└─────────┬─────────────────┘    └─────────┬─────────────────┘
│                                │
└────────────────────────────────┘
│
▼
[ Dashboard Final ARI News ]

```

### Funciones de cada agente:
1. **Agente de Búsqueda de Noticias:** Recibe las variables de entrada (`Sector`, `Región`, `Fecha_noticias`, `Número_noticias`) y recupera la información más reciente.
2. **Agente Validador de Links:** Verifica que las URLs extraídas existan y correspondan exactamente a la fuente de la noticia.
3. **Agente de Generación Visual:** Diseña un arte conceptual abstracto representativo del sector sin texto impreso.
4. **Agente de Interfaz HTML:** Ensambla las noticias, la imagen y la paleta de colores en un dashboard web estilizado y funcional.

---

## 🎨 Paleta de Colores & Diseño

El dashboard utiliza la siguiente identidad visual para mantener un tono corporativo y elegante:

- **Fondo Bloques Principales / Impares:** Blanco Puro (`#FFFFFF`)
- **Fondo Bloques Secundarios / Pares:** Gris Suave (`#F9F9F9`)
- **Tipografía Principal:** Negro Charcoal (`#0D0D0D`)
- **Metadatos e Índices (`01 / 03`):** Gris Mate (`#555555`)
- **Color de Acento / Interacción:** Azul Cobalto (`#2738F5`)

---

## 🛠️ Variables de Entrada Utilizadas

- **`Sector`**: Área de negocio o industria a monitorear (Ej. *Educación Tecnológica, Finanzas, IA*).
- **`Región`**: Ubicación geográfica de las noticias (Ej. *Latinoamérica, Global*).
- **`Fecha_noticias`**: Rango temporal solicitado.
- **`Número_noticias`**: Cantidad dinámica de artículos a listar en el panel.
- **`Sector_o_Tema`**: Tema específico para la imagen de cabecera.
- **`Color_de_Acento`**: Tono secundario para la composición visual.
- **`Efecto_Visual`**: Estilo abstracto de la imagen (Ej. *caminos de luz interconectados*).

---

## 📚 Créditos y Agradecimientos

- **Evento:** Inmersión Agentes de IA para Negocios — Clase 1
- **Organización:** [Alura Cursos](https://www.aluracursos.com/)
- **Herramienta:** [Google Opal](https://opal.google/)

```

---
