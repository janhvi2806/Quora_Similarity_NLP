# Quora Similarity Model

This project involves the deployment of a classification model that achieves 77% accuracy. The model's performance metrics and a detailed plan for scaling and potential cloud deployment are provided below.

## Performance Metrics

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.77      | 0.87   | 0.81     | 50803   |
| 1     | 0.71      | 0.55   | 0.62     | 30055   |

*Overall Metrics:*
- *Accuracy*: 0.77
- *Macro Avg Precision*: 0.74
- *Macro Avg Recall*: 0.71
- *Macro Avg F1-Score*: 0.72
- *Weighted Avg Precision*: 0.75
- *Weighted Avg Recall*: 0.75
- *Weighted Avg F1-Score*: 0.74

## Scaling the Solution to Larger Datasets

### Data Preprocessing and Management
- *Distributed Storage*: Utilize HDFS, Amazon S3, or Google Cloud Storage.
- *Efficient Data Loading*: Employ frameworks like Apache Spark or Dask for parallel data processing.

### Model Training
- *Distributed Training*: Use TensorFlow Distributed, PyTorch Distributed, or Horovod.
- *Optimization Techniques*: Apply gradient checkpointing, mixed precision training, and model parallelism.

### Hardware Considerations
- *High-Performance Computing*: Leverage clusters with multiple GPUs or TPUs.
- *Autoscaling*: Implement autoscaling for computational resources.

## Cloud Deployment Plan

### Infrastructure Setup
- *Cloud Provider*: Choose AWS, GCP, or Azure.
- *Containerization*: Use Docker for containerizing the application.

### Service Deployment
- *Kubernetes*: Manage and scale containerized applications with Kubernetes.
- *Managed Services*: Utilize AWS SageMaker, GCP AI Platform, or Azure Machine Learning.

### Continuous Integration/Continuous Deployment (CI/CD)
- *CI/CD Pipeline*: Use Jenkins, GitHub Actions, or GitLab CI/CD.
- *Monitoring and Logging*: Implement Prometheus, Grafana, and ELK Stack.

### Scaling and Maintenance
- *Auto-Scaling*: Configure policies to adjust the number of instances based on demand.
- *Regular Updates*: Continuously update the model and application code.

## Reflection

### What Worked Well
1. *Efficient Model Performance*: Achieved satisfactory performance metrics.
2. *Scalability*: Easy scalability with distributed training and cloud deployment strategies.
3. *Automation*: Consistent, repeatable, and automated deployments with CI/CD.

### Areas for Improvement
1. *Data Imbalance*: Address through techniques like SMOTE or re-sampling.
2. *Hyperparameter Optimization*: Further tuning and experimentation.
3. *Real-Time Monitoring*: Implement real-time monitoring and alerting systems.
4. *Resource Optimization*: Continuous evaluation and optimization of computational resources.

## Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook

### Installation

1. Clone the repository:
    sh
    `git clone https://github.com/janhvi2806/Quora_Similarity_NLP.git`
   
    cd Quora_Similarity_NLP
    

3. Start Jupyter Notebook:
    sh
    jupyter notebook
    

4. Open and run the provided notebooks to explore the data, train the model, and evaluate performance.
