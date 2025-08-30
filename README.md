LLM Security Study Script This Jupyter Notebook contains a comprehensive script for conducting a security study on Large Language Models (LLMs) by testing them against various attack vectors. The script is designed to be a "Policy Engine Efficacy Testbed" and a "Container Escape Gauntlet" to evaluate the resilience of different defense systems.

Overview The notebook automates the process of generating attack prompts and evaluating the LLM's responses. It uses predefined prompts and user-defined attack types to simulate real-world security threats. The primary goal is to assess how different defense configurations (e.g., "Multilayered," "Double Layer," "No Defence") perform in preventing successful attacks.

Features Automated Attack Simulation: Automatically generates and executes attack prompts against an LLM.

Configurable Defenses: Allows testing of multiple defense configurations to compare their effectiveness.

Attack Categorization: Classifies attacks into different types (e.g., Jailbreak, Prompt Injection, Container Escape).

Automated Scoring: Calculates and displays a risk score based on the ratio of successful to failed attacks.

Detailed Reporting: Generates a summary table showing the number of successful and failed attacks for each defense configuration.

Getting Started Prerequisites A Google Colab environment or a local Python environment with Jupyter Notebook installed.

API keys for the LLM providers you wish to test (e.g., OpenAI, Hugging Face).

Setup Open the Notebook: Open LLM_Security_Study_Script (final).ipynb in your chosen environment.

Install Dependencies: Run the first cell to install the required Python libraries.

Configure API Keys:

The notebook is set up to retrieve API keys from Google Colab's "Secrets" feature.

If you are using Google Colab, go to the key icon on the left sidebar, click "Add new secret," and add your keys with the names OPENAI_API_KEY and HF_TOKEN.

If you are running the notebook locally, you can directly paste your keys into the designated variables at the top of the script.

Run the Notebook: Execute the cells in order to run the security study.

Usage The notebook is divided into logical sections:

API Key Setup: Initializes API clients.

Core Functions: Defines the primary functions for running attacks and evaluating responses.

Attack Configuration: Configure the attack types, defense systems, and the number of tests to run.

Main Execution Block: Executes the security study and prints the results.

Results and Visualization: Displays a summary table of the study's findings.

After running the complete notebook, you will see a detailed table in the output that quantifies the performance of each defense system.

License This project is open-source and available under the MIT License.
