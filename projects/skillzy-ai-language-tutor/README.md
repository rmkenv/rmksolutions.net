# Skillzy – Master the AI Language

**Live App:** https://skillzy-master-the-ai-language-422293089314.us-west1.run.app

## Overview

Skillzy is an AI-powered language learning assistant that provides conversational practice and real-time feedback. Users engage in natural dialogue while the AI tutor guides them through vocabulary, grammar, and pronunciation improvements.

## Problem

Traditional language learning apps often lack personalized, conversational practice. Skillzy leverages large language models to create adaptive, context-aware tutoring sessions that respond to individual learner needs and progress.

## Approach

- **LLM Orchestration:** Designed prompt templates and conversation flows to maintain tutoring context across multi-turn dialogues
- **State Management:** Tracks user progress, vocabulary mastery, and learning goals
- **Safety & Quality:** Implemented content filtering and response validation to ensure appropriate educational content
- **User Experience:** Built intuitive chat interface with real-time feedback and progress tracking

## Tech Stack

- **Backend:** Python, FastAPI
- **AI/ML:** OpenAI API / Anthropic Claude (specify which you used)
- **Infrastructure:** Docker, GCP Cloud Run
- **Frontend:** (Specify: React, vanilla JS, or framework you used)

## Key Features

- Conversational practice in multiple languages
- Real-time grammar and vocabulary feedback
- Adaptive difficulty based on user performance
- Progress tracking and learning analytics
- Safe, educational content generation

## Architecture
User Interface
↓
FastAPI Backend
↓
LLM API (OpenAI/Anthropic)
↓
Response Processing & Validation
↓
User Feedback & State Update


## Deployment

Deployed as a containerized application on GCP Cloud Run for:
- Auto-scaling based on demand
- Cost-effective serverless architecture
- Global availability and low latency

## Future Enhancements

- Voice input/output for pronunciation practice
- Spaced repetition system for vocabulary retention
- Multi-modal learning with images and videos
- Integration with language proficiency assessments
