# AI Study Planner

I built this n8n workflow to help students prepare for exams using their course materials, exam date, available study hours, and the topics they need to study. It generates detailed study material and a personalized study plan that is sent by email.

<img width="608" height="207" alt="image" src="https://github.com/user-attachments/assets/376cac4c-00c2-4d3a-a039-fcea1bf170b0" />

## How it works

1. The student submits the course name, exam date, available daily study hours, requested topics, course material link, and email address through the connected form.
2. The workflow downloads the uploaded lecture or course material.
3. Google Gemini analyzes the material and prepares explanations, practical examples, important exam points, practice questions with answers, and chapter summaries.
4. The AI creates a day-by-day study schedule based on the time remaining until the exam and the student's available study hours.
5. The workflow converts the result into HTML and sends the study plan by email.

## Main features

- Course material and lecture file processing.
- Study plan based on the exam date.
- Personalized daily schedule.
- Detailed explanations and practical examples.
- Practice questions with model answers.
- HTML-formatted email delivery.

## Technologies

n8n, Google Sheets, Google Gemini, HTTP Request, JavaScript, HTML, and Gmail.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Google Sheets, Gemini, and Gmail credentials, then connect your form response sheet and test the workflow with a sample course file and exam date.
