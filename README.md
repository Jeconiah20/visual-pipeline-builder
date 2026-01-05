Visual Pipeline Builder

This project is a visual pipeline builder built using React, ReactFlow, and FastAPI.

Users can create pipelines by dragging and connecting different types of nodes such as Input, Text, LLM, and Output. Each node represents a step in a pipeline, and edges define the flow between steps.

To reduce repeated code, a reusable BaseNode component is used to create multiple node types with consistent structure and styling. New nodes can be added easily by extending this base component.

The Text node dynamically resizes as the user types.
The frontend sends pipeline data to a FastAPI backend, which validates the pipeline by counting nodes, edges, and checking whether it forms a Directed Acyclic Graph (DAG).

This project was completed as part of a frontend technical assessment.

Tech Stack
React
ReactFlow
Zustand
FastAPI
Python

How to Run

Frontend
cd frontend
npm install
npm start


Backend
cd backend
python -m uvicorn main:app --reload
