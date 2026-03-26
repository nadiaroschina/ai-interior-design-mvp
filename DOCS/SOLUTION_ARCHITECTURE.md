# Universal MVP Description

## 1. MVP Overview

The MVP is a web-based interior image generation service. It allows users to describe a desired interior in natural language and optionally refine the request with structured parameters. The system then uses an LLM to create an optimized English prompt and sends it to an image generation model to produce a visual concept.

## 2. Core Functionality

The MVP supports the following flow:

- the user enters a free-form text description of the desired interior
- the user can optionally select additional parameters:
  - **interior style**
  - **room size**
  - **lighting type**
- the system sends the input to an LLM
- the LLM transforms the input into a detailed English prompt optimized for image generation
- the enhanced prompt is sent to a Text-to-Image API
- the generated image is returned and displayed in the interface
- optionally, the interface also shows the original request and the enhanced prompt for transparency

### Example user input
> “Scandinavian-style bedroom with a large bed, panoramic window, cozy atmosphere”

## 3. System Architecture

The solution consists of three main components:

### Frontend
A simple web interface built with HTML, CSS, and JavaScript that:

- collects the user’s text input
- allows selection of structured parameters
- sends the request to the backend
- displays loading status, the enhanced prompt, and the final image
- allows for interface language selection

### Backend
A Python server that:

- receives requests from the frontend
- combines free text and selected parameters into a structured input
- calls the LLM API
- sends the enhanced prompt to the image generation API
- returns the final result as JSON

### External APIs

- **LLM API**  
  Used to improve and structure the user request into an English image-generation prompt  
  Examples: Yandex GPT, GigaChat

- **Text-to-Image API**  
  Used to generate the final interior image from the enhanced prompt  
  Examples: Kandinsky 3.0, Replicate SDXL

## 4. Input Parameters

The system accepts both unstructured and structured input.

### Free-text input
The user describes the desired interior in natural language.

### Structured parameters
The user can also choose:

- **Style** — e.g. Scandinavian, Minimalist, Loft, Modern, Japandi, Provence
- **Room size** — Small, Medium, Large, Open Space
- **Lighting** — Daylight, White Light, Warm Side Light, Warm Evening Light, Accent Light

These parameters improve control and make the generated result closer to user expectations.

## 5. Request Processing Logic

Originally, the system sent only the raw user text to the LLM. In the updated MVP, the request includes both the text and the selected UI parameters.

The backend accepts the following fields:

- `text`
- `style`
- `room_size`
- `lighting`

Using these values, it creates a more structured input for the LLM. This makes the final prompt more specific, consistent, and controllable.

## 6. User Flow

The full user scenario is:

1. The user opens the web page.
2. The user enters a text description of the interior.
3. The user optionally selects style, room size, and lighting.
4. The user clicks **Generate**.
5. The frontend sends all data to the backend.
6. The backend prepares a structured request for the LLM.
7. The LLM generates a detailed English prompt.
8. The backend sends that prompt to the image generation model.
9. The image API returns the generated result.
10. The frontend displays the image, and optionally the original and enhanced prompts.

## 7. Frontend Features

The frontend includes the following improvements:

- parameter selection blocks for style, room size, and lighting
- consistent visual design across the page
- updated JavaScript request handling
- transfer of both text and structured parameters in JSON
- temporary disabling of the generate button while processing
- loading indicator during generation
- display of the enhanced prompt and final image

## 8. Example Request

```json
{
  "text": "Scandinavian-style bedroom with a panoramic window",
  "style": "Scandinavian style",
  "room_size": "Medium room with balanced proportions",
  "lighting": "Soft natural daylight"
}
```

## 9. Example Response

```json
{
  "original": "Scandinavian-style bedroom with a panoramic window",
  "enhanced_prompt": "A bright Scandinavian-style bedroom with a large cozy bed, panoramic window, soft natural daylight, wooden floors, white walls, minimalist decor, hygge atmosphere, ultra realistic, 8k",
  "image_url": "https://..."
}
```

## 10. Result

This MVP provides a simple but controllable way to generate interior concepts. It combines:

- natural language input
- structured parameter selection
- LLM-based prompt enhancement
- AI image generation

As a result, the system is easier to use than professional design software and more controllable than basic text-to-image tools.