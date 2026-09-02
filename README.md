Project Goal
The goal of this project is to automate the process of retrieving data from a Wikipedia article using the Wikipedia REST API, formatting the extracted information, and writing it into a well-structured Google Document. The workflow is built using Parent and Child Workflows in n8n to demonstrate modular workflow design.

Project Workflow :
Parent Workflow
│
├── Manual Trigger
│
├── HTTP Request
│      ↓
│   Fetch Wikipedia Article
│
├── Edit Fields
│      ↓
│   Format Required Data
│
└── Execute Workflow
       ↓
Child Workflow
│
├── When Executed by Another Workflow
│
└── Google Docs (Update Document)
       ↓
Formatted Wikipedia Article

Tools Used :
n8n
Wikipedia REST API
HTTP Request Node
Edit Fields Node
Execute Workflow Node
When Executed by Another Workflow Node
Google Docs Node
Google Drive

