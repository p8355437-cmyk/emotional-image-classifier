# Image Emotion Classifier

Welcome! This project is a web application that analyzes an uploaded image to identify the emotions it expresses. This guide will walk you through building the project from scratch using the provided architecture documents and Roo, an AI software engineer.

## Your Mission

Your goal is to build this application by instructing an AI, using the same kinds of architectural documents that professional software teams use. This exercise will give you hands-on experience with AI-driven software development.

## Step 1: Build the Application with Roo

You're ready to build the application. Your environment is already set up with Roo and the necessary API key. You will use Roo's **"code" mode** to instruct it to build the application based on the provided architecture documents.

1.  **Start a Conversation with Roo**:
    *   Open the Roo extension by clicking on its icon in the activity bar on the side of your editor.
    *   Ensure you are in **"code" mode**.
    *   Send the following message to Roo to begin:

    "Hello. Please build the application as described in the `technical_architecture.md` document. This document outlines the project's technical requirements, including the frontend, backend, and necessary environment variables. The `business_architecture_overview.md` and `data_privacy_policy.md` files are also available for additional context on the project's goals and data handling policies."

2.  **Provide Azure Credentials When Prompted**:
    Roo will require credentials for the Azure ML service. When it asks for them, provide the following information:

    *   **Azure ML Endpoint URL**: `https://emo-endpt-be5265.australiaeast.inference.ml.azure.com/score`
        *   Tell Roo to use the environment variable name: `AZURE_ML_ENDPOINT`
    *   **Azure ML API Key**: `4APrDEtqCIhG2CpK4j1gynYjNhiJheCX2QqO8isyTep6dmCr7YivJQQJ99BJAAAAAAAAAAAAINFRAZML74bp`
        *   Tell Roo to use the environment variable name: `AZURE_ML_API_KEY`

Roo will begin creating the project file by file. Review and approve each step, and you will see the application come to life.

## Step 2: Run the Application

Once Roo has finished writing the code, it's your turn to figure out how to run it. Analyze the files Roo created to determine how to start the frontend and backend servers.

Good luck!