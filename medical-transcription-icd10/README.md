## Medical Transcription Extraction & ICD-10 Matching

### Problem
Medical transcriptions are dense, unstructured clinical notes. 
Extracting structured data manually is slow and error-prone.

### Solution
Built a two-stage LLM pipeline using OpenAI API to automatically 
extract patient age, specialty, and recommended treatment — then 
map each treatment to its ICD-10 billing code.

### Approach
- Stage 1: OpenAI function calling with custom JSON schema 
  for structured entity extraction
- Stage 2: Second LLM call maps treatments to ICD-10 codes
- Fallback handling for missing/unknown fields throughout

### Tech Stack
Python · OpenAI API · Function Calling · pandas · JSON

### Output
A clean DataFrame ready for insurance claims processing


> **📌 Note:** The patient data included in this repository (`transcriptions.csv`) 
> is entirely fictional and anonymized, created solely for the purpose of this 
> project. It does not represent or relate to any real individuals or medical records.
