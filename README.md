# Build and push docker image to Google Container Registry action

Opinionated github workflow action to build a docker image from Dockerfile
and push the image to Google Continer Registry.

Pass all sensitive data using secrets.

## Inputs

### `service_key`

**Required** Google Service Account Key.

### `google_compute_zone`

### `google_project_id`

### `gcr_host`

### `image_name`

### `image_tag`

## Example usage

uses: raccoondev/push-docker-gcr
with:
  service_key: ${{ secrets.GCLOUD_SERVICE_KEY }}
  google_compute_zone: ${{ secrets.GOOGLE_COMPUTE_ZONE }}
  google_project_id: ${{ secrets.GOOGLE_PROJECT_ID }}
  gcr_host: eu.gcr.io
  image_name: my_image
  image_tag: latest
