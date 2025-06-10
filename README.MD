# Multi-Agent AI Software Development System

## What This Project Does

This project demonstrates an innovative **multi-agent AI system** that simulates a complete software development team using artificial intelligence. Think of it as having three AI specialists working together to build software applications - just like a real development team, but powered by AI!

The system creates a **simple calculator web application** through collaboration between three specialized AI agents:
- **Program Manager AI**: Plans and organizes the project
- **Software Engineer AI**: Writes the actual code
- **Project Manager AI**: Reviews and approves the final product

## Understanding the AI Agents

### 🎯 Program Manager Agent
**What it does**: Acts like a project leader who understands what you want and creates a detailed plan.
- Takes your requirements (like "I want a calculator app")
- Creates detailed project documentation
- Estimates costs and timelines
- Breaks down complex requests into manageable tasks

### 💻 Software Engineer Agent  
**What it does**: Acts like a programmer who builds the actual application.
- Receives the plan from the Program Manager
- Writes HTML and JavaScript code
- Creates functional web applications
- Follows technical best practices

### 👔 Project Manager Agent
**What it does**: Acts like a quality supervisor who ensures everything meets standards.
- Reviews the code created by the Software Engineer
- Checks that all requirements are completed
- Ensures quality standards are met
- Gives final approval by saying "approve" when satisfied

## How the System Works - Step by Step

### Step 1: Setting Up the AI Framework
The notebook begins by importing powerful AI libraries called **Microsoft Semantic Kernel Agents**. Think of these as the "brain" that powers our AI agents.

**What happens**: The system downloads and prepares specialized tools for creating AI agents that can have conversations and work together.

### Step 2: Loading Your AI Configuration
The system reads your personal AI settings from a configuration file.

**What happens**: 
- Loads your Azure OpenAI credentials (like a password for AI services)
- Connects to Microsoft's powerful GPT-4 AI model
- Sets up secure communication with the AI service

### Step 3: Creating the AI "Kernel"
A **kernel** is like the central brain that all AI agents use to think and communicate.

**What happens**: The system creates a shared "thinking engine" that connects to Azure OpenAI, allowing all agents to use advanced AI capabilities.

### Step 4: Defining Agent Personalities
Each AI agent gets a specific personality and role description.

**What happens**:
- **Program Manager**: Programmed to understand requirements and create plans
- **Software Engineer**: Programmed to write HTML/JavaScript code
- **Project Manager**: Programmed to review work and give approvals

### Step 5: Creating the AI Agents
The system transforms the personality definitions into actual working AI agents.

**What happens**: Three intelligent agents are created, each with their specific role, name, and connection to the AI brain.

### Step 6: Setting Up Conversation Rules
The system creates rules for how the conversation should end.

**What happens**: An "Approval Termination Strategy" is created that automatically stops the conversation when the Project Manager says "approve" - meaning the work is complete and approved.

### Step 7: Creating the Team Chat
All agents are organized into a group chat where they can collaborate.

**What happens**: 
- A group conversation is set up with all three agents
- Maximum of 10 conversation rounds to prevent endless discussions
- The Project Manager has the authority to end the conversation with approval

### Step 8: Starting the Development Process
A user request is submitted to the AI team to develop a calculator application.

**What happens**:
- The user's request: "I want to develop app which will provide me calculator. Keep it very simple. And get final approval from manager."
- The request is added to the group chat
- Each agent responds in their role, creating a collaborative development process

### Expected Workflow:
1. **Program Manager** receives the request and creates a development plan
2. **Software Engineer** takes the plan and writes the HTML/JavaScript code for the calculator
3. **Project Manager** reviews the code and gives final approval
4. The conversation automatically ends when "approve" is mentioned

## Prerequisites

Before running this AI development team, you need:

1. **Azure OpenAI Access**: An active subscription to [Azure OpenAI](https://azure.microsoft.com/en-us/services/cognitive-services/openai-service/) with a GPT-4 model deployment
2. **Visual Studio Code**: Download from [here](https://code.visualstudio.com/)
3. **.NET Interactive**: Install from [GitHub](https://github.com/dotnet/interactive)
4. **Jupyter Extension**: Install the [Jupyter Notebooks extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) for VS Code

## Setup Instructions

### Step 1: Configure Your AI Connection

1. **Find the template**: Locate `config-template.json` in the project folder
2. **Create your config**: Copy the file and rename it to `config.json`
3. **Add your details**: Open `config.json` and replace the placeholder values:
   - `AOAI_apikey`: Your Azure OpenAI API key
   - `AOAI_endpoint`: Your Azure OpenAI service endpoint URL
   - `AOAI_deploymentname`: The name of your GPT-4 model deployment
4. **Save the file**: Your AI agents now have access to the OpenAI service

### Step 2: Prepare Visual Studio Code

1. **Open the project**: Launch VS Code and open this project folder
2. **Install extensions**: Ensure .NET Interactive and Jupyter extensions are installed
3. **Verify setup**: Check that you can see .ipynb files properly formatted

## Running the Multi-Agent System

### Step 1: Open the Notebook
1. **Navigate**: Find and open `Calculator.ipynb` in VS Code
2. **Select kernel**: Choose ".NET (C#)" as your notebook kernel
3. **Prepare for execution**: Clear any previous outputs if needed

### Step 2: Execute the AI Collaboration
1. **Run sequentially**: Execute each cell in order (or run all cells at once)
2. **Watch the magic**: Observe as each cell prepares a different part of the system
3. **See the collaboration**: The final cell will show the AI agents working together

### What You'll See
- **Setup messages**: Confirmation that libraries and configurations loaded successfully
- **Agent creation**: Notifications that each AI agent is ready
- **Live conversation**: Real-time chat between the AI agents as they develop your calculator
- **Final approval**: The Project Manager's approval message ending the process

## Understanding the Output

When you run the notebook, you'll see a conversation like this:

```
# User: 'I want to develop app which will provide me calculator. Keep it very simple. And get final approval from manager.'
# Assistant - ProgramManagerAgent: '[Detailed project plan for calculator app]'
# Assistant - SoftwareEngineerAgent: '[HTML and JavaScript code for calculator]'
# Assistant - ProjectManagerAgent: '[Code review and final approval]'
```

Each agent contributes their expertise, resulting in a complete calculator application created through AI collaboration.

## Troubleshooting

**If the notebook doesn't run:**
- Verify your Azure OpenAI credentials in `config.json`
- Ensure all VS Code extensions are properly installed
- Check that your Azure OpenAI deployment is active and accessible
- Restart VS Code and try again

**If agents don't respond as expected:**
- Check your Azure OpenAI service limits and quotas
- Verify the deployment name matches exactly
- Ensure your API key has the correct permissions

## What Makes This Special

This project showcases the future of software development where:
- **AI agents collaborate** like human team members
- **Complex tasks are broken down** into manageable parts
- **Quality assurance is built-in** through the review process
- **Complete applications are generated** from simple requests

The multi-agent approach mirrors real-world development teams, making AI development more organized, efficient, and reliable than single-agent systems.