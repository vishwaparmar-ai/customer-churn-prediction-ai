# Customer Churn Prediction & AI Retention Copilot

## Project Goal
Build one portfolio system that demonstrates traditional ML fundamentals, production ML engineering, MLOps, 
backend/API engineering, GenAI integration, AI observability, CI/CD and AWS deployment. The ML model predicts 
churn; the LLM does not replace the model. It receives the model prediction and structured customer context and 
produces an explainable retention recommendation and customer message.


## Target Architecture
Data → validation → preprocessing/features → model training → evaluation → MLflow tracking/registry → model artifact → FastAPI inference → SHAP explanation → LLM retention reasoning → structured response → logs/metrics/traces → Docker → GitHub Actions CI/CD → AWS 

## Repository structure 
customer-churn-ai/ 
├── src/ 
│   ├── data/              
AWS Secrets Manager / environment 
variables locally 
│   ├── features/          
│   ├── models/            
│   ├── llm/               
│   ├── api/               
│   ├── observability/     # logging/tracing/metrics helpers 
│   └── config.py 
├── tests/ 
│   ├── unit/ 
│   └── integration/ 
├── notebooks/              
├── configs/ 
├── scripts/ 
├── artifacts/              
├── Dockerfile 
├── docker-compose.yml 
├── pyproject.toml 
├── .env.example 
├── README.md 
└── .github/workflows/ci.yml

