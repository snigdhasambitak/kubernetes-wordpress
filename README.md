# kubernetes-wordpress
A sample wordpress app to deploy in kubernetes using sql backend

To install all the wordpress and sql deployment and service yaml plus ingress use the following command.

kubectl apply -f .

Now you can finish the installation of your Wordpress application using the following details :

Database name : wordpress as defined in the DB’s yaml file

User name : root

Password : aStr0ngPassW0rd as defined in yaml too

Database host : mysql or mysql.wordpress-example.svc.cluster.local

As you can see, talking to your DB from your frontend pod is not difficult due to the creation of our mysql service. Without this you would have had to find the actual container IP, and then change it if the pod were recreated due to an update or outage.
