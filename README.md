# Multi-Agent Content Writing System using Crew AI with Local LLM

This project leverages Crew AI and a locally running Large Language Model (LLM) to create a multi-agent system specifically designed for content writing. The system is composed of multiple agents, each with distinct roles and responsibilities to assist in generating high-quality content efficiently.


## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [System Requirements](#system-requirements)
- [Installation](#installation)


## Overview

This project creates an intelligent content writing system by using Crew AI for agent orchestration and a local LLM for text generation. The system is designed to automate various aspects of content creation, from idea generation to final drafts, with each agent focusing on different aspects of the writing process.

## Key Features:

- **Multi-Agent Framework**: A group of specialized agents to collaborate and generate content.
- **Local LLM**: An advanced LLM running locally to ensure privacy and fast generation.
- **Content Creation Workflow**: Agents that handle tasks such as research, drafting, editing, and proofreading.
- **Customizable Roles**: Ability to add or modify agent roles to suit specific needs.

## System Requirements

Before you begin, ensure that your system meets the following requirements:

- **Python 3.8+** (Recommended version: 3.9 or higher)
- **A locally hosted LLM**

---


## Installation

**Follow these steps to set up the multi-agent system on your local machine.**

**Clone the Repository:**

```bash
git clone https://github.com/Afssal/crew_ai.git
cd crew_ai
```

Install Dependencies: Set up a Python virtual environment and install required dependencies:

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt


Install Local LLM: 

install ollama framework

for more details follow this link : https://ollama.com/

then copy your model name in given code 


```bash
llm = LLM(
    model = 'ollama/{your ollama model}',
    base_url = "http://localhost:11434"
)
```

Run the Agents: Start the multi-agent system:
```bash
streamlit run content_writer.py
```
