# Literature Review and Existing Solutions

## 1. Introduction

In recent years, generative AI systems for interior design have developed rapidly. These tools help automate the creation of visual room concepts and make design more accessible to users without professional experience.

Modern solutions often combine:

- large language models (LLMs)
- image generation models (diffusion models)
- 3D visualization and AR/VR tools

AI systems for interior design can generate concepts, style variations, and visualizations from text or images, speeding up both design and decision-making.

## 2. Categories of Existing Solutions

### 2.1 Text-to-Image Generation

This category includes models that create interior images from text descriptions:

- Midjourney
- DALL·E
- Stable Diffusion

These systems allow users to describe an interior in words and receive a visual result. They are especially useful for idea generation and early concepts.

**Strengths:**

- high visual realism
- flexible text-based control
- strong support for creative exploration

**Weaknesses:**

- difficult to control results precisely
- dependent on prompt quality
- requires prompt engineering skills
- lacks structured input

In general, Midjourney is better at conveying atmosphere and style, while DALL·E tends to follow precise instructions more accurately.

### 2.2 AI Platforms for Interior Design

This category includes more comprehensive platforms:

- Planner 5D
- Homestyler
- Roomstyler
- Foyr Neo

These tools allow users to:

- create floor plans
- arrange furniture
- work with 3D visualizations

For example, Planner 5D uses AI for automatic furniture placement and realistic interior generation.

**Strengths:**

- high accuracy
- support for real dimensions
- 3D visualization

**Weaknesses:**

- complex interfaces
- often excessive for casual users
- requires manual adjustment
- can be expensive

### 2.3 Image-to-Image Interior Design

A separate category focuses on redesigning interiors from photos:

- RoomGPT
- ReimagineHome
- IA Decora

**How it works:**

- the user uploads a room photo
- the system generates redesign options

For example, RoomGPT can produce several design variations from a single image.

**Strengths:**

- high personalization
- easy to use

**Weaknesses:**

- limited control
- somewhat template-based outputs
- weak detail accuracy

## 3. Research Trends

Academic research actively explores AI-based interior generation.

Main directions include:

- **Text- and image-based generation**  
  Combining textual and visual input improves result accuracy and consistency.  
  Example: **VIDES** generates interiors using both text and visual cues.

- **Layout optimization**  
  LLMs can help generate room structure and optimize furniture placement by extracting constraints.

- **Interactive systems**  
  Users interact with the model during generation.  
  Example: **Chat2Layout** enables furniture arrangement through dialogue.

- **Controllable generation**  
  Research aims to improve control over diffusion models.  
  Example: **DiffDesign** introduces control over style, size, and composition.

## 4. Limitations of Existing Solutions

Despite recent progress, most current solutions still have common limitations:

- difficult result control
- dependence on text prompt quality
- lack of structured parameters
- limited personalization
- sometimes unrealistic or repetitive outputs

A common issue is the lack of balance between ease of use and precise control.

## 5. Conclusions and Project Positioning

The analysis shows that:

- image generators produce attractive results but are hard to control
- professional tools are accurate but complex
- photo-based solutions are convenient but limited

This creates an opportunity for a solution that combines a simple interface with structured parameter control, uses LLMs to improve prompts, and generates realistic images.

## 6. How Our Solution Differs

The MVP being developed takes a middle position: it is simpler than professional design tools and more controllable than pure text-to-image models.

**Key features:**

- LLM-based prompt generation
- structured parameters such as style, size, and lighting
- a simple user interface

As a result, the project addresses one of the main weaknesses of existing solutions: limited controllability while keeping the system easy to use.