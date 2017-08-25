# Three Tier Infrastructure

The three tire infrastructure has an ELB, Apache Web Server and a RDS Database. This infrastructure provides High Availability and Scalability. 

### Instructions

The yaml template takes Stack Name, Instance type and SSH Key as Input. Cloudformation creates a 3 Tier architecture with Elastic Load Balancer accepting connections to port 80, Apache Web Server EC2 Instances would serve the requests through the Elastic Load Balancer and Apache Web Server will connect to the RDS Database for data.   

*Output : Provides an Elastic Load Balancer URL that displays a Sample PHP App that has the Instance Hostname of the instance the page is being serverd from.* 

## Best Practices Used

1. ELB with Healthcheck
2. MultiAZ provides High Availability
3. AutoScaling Up/Down
4. Security Groups 

[Infrastruture](./Infra.jpg)
