# Wikipedia to Google Docs Automation

## Project Overview

This project automates the process of retrieving information from a Wikipedia article and writing the extracted content into a structured Google Document.

The workflow is built using **n8n Parent and Child Workflows**. The Parent Workflow retrieves and formats the required Wikipedia data, then passes the information to the Child Workflow. The Child Workflow receives the data and updates a Google Document.

This project demonstrates **API integration, data transformation, workflow modularity, and automated document generation** using n8n.

## Project Workflow

### Parent Workflow

Manual Trigger
↓
HTTP Request
↓
Fetch Wikipedia Article
↓
Edit Fields
↓
Format Required Data
↓
Execute Workflow
↓
Child Workflow

### Child Workflow

When Executed by Another Workflow
↓
Google Docs
↓
Update Document
↓
Formatted Wikipedia Article

## Tools & Technologies

* **n8n** – Workflow automation platform
* **Wikipedia REST API** – Retrieves Wikipedia article data
* **HTTP Request Node** – Sends API requests
* **Edit Fields Node** – Extracts and formats required data
* **Execute Workflow Node** – Connects the Parent and Child Workflows
* **When Executed by Another Workflow Node** – Receives data from the Parent Workflow
* **Google Docs** – Creates and updates the document
* **Google Drive** – Stores the generated Google Document

## Key Features

* Retrieves Wikipedia article data automatically using the REST API
* Extracts and formats the required information
* Uses Parent and Child Workflows for modular automation
* Passes data between workflows using n8n
* Automatically updates a Google Document
* Reduces manual copy-paste work
* Demonstrates API-based workflow automation


