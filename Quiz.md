# Docker quiz sample

- If you wanted to view running containers as well as containers that you have stoped and not removed, what command would you use?

-> Docker container ls -a 

</br> 

- What does the -d flag do in a docker run command? 

It detaches the container to run in the background, and returns you to the shell prompt

</br> 

- Would the following two commands create a port conflict error with each other?
  
    Docker container run -p 80:80 -d nginx
  
    Docker container run -p 8080:80 -d nginx
  
-> No 

</br> 

- I ran ‘docker container run -p 80:80 nginx’ and my command line is gone and everything looks frozen. why?

-> Because you didn’t specify the -d flag to detach it in the background, and there aren’t any Ngnix logs yet.  
