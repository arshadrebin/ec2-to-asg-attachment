### Attachment of EC2 instance to Auto Scaling group

1) Create EC2 Instance (if not already done).
2) Create an AMI of the mentioned instance.
3) Create Launch Configuration. Ensure to choose newly created AMI for the Launch configuration creation.
 <img width="657" alt="Capture" src="https://github.com/arshadrebin/ec2-to-asg-attachment/assets/116037443/d89912f0-26db-4e4c-a8fa-793f55b47036">
 
4) Create Auto Scaling group with the above launch configuration. The group size should be below parameters.

#### Desired capacity = 0

Desired capacity represents the initial capacity of the Auto Scaling group at the time of creation.

#### Minimum capacity = 0

Minimum capacity refers to the minimum number of instances that should be running in an Auto Scaling group (ASG) at all times, even during periods of low demand or when scaling down.

#### Maximum capacity = 1

The maximum capacity refers to the upper limit on the number of instances that can be launched and maintained by an Auto Scaling group (ASG).

<img width="470" alt="Capture1" src="https://github.com/arshadrebin/ec2-to-asg-attachment/assets/116037443/44cc6f08-4d11-4ca5-bba7-2d0e73235412">

5) Attach the EC2 to created ASG. Go to EC2 section >> Instances >> Select the instance >> Attach to Auto Scaling group >> 
   Select the mentioned Auto Scaling group.

<img width="800" alt="Capture2" src="https://github.com/arshadrebin/ec2-to-asg-attachment/assets/116037443/194e3c1a-4e1e-4e8c-b4a9-e6af709a94e0">

<img width="720" alt="Capture3" src="https://github.com/arshadrebin/ec2-to-asg-attachment/assets/116037443/c1452001-e8ba-4c3f-93e2-bf05c401f3db">

Activity history of the Auto Scaling Group is as below

<img width="772" alt="Capture4" src="https://github.com/arshadrebin/ec2-to-asg-attachment/assets/116037443/fd3c0724-b9e0-4611-8ae1-860d84998406">

