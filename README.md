# ECS-Start-Stop-Basic


Basic AWS Lambda Python function for Starting and stopping ECS cluster services

The lambda code is dynamic as theres no cluster and service hardcoded in the code

Set the Eventbridge trigger for start and stop like below : 

```batch
For Stopping the services : 

{
  "cluster": "Test",
  "service_name": "test",
  "service_desired_count": "0"
}

For Starting the services : 

{
  "cluster": "Test",
  "service_name": "test",
  "service_desired_count": "1"   # set this to your desired
}
```

Set the cron as per your requirement 