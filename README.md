## Productionizing-RAG-Mental-Wellness-Assistant-with-Azure-AI-Search-OpenAI-Safety-Framework

## 🎯 Project Overview
This project demonstrates the migration of open-source AI components in my previous project 
https://github.com/padmapria/RAG-Care-Mental-Wellness-Assistant
to Azure's enterprise cloud platform, transforming a proof-of-concept into a production-ready medical RAG system with comprehensive LLM evaluation and enterprise-grade safety.

## 🔄 Migration Journey
- **Search**: Elasticsearch → **Azure AI Search** with hybrid vector search
- **LLMs**: Llama3.1, Gemma2, OpenAI API → **Azure OpenAI** (GPT-4.1 Mini, O3-Mini)
- **Safety**: Basic filtering → **Azure AI Content Safety** for enterprise-grade content moderation
- **MLOps**: Manual tracking → **MLflow on Azure** for experiment management

## 📊 Key Features
- Hybrid vector search with semantic retrieval
- Multi-LLM configuration evaluation (3 models tracked)
- Comprehensive metrics: Hit Rate, MRR, semantic similarity
- MLOps pipeline with experiment tracking
- Content safety and moderation

## 🧪 LLM Experimentation Framework
We conducted systematic evaluation of multiple Azure OpenAI models to determine optimal configurations for medical conversations:

### Models Tested
- **GPT-4.1 Mini** (Temperature 0.8) - Creative variant
- **GPT-4.1 Mini** (Temperature 0.5) - Balanced variant  
- **O3-Mini** - Reasoning-optimized model

### Evaluation Methodology
```python
# Example evaluation metrics tracked
evaluation_metrics = {
    "retrieval_accuracy": ["hit_rate@5", "mrr", "ndcg"],
    "generation_quality": ["semantic_similarity", "rouge_scores", "relevance"],
    "performance": ["latency", "throughput", "cost_per_query"],
    "safety": ["content_moderation", "false_positive_rate"]
}
```
## 🛡️ Production Architecture
- **Azure AI Content Safety** integration for compliant mental health conversations
- **Enterprise-grade security** with managed identities and RBAC
- **Managed services** reducing operational overhead by 60%
- **Comprehensive monitoring** with Azure Monitor and custom dashboards

## 📊 System Capabilities
- **Intelligent Retrieval:** Hybrid search combining semantic understanding with keyword matching
- **Model Optimization:** Data-driven LLM selection based on performance benchmarks
- **Quality Assurance:** Automated evaluation pipeline with 10+ quality metrics
- **Safety First:** Multi-layer content moderation for sensitive healthcare domain
- **Production Ready:** Scalable, secure, and monitored enterprise architecture

## Notebook: 
### OpenSource RAG Flow and Evaluation   <br/>
(Notebook in the folder `/notebooks/step1_data_preparation.ipynb`) <br/>
[RAG Test Notebook: Step 1](https://github.com/padmapria/RAG-Care-Mental-Wellness-Assistant/blob/master/notebooks/step1_rag_test.ipynb)

### Azure RAG Flow and Evaluation   <br/>
[RAG Azure Implementation: Step 2](https://github.com/padmapria/Productionizing-RAG-Mental-Wellness-Assistant-with-Azure-AI-Search-OpenAI-Safety-Framework/blob/main/notebooks/step2_rag_Azure.ipynb)


## Acknowledgement
I would like to extend my gratitude to the following individuals and organizations for their valuable resources and contributions:
-https://learn.microsoft.com/en-us/azure/machine-learning/concept-workspace?view=azureml-api-2


---
