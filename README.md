# Test Excersise DevOps

#### Spec
Usign k8s
Prepare Kafka cluster with possibility for external access.
Prepare Kubernetes deployment that listen to kafka topic.
Prepare Kubernetes job that produce N messages of random strings to kafka topic. User should be able to use value file to override number of messages. Should be 5 by default.

#### Expected results
Git repo that contains:
- 3 helm charts
1. Chart with custom values for incubator/kafka chart (use helm requirements for refference original chart)
2. Chart with kafka console toolset that has entrypoint for reading messages from topic TEST (use deployment with single replica)
3. Chart with kafka console toolset that has entrypoint to push N messages to topic TEST (use job with no restart policy)
- README.md with *how to use* instructions


