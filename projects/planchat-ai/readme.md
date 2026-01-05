# PlanChat AI – Engineering Blueprint Analytics & Chat Hub

**Live App:** https://planchat-ai-278412187073.us-west1.run.app  

---

## Overview

PlanChat AI is a specialized decision-support platform for construction, architecture, and engineering (AEC) professionals. It transforms static technical drawings into interactive data sources, allowing users to “converse” with complex blueprint sets to retrieve dimensions, specifications, and code compliance details instantly.

## Problem

AEC professionals spend significant portions of their workweek hunting for specific details across hundreds of pages of as-built drawings. This manual process is prone to human error, leads to costly site delays, and often results in missed cross-references between different engineering disciplines (e.g., structural vs. electrical). PlanChat AI addresses this by turning drawing sets into a searchable, conversational interface.

## Data

- **Sources:**
  - User-uploaded technical plan sets
  - Architectural PDFs
  - As-built records
  - CAD exports (converted to document/image formats)

- **Formats:**
  - Multi-page PDF document sets
  - High-resolution imagery (PNG, JPG)
  - Engineering-standard TIF/TIFF files

- **Contextual Variables:**
  - Geometric dimensions and annotations
  - Title block metadata
  - Visual symbols (legend keys)
  - Text-based specifications and notes

## Approach

### Analytics

- **Multimodal Processing:** Utilizes Gemini 2.5 Flash to simultaneously interpret visual spatial data (line work) and technical text.
- **Interactive Citation Mapping:** Automatically maps AI-generated answers back to specific sheet names with clickable links for immediate human verification.
- **Transient Memory Model:** Implements a high-security architecture where drawing data is processed in browser RAM and encrypted in transit, ensuring sensitive project files are never stored on the app’s servers.

### Conversational Logic

- **RAG (Retrieval-Augmented Generation):** Merges long-context window capabilities with user-uploaded document parts for grounded, context-aware responses.
- **Professional Rigor:** System prompts are engineered to mimic the mindset and vocabulary of a US Professional Engineer (PE), emphasizing conservative, standards-aligned reasoning and explicit references to source sheets.

## Tech Stack

- **Frontend:** React (v19), Tailwind CSS, PDF.js (for high-fidelity plan rendering)
- **Intelligence:** Google Gemini API (Gemini 2.5 Flash model)
- **Backend / Auth:** Supabase (PostgreSQL for chat persistence, Auth for user management)
- **Deployment:** ES6 module–based static hosting with dynamic API integration

## Key Features

- **Multimodal Chat:** Ask technical questions about visual details on blueprints (e.g., clear height, beam size, conduit routing) using natural language.
- **Sheet Citations:** Every response includes `[[Citation:SheetName]]` tags that sync with the built-in PDF viewer for one-click verification.
- **Official Report Generation:** Exportable plain-text transcripts formatted for professional record-keeping and project documentation.
- **Tiered Usage System:** Persistent monthly usage tracking (e.g., 5 free messages/month) with a **Bring Your Own Key (BYOK)** option for unlimited professional use.

## Results

- **Efficiency:** Reduces information retrieval time from minutes to seconds, especially for repetitive RFIs and detail lookups.
- **Accuracy:** Promotes a “verify-first” culture via integrated document citations and explicit linkage back to original drawings.
- **Accessibility:** Centralizes project knowledge, allowing non-CAD users to understand complex engineering documents via conversation instead of tooling.

---

[← Back to Portfolio](../../README.md)
