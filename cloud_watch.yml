cloud_watch is a:
  A general purpose time-series metrics data store:


cloud_watch:
  core_concepts:
      -  1. Namespaces
         - AWS Services reside in the AWS/  Namespace:
            - Each AWS service has its own namespace:
              - AWS/EC2
              - AWS/S3
              - AWS/EBS

         - Custom Namespaces can be created for the custom metrics:


      -  2. Dimensions
         - Its a key - value pair that contains information to help and identify the metrics:
            - Used for Grouping and filtering


      -  3. Metrics 
         - Sample of time-series data identified by the combination of namespace name and metric name:




1. aws cloudwatch get-metric-statistics --namespace AWS/EC2 --metric-name CPUUtilization --start-time 2019-09-26T00:00:00Z --end-time 2019-09-26T23:59:59Z --period 60 --statistics Average --dimensions Name=InstanceId,Value=i-05245bb6d535d56ca --region us-west-1 | jq:

2. aws cloudwatch get-metric-statistics --namespace AWS/EC2 --metric-name CPUUtilization --start-time 2019-11-17T00:00:00Z --end-time 2019-11-17T23:59:59Z --period 60 --statistics Average --dimensions Name=InstanceId,Value=i-0bac8256b751a019e --region us-west-1 | jq:

3. aws cloudwatch get-metric-statistics --generate-cli-skeleton --region us-west-1:


4. aws cloudwatch put-metric-alarm --alarm-name cpu-mon-cli  --alarm-description "Alarm when CPU exceeds 20 percent" --metric-name CPUUtilization --namespace AWS/EC2 --statistic Average --period 60 --threshold 20 --comparison-operator GreaterThanThreshold  --dimensions "Name=InstanceId,Value=i-0bac8256b751a019e" --evaluation-periods 2 --alarm-actions arn:aws:sns:us-west-1:172586632398:bharaths_cloudwatch_topic --unit Percent --region us-west-1:


Cloud_watch:
  alarms:
    - 1. OK
    - 2. ALARM 
    - 3. INSUFFICIENT






