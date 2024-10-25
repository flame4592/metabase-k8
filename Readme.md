1. Create a Kubernetes secret that stores sensitive PostgreSQL credentials secret.yaml . Values are base64 encoded (not encrypted)
and these secrets will be mounted as environment variables in the Metabase pod.

2. Create a configmap to store any non-sensitive configuration using configmap.yaml

3. Create the pod using the deployment.yaml file

4. Create the service of the metabase pod using the service.yaml file

5. Finally we can attach the service with ingress using the ingress.yaml file , nginx has been used here .

To create any of the above files run the following command :-  kubectl apply -f <file_name>
