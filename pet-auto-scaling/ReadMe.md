Task 

1. Launch a 3 tier applciation , across 3 azs , 1 front end instance, one back end instance and one database in each az
2. Create an austo scaling group for the front end [ the concept would be the same for the back end ]
3. Associate the auto scaling group with a load balancer 

Resources.

a private and public subnet in each of the three azs 

3 Front end instances , in af-south-1a , af-south-1b , af-south-1c

3 back end instances , in af-south-1a , af-south-1b , af-south-1c


a security group that opens the load balanncer to tcpip traffic from the internet  on port 8785

a security group that opens port 8785 on the auto scaling group  to traffic from the load balancer

a security group that opens database connections on port 5432 to traffic from the auto scaling group

