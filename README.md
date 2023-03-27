# tekton-project

1. start minikube
2. install tekton pipelines: kubectl apply --filename \
https://storage.googleapis.com/tekton-releases/pipeline/latest/release.yaml

When a Task is part of a Pipeline, Tekton creates a TaskRun object for every task in the Pipeline.

Tekton is made up of 6 main components:

    Step: run commands
    Task: list of steps
    Pipeline: graph of tasks
    Pipeline Resource: a resource that is declared and then referenced and used in tasks and pipelines
    Task Run: invoke a task (Pipeline runs create Task Runs when run)
    Pipeline Run: invoke a pipeline