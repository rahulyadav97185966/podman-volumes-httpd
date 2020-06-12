# podman-volumes-httpd

# podman-volumes

#mkdir /data : Create Directory using this command in which the data of the container will be stored

#goto /data (cd /data)
    --> create one file index.html there as one file is created in this repos.then run the below command

#podman run -v /data:/usr/local/apache2/htdocs:Z -d -p 18080:80 docker.io/httpd  : using this command we run the httpd container in backend using -d (detach ) option , Z is for pemissive the SElinux (Security-Enhanced Linux) policies that allows user to create and use file and folders. 

#podman ps : using this command we will see the running containers.

#now go to browser and paste the IP of your system and the port number 18080 as mention in the above command like (192.168.174.05:18080)
and you will see the html pahge that you created there.

#podman exec -it 49 bash : using this command we can access teh running container

