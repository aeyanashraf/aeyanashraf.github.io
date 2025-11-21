---
layout: page
title: PerfectPitch
description: LLM-powered mock interview + resume coach built with realtime speech, ATS feedback, and auto-coaching loops.
img: assets/img/12.jpg
importance: 1
category: work
github: https://github.com/aeyanashraf/perfectpitch
---

PerfectPitch is a full-stack interview preparation and resume-tuning platform that blends real-time speech interfaces with grounded LLM feedback. Candidates practice with voice prompts, receive structured behavioral coaching, and get ATS-style resume diagnostics without leaving the browser.

### Core capabilities
- **Realtime practice**: Assembly.ai streams speech-to-text transcripts directly into coaching prompts so Gemini can respond in seconds with follow-up questions and feedback.
- **Actionable guidance**: LangChain workflows score each answer across clarity, structure, and depth; feedback is mapped to STAR storytelling tips and concrete rewrites.
- **Resume optimization**: The same pipeline ingests a PDF resume, centralizes sections in Firebase, and runs NLP heuristics against a job description to highlight gap areas.

### Architecture notes
- Next.js + Tailwind UI for a fast SPA, with Firebase Auth/Firestore for multi-session state.
- Gemini + custom prompt templates to keep feedback grounded in job-specific competencies.
- Serverless functions orchestrate transcript batching, ATS scoring, and analytics events.

The result is a coach that feels conversational, measures improvement, and helps candidates walk into technical and behavioral interviews with evidence-backed prep.
