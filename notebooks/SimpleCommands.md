## Delete and run the pipelin build
```
kubectl delete PipelineRun fd-pipeline-run-1  -n odhk && kubectl apply -f pipelinerun.yaml -n odhk && tkn pipelinerun logs fd-pipeline-run-1  -f -n odhk
kubectl delete Pipeline fd-model-pipeline && oc apply -f pipeline.yaml
kubectl delete Task bud-push && oc apply -f bud-push-task.yaml
```
