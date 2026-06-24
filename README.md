# AI Resume Screener

Système automatisé de présélection de CV propulsé par l'IA (LLaMA 3.3 70B via Groq) et orchestré avec n8n.

## Concept

Le recruteur uploade un CV (PDF) et décrit le poste. Le système extrait automatiquement le profil, calcule un score de matching, identifie les compétences présentes et manquantes, enregistre dans Google Sheets et envoie une notification Slack si le candidat est qualifié.

## Stack

n8n · Groq API (LLaMA 3.3 70B) · Google Sheets · Slack API

## Installation

1. Installer n8n : `npx n8n`
2. Importer `AI_Resume_Screener.json` dans n8n
3. Configurer les credentials : Groq, Google Sheets, Slack
4. Activer le workflow
