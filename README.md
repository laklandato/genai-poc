# GENAI PoC

1. Provision demo environment "RHOAI on OCP on AWX with NVIDIA GPUs" provision time around 90mins
https://catalog.demo.redhat.com/catalog?item=babylon-catalog-prod/sandboxes-gpte.ocp4-demo-rhods-nvidia-gpu-aws.prod&utm_source=webapp&utm_medium=share-link

2. Deploy minio as object buckets.
  - minio/minio123
    Create bucket models
    create folder taide-7b
    create folder taide-8b
    upload llm files

3. Add Custom Workbench
   - anythingLLM quay.io/rh-aiservices-bu/anythingllm-workbench <<- for chatbot UI
   - odh-tools quay.io/rh-aiservices-bu/odh-tec:latest <<- for testing object connections
  
4. Create two project
   - anythingLLM and create anythingLLM workbench
   - odh-tools and create odh-tools workbench

5. Create taide project
   - setup date connection
   - setup model serving with vLLM nvidia GPU(add argu --max-model-len 16000)

6. 
  


OLS = OpenShift Lightspeed.
