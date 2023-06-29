# Azure Machine Learning <3 OpenAI

Learn how to connect Azure Machine Learning with Azure OpenAI, without the use of shared API keys.

Best practice in an enterprise environment is to [disable public internet access](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-virtual-networks?tabs=portal) to your Azure OpenAI resource and to enforce a policy that [disables local authentication methods (key based access)](https://learn.microsoft.com/en-us/azure/cognitive-services/policy-reference#azure-cognitive-services). This will give you full control of whom is able to access your Azure OpenAI resource and mitigate the risks of shared API keys.

## Notebooks

When you use a Compute Instance in Azure Machine Learning, you can utilize the following notebooks to authenticate to your Azure OpenAI resource, without having to provide any credentials in your code.

- [Access OpenAI via Compute Instance Managed Identity](/notebooks/access-openai-via-managed-identity.ipynb)
- [Access OpenAI via User Identity (credential passthrough)](/notebooks/access-openai-via-user-identity.ipynb)
- [Access OpenAI via User Identity (credential passthrough) and API key (via API Management proxy)](/notebooks/access-openai-via-user-identity-apim.ipynb)

