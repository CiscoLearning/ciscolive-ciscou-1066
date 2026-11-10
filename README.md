# ciscolive-ciscou-1066

**5 Ways to Leverage AI to Successfully Pass your Certification Exam**

This repository contains the companion prompts for Cisco Live session **CiscoU-1066**. Each prompt is written using the **SCOPE** framework (Situation, Character, Outcome, Purpose, Example) and is designed to help certification candidates use AI as a study aid throughout their exam preparation journey.

## Prompts

The [`prompts/`](./prompts) folder contains five ready-to-use prompts, each targeting a different stage of exam prep:

| # | Prompt | Use it to... |
|---|--------|--------------|
| 1 | [AI as your Blueprint Decoder](./prompts/AI%20as%20your%20Blueprint%20Decoder.md) | Break down the official exam blueprint into a prioritized, plain-language study roadmap. |
| 2 | [AI as Your Study Scheduler](./prompts/AI%20as%20Your%20Study%20Scheduler.md) | Build a realistic week-by-week study plan based on your exam date and available hours. |
| 3 | [AI as Your Study Partner](./prompts/AI%20as%20Your%20Study%20Partner.md) | Turn passive reading material into flashcards, mnemonics, and comparison tables. |
| 4 | [AI as your Lab Architect](./prompts/AI%20as%20your%20Lab%20Architect.md) | Generate hands-on practice labs in Cisco Modeling Labs (CML). |
| 5 | [AI as your Exam Simulator](./prompts/AI%20as%20your%20Exam%20Simulator.md) | Generate targeted, exam-style practice questions focused on your weakest domains. |

## How to use

1. Open the prompt that matches the stage of your study journey.
2. Copy the prompt text into your AI assistant of choice.
3. Replace the `{placeholders}` (e.g., `{exam_name}`, `{x_hours}`) with your own details and attach or paste the relevant study content (blueprint, notes, etc.).
4. Iterate on the AI's response — refine, re-prompt, and use the output as an active study tool rather than passive reading.

## Fill the placeholders automatically

Every `{placeholder}` in the prompts matches a key in [`values.json`](./values.json), which comes pre-filled for **CCNA Automation (200-901 CCNAAUTO v1.1)**. To study for a different exam, change `exam_name`, `blueprint_url`, `domains`, and the lab values.

To use it in a Claude Project (or any assistant that supports project files and instructions):

1. Edit `values.json` with your exam date, study hours, study material, and weakest topics. Leave a value as `""` and the assistant will ask for it.
2. Upload `values.json` and the files in `prompts/` as project files.
3. Paste this into the project instructions:

   > When I say "Run [prompt name]" (for example "Run Study Scheduler" or "Run Learning Tracker"), take that prompt from the prompt files, replace every `{placeholder}` with the matching value from values.json, and ask me for any value that is empty. If I give a value in my message, use mine for this run. Show me the filled-in prompt, then carry it out. After a Learning Tracker run, tell me which values in values.json to update.

4. Type **"Run Study Scheduler"**. After each study session, type **"Run Learning Tracker"**, then update `values.json` and re-upload it.

## Session

Presented at **Cisco Live** as session **CiscoU-1066 — 5 Ways to Leverage AI to Successfully Pass your Certification Exam**.
