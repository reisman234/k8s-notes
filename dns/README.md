# Specify DNS Records 


- define in the pod.spec the hostAliases entry
  ```
  ...
    hostAliases:
    - ip: X.X.X.X
      hostnames:
      - db1.domain.com
      - db2.domain.com
  ...
  ```
- specify clusterwide by configure the coredns configmap 

https://stackoverflow.com/questions/37166822/is-there-a-way-to-add-arbitrary-records-to-kube-dns

## Question
- is it possible to use a mutating webhook to define dns at namespace level? 
