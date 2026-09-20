# AI PriorAuth Generator

## AI-Powered Prior Authorization Automation for Healthcare

AI PriorAuth Generator is an AI-assisted healthcare documentation application designed to simplify the preparation of prior authorization requests.

The application takes structured clinical and insurance information and generates a clear, structured medical-necessity justification that can be used as the basis for a prior authorization document.

The project focuses on one practical problem: **reducing repetitive documentation effort while keeping the healthcare professional in control of the final request.**

---

## 🚀 Live Demo

**Live Application:**  
http://healthcare-ai-prod.eba-kuqdyd4m.ap-south-1.elasticbeanstalk.com

The application is deployed on **AWS Elastic Beanstalk** and is publicly accessible.

> **Demo Notice:** This application is a prototype. Use only synthetic/demo patient information. Do not enter real patient information, Protected Health Information (PHI), or other sensitive healthcare data.

---

## 🎯 Problem Statement

Prior authorization is an administrative process in which healthcare providers may need to provide supporting information before a treatment, procedure, or service can be authorized by an insurance provider.

Preparing a prior authorization request can involve repeatedly:

- Reviewing patient information
- Identifying diagnosis and treatment codes
- Writing medical-necessity explanations
- Organizing clinical notes
- Preparing supporting documentation
- Formatting the request

For healthcare providers and administrative teams, this can become a repetitive documentation task.

### The problem we address

> **How can AI assist healthcare teams in transforming structured clinical information into a consistent prior authorization justification?**

Instead of attempting to solve the entire healthcare authorization process, this project focuses on one specific and practical part of the workflow: **documentation generation.**

---

# 💡 Our Solution

AI PriorAuth Generator provides a simple web interface where users enter the information required to prepare a prior authorization request.

The application accepts information such as:

- Patient name
- Date of birth
- ICD-10 diagnosis code
- Diagnosis
- CPT/treatment code
- Treatment or procedure
- Clinical notes
- Provider information
- Insurance information

The application then uses an LLM to generate an AI-assisted medical-necessity justification based on the information provided.

### Workflow

```text
Clinical Information
        │
        ▼
   Web Interface
        │
        ▼
    FastAPI API
        │
        ▼
   LLM Generation
        │
        ▼
Medical Necessity
   Justification
        │
        ▼
Authorization Document
