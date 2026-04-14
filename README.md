# AI-Job-Application-Intelligence-Agent
Built a full end-to-end AI-powered job application tracker that automatically analyzes job postings, scores resume fit, and logs structured entries into a Notion database with zero manual input.

How it works:
• Paste a job URL into a form trigger
• n8n orchestrates the entire pipeline
• Claude AI (Anthropic) extracts role, company, seniority level, and required skills from the posting
• A second Claude call compares job requirements against my resume and generates a match score (out of 10) and a plain-English fit summary
• Composio writes a fully structured entry into a Notion job tracker database automatically

Each Notion entry includes:
— Company & Role
— Match Score (out of 10)
— Skills Gap analysis
— Application Status
— Follow-up Date
— AI-generated Fit Summary

Tech Stack: n8n · Claude AI (Anthropic) · Composio · Notion API
