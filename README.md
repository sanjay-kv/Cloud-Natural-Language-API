# Cloud-Natural-Language-API
Syntax Analysis/Entity Recognition/Sentiment Analysis/Content Classification/Multi-Language/Integrated REST API

Run this command in Cloud shell

gcloud auth list

gcloud config set account `ACCOUNT`

gcloud config list project

# Create API 

export GOOGLE_CLOUD_PROJECT=$(gcloud config get-value core/project)

gcloud iam service-accounts create my-natlang-sa \
  --display-name "my natural language service account"
  
  gcloud iam service-accounts keys create ~/key.json \
  --iam-account my-natlang-sa@${GOOGLE_CLOUD_PROJECT}.iam.gserviceaccount.com
  
  export GOOGLE_APPLICATION_CREDENTIALS="/home/USER/key.json"
  
  Make ANalysis report
  
  Below code to run in SSH
  
  gcloud ml language analyze-entities --content="Michelangelo Caravaggio, Italian painter, is known for 'The Calling of Saint Matthew'." > result.json
  
  
  
  
