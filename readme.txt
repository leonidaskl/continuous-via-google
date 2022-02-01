gcloud build submit --tag gcr.io/<Project-Name>/<AppName> --project=<Project-Name>

gcloud run deploy <AppName> --image gcr.io/<Project-Name>/<AppName> --platform managed --project=<Project-Name> --allow-unauthenticated --region us-east1

gcloud iam service-accounts list --project=<Project-Name>

gcloud iam service-accounts create ./keys.json --iam-account github-actions@arboreal-cosmos-338023.iam.gserviceaccount.com

gcloud auth activate-service-account --key-file=keys.json