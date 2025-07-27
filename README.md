# Resume-AI-Agent
Overview
Objective was to design and build a Resume Refiner AI Agent using n8n that tailors a user-submitted resume to a job posting and emails suggested edits back to the user. The goal is to create an AI Agent pipeline that automates job application personalization. 

AI Agent Flow diagram
<img width="975" height="485" alt="image" src="https://github.com/user-attachments/assets/0f631dfd-38eb-43cb-af02-938ba3a2a5fd" />

Building the Agent

What approach did you take to design your agent? First I did a rough map in draw.io of how I think the workflow should look to use as a guide for my workflow in n8n. I worked on each individual node step by step and tested prior to moving to another node and when trying to find ways to personalize it from the instructions given I leveraged the AI assistant tool to rename the first node and second node as well as using a URL expression in the HTTP request node to bypass having an extra step extracting the file node. 

What challenges did you face in parsing, formatting, or integrating? 

The primary challenge I had was not being able to test properly the AI Agent node going forward due to expired tokens. This affected by ability to full integrate all nodes working properly in the workflow.

How did you ensure that the AI returned JSON reliably? 

I would test the output function and make sure it returned successfully.

Troubleshooting

What issues did you encounter and how did you resolve them? 

Formatting the output resume corrections in an easy to read version for the email was a challenge and I leveraged Co-pilot with this prompt to help " I am working in n8n creating an Ai Agent flow. I was able to get the AI to output resume corrections, however I want to format this output so that it is easy to read in an email. Can you create a JSON schema for my output please?"  Also, not being able to test the full workflow past the AI agent node was a blocker but I proceded to just map out what the rest of the flow would look like for full transparency

Optimization

What might you improve or add in future iterations?

I would add in a percentage rating as part of the suggestions to let users know how strong of a candidate they would be for the role once the suggestions are implemented to encourage users to follow through. Also maybe some kind of celebratory effect when the form is submitted with confettti to make the feel user feel good about their decision to use the tool and encourage more adoption in the future.
