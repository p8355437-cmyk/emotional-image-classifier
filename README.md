# Image Emotion Classifier

Welcome! This project is a web application that analyzes an uploaded image to identify the emotions it expresses. This guide will walk you through building the project from scratch using the provided architecture documents and Roo, an AI software engineer.

## Your Mission

Your goal is to build this application by instructing an AI, using the same kinds of architectural documents that professional software teams use. This exercise will give you hands-on experience with AI-driven software development.

## Step 1: Set Up Your Roo Environment

First, you'll need to get Roo ready to help you write the code.

1.  **Install Roo**: If you haven't already, install the Roo extension in your code editor.
2.  **Configure Your Gemini API Key**:
    *   Open the `gemini-key.txt` file.
    *   Replace the placeholder `YOUR_GEMINI_API_KEY_HERE` with your actual Gemini API key.
    *   Follow the instructions within the Roo extension to add your API key.

## Step 2: Build the Application with Roo

Now you're ready to build the application. You will use Roo's **Code Mode**, which is designed for writing, modifying, and refactoring code.

1.  **Start a Conversation**: Open Roo and select **Code Mode**.
2.  **Provide Context**: Your repository contains the following architecture documents:
    *   `business_architecture_overview.md`: Explains the project's purpose and goals.
    *   `technical_architecture.md`: Details the technologies and structure to be used.
    *   `data_privacy_policy.md`: Outlines data handling requirements.
3.  **Instruct Roo**: Tell Roo to build the application based on the `technical_architecture.md` document. You will also need to provide the credentials for the Azure ML service. Here is the information you'll need to give Roo:

    *   **Azure ML Endpoint URL**: `https://emo-endpt-be5265.australiaeast.inference.ml.azure.com/score`
        *   Tell Roo to use the environment variable name: `AZURE_ML_ENDPOINT`
    *   **Azure ML API Key**: `4APrDEtqCIhG2CpK4j1gynYjNhiJheCX2QqO8isyTep6dmCr7YivJQQJ99BJAAAAAAAAAAAAINFRAZML74bp`
        *   Tell Roo to use the environment variable name: `AZURE_ML_API_KEY`

Roo will begin creating the project file by file. Review and approve each step, and you will see the application come to life.

## Step 3: Run the Application

Once Roo has finished writing the code, it's your turn to figure out how to run it. Analyze the files Roo created to determine how to start the frontend and backend servers.

Good luck!