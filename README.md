# redis-deploy

1.Ceate namesapce:

      kubectl create namespace hacker-company
      
2.For deploying redis in hacker-company namespace:

      kubectl apply -f definition.yaml
     
3.To scale the replica to 2:

      kubectl scale deployment/redis-deployment --replicas=2 (we also can edit the replica field in yaml file and apply it again)
 
4.Exposing thhe container port to 66379
      Handeled it in definition.yaml file itself.
