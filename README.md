# AI interior design

A web service for generating interior design concepts from natural-language descriptions using an LLM and a text-to-image model.

## Live app

Link to the deployed app: https://ai-interior-design-mvp-production.up.railway.app/

## Team

Team 16
- Вакулич Анастасия Андреевна
- Рощина Надежда Романовна

## Project Overview

AI Interior Design helps users turn vague interior ideas into visual concepts.

The current MVP focuses on a simple flow:

**text description + reqired parameters → enhanced prompt → generated interior image**

The system is designed to be easier to use than professional interior design tools and more controllable than basic text-to-image generation.

## MVP Features

- free-text interior description
- reqired structured parameters
  - style
  - room size
  - lighting
- LLM-based prompt enhancement
- AI-generated interior image
- simple web interface

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Python
- **LLM:** GigaChat
- **Image generation:** Yandex ART
- **Deployment:** Railway

## Repository Structure

- [`main.py`](main.py) — main application code
- [`yandex_utils.py`](yandex_utils.py), [`gigachat_utils.py`](gigachat_utils.py) — API helper functions
- [`templates/index.md`](templates/index.md), [`templates/index_v2.md`](templates/index_v2.md), [`templates/index_v3.md`](templates/index_v3.md) — frontend layouts

## Documentation

Project details are available in the following files:

- [`DOCS/MARKET_REVIEW.md`](DOCS/MARKET_REVIEW.md) — analysis of existing solutions on the market
- [`DOCS/USER_STORY_ANALYSIS.md`](DOCS/USER_STORY_ANALYSIS.md) — target audience user story analysis
- [`DOCS/SOLUTION_ARCHITECTURE.md`](DOCS/SOLUTION_ARCHITECTURE.md) — technical project description
- [`DOCS/CUSTOMER_SURVEY.md`](DOCS/CUSTOMER_SURVEY.md) — results of customer survey on a small focus group

## Current Limitations

The MVP does not yet include:

- exact room planning with real dimensions
- renovation estimates or engineering calculations
- product recommendations with real store links
- photo-based room redesign

## Future Work

Possible next steps:

- generate multiple design concepts per request
- create a structured design brief
- support iterative refinement
- add photo upload
- integrate product selection from stores/marketplaces

## Key Value

The project aims to solve a common problem in interior AI tools:

**better control without losing simplicity**
