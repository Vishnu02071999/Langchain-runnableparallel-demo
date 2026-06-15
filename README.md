# Langchain-runnableparallel-demo
This project demonstrates how to use LangChain's `RunnableParallel` to execute multiple AI tasks simultaneously using different Large Language Models (LLMs).

## Overview

The workflow performs three steps:

1. **Generate concise study notes** from the input text using OpenAI.
2.  **Generate five question-answer pairs** from the same text using Anthropic Claude.
3.  **Merge both outputs** into a single structured learning document.

By running the note-generation and quiz-generation tasks in parallel, the application reduces overall execution time while showcasing LangChain's workflow orchestration capabilities.

## Features

- Parallel execution with `RunnableParallel`
  
- Multi-LLM integration (OpenAI + Anthropic)
  
- Prompt engineering using `PromptTemplate`
  
- Output formatting with `StrOutputParser`
  
- Chained workflow composition using LangChain Expression Language (LCEL)
  
- Graph visualization of the execution pipeline

## Workflow Architecture

Input Text
│
├── Notes Generation (OpenAI)
│
├── Quiz Generation (Anthropic Claude)
│
└── RunnableParallel
│
▼
Merge Results
│
▼
Final Learning Document

## Technologies Used

- LangChain
  
- OpenAI GPT Models
  
- Anthropic Claude Models
  
- Python
  
- dotenv

  ## Learning Objectives

This project helps developers understand:

- Parallel task execution in LangChain
- Combining outputs from multiple AI models
- Building scalable AI pipelines
- Using LCEL operators (`|`) for chain composition
- Visualizing chain execution graphs

