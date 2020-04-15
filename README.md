# GCP Custom Roles

I can not create the custom role from Editor role, because there's the maximum of 2087 permissions in a custom role.

## Create a Limit Editor

```
gcloud iam roles create limiteditor \
  --project=$(gcloud config get-value core/project) \
  --file=<(curl -so- https://raw.githubusercontent.com/timfanda35/gcp-custom-roles/master/limitEditor.yml)
```
