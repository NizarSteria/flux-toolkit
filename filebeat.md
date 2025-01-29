kubectl get no worker-*** -L heat --show-labels


kubectl get po -n elastic-beats

kubectl logs -f metricbeat-2ckbd -n elastic-beats

Filebeat -> producer kafka -> topic kafka -> pipelines logstash -> kibana:


kubectl top pods -n elastic-beats 

NAME                          CPU(cores)   MEMORY(bytes)   
filebeat-masters-4872z        25m          50Mi            
filebeat-masters-qdqpp        23m          49Mi            
filebeat-masters-qqhwj        23m          56Mi            
filebeat-masters-xw7vg        22m          48Mi            
filebeat-workers-65wcg        74m          234Mi           
filebeat-workers-9hvjz        44m          61Mi  
metricbeat-2ckbd              77m          97Mi                      
metricbeat-fkn25              52m          89Mi            
metricbeat-ggjj6              73m          86Mi            
metricbeat-gv6jm              66m          95Mi 
