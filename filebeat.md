kubectl get no worker-*** -L heat --show-labels


kubectl get po -n elastic-beats

kubectl logs -f metricbeat-2ckbd -n elastic-beats

Filebeat -> producer kafka -> topic kafka -> pipelines logstash -> kibana:
