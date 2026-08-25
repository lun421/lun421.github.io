---
title: "Gen AI-Powered Interview Chatbot MVP for Technology Transformation — Internal Project in Deloitte"
date: 2026-01-30
summary: "An interview chatbot MVP using Llama 3 to extract structured insights from executive interviews in consulting."
skills: ["Generative AI Deployment", "Prompt Engineering", "Python"]
---

In technology transformation consulting, interviews with managers and executives from client companies are essential for understanding organizational context, decision processes, and operational constraints. However, these interviews are highly time-intensive and difficult to standardize. In the AI era, this project explores how interview workflows can be partially automated through the deployment of an interview-oriented chatbot, focusing on the design and implementation of a functional MVP prototype using Llama 3 opersource model.


Interview chatbot is fundamentally different from traditional customer service chatbots that handle simple transactional requests. Instead of resolving predefined intents such as refunds or service inquiries, this interview chatbot is designed to extract structured value from open-ended managerial responses. The core challenge lies in teaching the model how to evaluate the quality of an answer and determine appropriate follow-up actions based on varying response completeness and relevance.

To address this, the project defines a set of core interview questions paired with explicit evaluation criteria derived from historical consulting interviews. These past interviews, previously documented and scored by consultants during face-to-face engagements, were transformed into a structured scoring framework. An intent-and-slot architecture was then implemented to detect whether specific value points were addressed in each response, enabling rule-guided assessment and controlled conversational branching.

Beyond the initial MVP, several development directions are identified. These include incorporating historical interview records to improve contextual understanding, adding clarification mechanisms when interviewees find questions ambiguous, enabling answer revision and supplementation through a rollback mechanism, and generating consolidated analytical summaries with visual outputs. Given that interview language, focus, and expectations vary significantly across industries and client types, the system is designed to support rapid customization of question sets, terminology, and evaluation logic to fit different consulting scenarios.