# choreo-image-push

This action make login and push images to container registries

## Inputs
``type`` - Action type
 - login : docker login
 - login_and_push:  docker login and push the image

## Example usage

```yaml
build:
    steps:
    - name: Image Push
      uses: choreo-templates/choreo-image-push@v1.0.6
      with:
       type: login_and_push
       organizationUuid: ${{ env.ORG_UUID }}
```
