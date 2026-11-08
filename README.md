# AI Study Planner and Exam Preparation Assistant

An n8n workflow that takes a student's course materials, exam date, available study hours, and selected topics, then uses AI to prepare detailed learning material and a day-by-day study plan delivered by email.

## How it works

1. The workflow is triggered by a submitted Google Sheets evaluation row containing the student's course, exam date, daily study time, requested topics, lecture files, and email address.
2. It downloads the uploaded lecture or course material.
3. A Gemini-powered AI agent prepares an extensive course explanation, examples, exam-focused points, practice questions with model answers, chapter summaries, and a daily study schedule based on the time remaining.
4. A JavaScript step converts the generated Markdown into HTML.
5. The final study material and plan are sent to the student by email.

## Technologies

- n8n
- Google Sheets
- Google Gemini
- HTTP Request
- JavaScript
- Markdown-to-HTML conversion
- Gmail

## Setup

1. Import workflow.json into n8n.
2. Configure Google Sheets, Gemini, and Gmail credentials.
3. Connect your own response sheet and ensure its column labels match the workflow expressions.
4. Use an accessible course-material link and a test email address when validating the workflow.

## Notes

This repository contains the exported n8n workflow. Configure your own credentials and integrations in n8n before running it.
