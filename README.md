# Stable-Diffusion-16371669
AI Animal Care & Pet Health Visualization System

GenAI: Controlled Image Generation with Stable Diffusion

# Title: Health Paws Viz
Author: Prathyu Adari

ID: 16371669

## Overview
This project implements a data-driven, controlled image generation system using Stable Diffusion. It takes structured input (animal type, breed, condition, environment) and generates responsible, high-quality educational visualizations for veterinary scenarios.

## Dataset & Scenario
* **Domain**: Veterinary Care & Animal Welfare.
* **Reference Context**: Inspired by datasets like the Oxford-IIIT Pet Dataset and Stanford Dogs Dataset for breed accuracy.

## Methodology & Pipeline
1.  **Framework**: Python, PyTorch, Hugging Face `diffusers`.
2.  **Model**: Stable Diffusion v1.5.
3.  **Data-to-Prompt Mapping**: Converts JSON/Dict structures into precise prompt templates.
4.  **Control Mechanism**: Utilizes strict positive prompt templating (focusing on clinical accuracy and compassionate tone) and robust **Negative Prompts** to prevent anatomical deformations and inappropriate content.

## How to Run
1. Install dependencies: `pip install diffusers transformers accelerate torch pillow`
2. Run the pipeline: `python main.py`
3. Check the `/output_images` directory for baseline vs. improved comparisons.

## Evaluation & Metrics
* **Prompt Alignment**: Does the image contain the correct breed and condition?
* **Consistency**: Do negative prompts successfully remove artifacts?
* **Visual Quality**: Measured by the realism and lighting of the output.

## Ethics & Transparency
* **Ethical Guardrails**: All outputs are automatically watermarked with "AI-Generated Illustration for Educational Purposes". The negative prompt strictly forbids blood or graphic injuries.
* **AI Tools Disclosure**: 
    * *GitHub Copilot*: Used for boilerplate code generation.
    * *Gemini*: Used for structuring the pipeline architecture, refining the prompt engineering templates, and formatting documentation.

# Demo Video
Link: https://umsystem.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=578c75da-4390-4a3b-886a-b433003e7d60
