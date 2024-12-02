# Fintelli: An AI-Enabled Financial Advisor

Team Members:
- Shireen Jain
- Amodh Sharma
- Shruti Gupta
- Ananya Prasad
- Harshita Saini

---

## Objective

Fintelli leverages a 3-pipeline architecture to deliver a comprehensive AI-enabled financial advisor. It leverages the following components:

### 1. Training Pipeline
- **Features:**
  - Loads a proprietary Q&A dataset.
  - Fine-tunes an open-source LLM using QLoRA.
  - Logs training experiments on [Comet ML](https://www.comet.com) for Experiment tracking and getting Inference results via Comet ML's LLMOps dashboard.
  - Stores the model in Comet ML's model registry.
  - Deploys the pipeline using Beam's serverless GPU infrastructure.

### 2. Streaming Real-Time Pipeline
- **Features:**
  - Ingests financial news from Alpaca.
  - Cleans and transforms documents into embeddings using Bytewax.
  - Stores embeddings in the Qdrant Vector DB.
  - Automatically deploys to an AWS EC2 machine via a GitHub Actions CI/CD pipeline.

### 3. Inference Pipeline
- **Features:**
  - Uses LangChain to create an inference chain that:
    - Downloads the fine-tuned model from Comet ML's model registry.
    - Processes user questions and queries the Qdrant Vector DB.
    - Enhances prompts with financial news context and chat history.
    - Calls the fine-tuned LLM for financial advice.
    - Logs interactions on Comet ML's LLMOps monitoring dashboard.
  - Deploys as a RESTful API on Beam's serverless GPU infrastructure.
  - Includes a Gradio-based UI for demonstration.

---

## Exploratory Data Analysis (EDA)
The prompts for training were analyzed to gain insights:

### Token Analysis:
- **Metrics:**
  - Average token length.
  - Token length distribution.
  - Min/Max tokens per prompt.

- **Coverage:**
  - Prompt coverage relative to token length.
  - Context size coverage.

- **Insights:**
  - Balanced prompts relative to context size.
  - Distribution skew for sentence lengths.
  - Detection of outliers.

### Word Analysis:
- **Word Cloud:**
  - Visual representation of key topics within the dataset.

---
