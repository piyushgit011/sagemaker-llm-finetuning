# sagemaker-llm-finetuning
In this sagemaker example, we are going to fine-tune open LLM, zephyr-7b beta using QLoRA and how to deploy them afterwards using the Hugging Face LLM Inference DLC.
In our example, we are going to leverage Hugging Face Transformers, Accelerate, and PEFT. We will also make use of new and efficient features and methods including, Flash Attention,  and Mixed Precision Training.

what we are going to do:

1.Setup Development Environment
2.Load and prepare the dataset
3.Fine-Tune Mistral 7B with QLoRA on Amazon SageMaker
4.Deploy Fine-tuned Mistral 7B on Amazon SageMaker
5.Stream Inference Requests from the Deployed Model using aws lambda aws api.

1. Setup Development Environment:
If you are going to use zeohyr-7b you need to login into our hugging face account, to use your token for accessing the gated repository. We can do this by running the following command:

!huggingface-cli login --token YOUR_TOKEN

we are going to use Sagemaker in a local environment. You need access to an IAM Role with the required permissions for Sagemaker.

2.
