# Designing for failure

	## Virtual servers (EC2) and elastic IP's

			- Amazon Elastic cloud compute (EC2) are your servers in the cloud
			- Almost any type of applications you're going to run in the cloud, it is most likely
			  to need servers
			- Elastic IP addresses are static IP addresses designed for dynamic cloud computing.
			  An Elastic IP address is created within your account and is not specific to a particular
			  instance. When you create a new elastic IP, you control this address until you choose to
			  explicitly release it.
			- so using Elastic IPs, you can quickly remap and failover to another set of servers so that 
			  your traffic is routed to the new servers. This works well for emergencies but also works 
			  well for rolling out new versions of hardware and software.

	## AWS Regions

			- EC2 instances can be launched in one or more geographical regions
			- Utilize multiple availability zones, and even multiple regions if required. Availability zones
			  are conceptually like logical data centers and by deploying your architecture to multiple
			  availability zones, you can ensure high availability, and recover easily from unforseen disasters.

	## Amazon Machine Image (AMI)

			- An AMI is basically a packaged environment containing software stack, along with all necessary parts
			  to properly set up and boot an EC2 instance.
			- AMIs are your unit of deployment. You specify an AMI when you launch an instance

			### Amazon Machine Image Contents:

				- template for root volume -ex operating system
				- launch permissions - that control which AWS accounts can use the AMI to launch instances
				- block device mapping - to attach to the instance when launched
				- AWS Console -> creating a new instance > click launch > Step1 Choose AMI (this allow you to start 
				  an instance from an existing Amazon package)






