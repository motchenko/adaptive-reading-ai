# AI-Assisted Adaptive Reading & Language Learning System

## Overview
This project is an independent AI system designed to support language learning by adapting texts to different learner proficiency levels.  
The system modifies input texts, generates contextual explanations, and produces structured learning-oriented outputs.

## Core Functionality
The system supports:
- Adaptive text modification based on learner level
- Contextual explanation generation
- Structured output tailored for language learning use cases

## System Design
The system is implemented as a modular backend with the following components:
1. Input handling and prompt construction
2. Retrieval-augmented generation (RAG)
3. Adaptive text generation with complexity control

## Retrieval-Augmented Generation (RAG)
The system implements a retrieval-augmented generation (RAG) pipeline that grounds explanations in curated linguistic resources, including vocabulary lists and reference materials.

Retrieved context is incorporated into prompt construction to improve factual grounding and reduce hallucination in generated explanations.

## Text Complexity Control
The system implements text complexity control mechanisms using:
- Readability metrics
- Vocabulary-level constraints

These controls are used to adapt generated content for different learner proficiency levels, including across multiple languages.

## Implementation
- Implemented as a serverless backend using JavaScript (Cloudflare Workers)
- Exposes an HTTP API for adaptive content generation
- Integrates the OpenAI API for generation
- Supports local development and deployed execution

## Languages
The system has been tested with text inputs in English and Chinese as part of ongoing development.

## Limitations
- Complexity control is heuristic and may not fully capture semantic difficulty
- Generated explanations may still hallucinate in edge cases
- Evaluation is ongoing and not yet large-scale
