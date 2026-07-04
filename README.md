# AzureFunctions Python - Engineering Project Data Pipeline

A dedicated Python-based serverless project leveraging Azure Functions to manage complex background jobs, continuous data transformations, and asynchronous API tasks. Developed as a major technical pillar of an engineering thesis, this application highlights how to build a highly responsive, cloud-native data pipeline without the system administrative overhead of maintaining permanent server operating systems.

## How It Works
This project takes full advantage of the modern Azure Functions Python V2 programming model. Unlike older configurations, this framework lets you define routes, cron schedules, and cloud resource bindings directly inside your Python application scripts using elegant, readable decorators. 
* Asynchronous Processing: The codebase is engineered to handle long-running data workflows asynchronously, preventing blocking issues when processing large analytical datasets.
* Compute Scales: Compute resources scale up instantly during heavy extract-transform-load (ETL) tasks and scale back down to zero when the pipeline is idle.

## Getting Started
Before setting up the project locally, confirm that you have these requirements installed on your machine:
* Python (version 3.10 or higher is highly recommended)
* Azure Functions Core Tools (v4.x)
* An active virtual environment tool (like built-in venv or Poetry)

Get your local sandbox ready with these command line steps:

1. Clone the project files down to your environment:
   git clone https://github.com/barankiewicz/AzureFunctions-Python-Inzynierska.git
   cd AzureFunctions-Python-Inzynierska

2. Create a clean virtual environment to isolate your libraries:
   python -m venv .venv
   source .venv/bin/activate  # If you are running on Windows, use: .venv\Scripts\activate

3. Install the application dependencies listed in the requirements manifest:
   pip install -r requirements.txt

4. Launch the local serverless development runtime host:
   func start
