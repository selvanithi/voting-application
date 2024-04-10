# voting-application
eks project

created cluster in eks with adding role to that.

made endpoint as public.

in add-ons, added Amazon EBS CSI Driver


created ec-2 instance for accessing cluster with below IAM policies
	
{

"Version": "2012-10-17",
 
	"Statement": [{
 
		"Effect": "Allow",
  
		"Action": [
  
			"eks:DescribeCluster",
   
			"eks:ListClusters",
   
			"eks:DescribeNodegroup",
   
			"eks:ListNodegroups",
   
			"eks:ListUpdates",

			"eks:AccessKubernetesApi"
		],
  
		"Resource": "*"
  
	}]
 
}
install kubctl in the machine and also install git. then clone the repository

created the namespace for cluster
created the pods and services using the mentioned pod files
By using the endpoint of front-end deployment we can access our application.
