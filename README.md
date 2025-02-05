python3 -m pip install flask


double click open terminal
cd
mkdir
rmdir
ls
python3 xx/xxx.py
ctrl +c
beware of -(minus sign) as sometimes if I copy it might be wrong
nano xxx.py
ctrl o , enter, ctrl x
ctrl o = save, crtl x = exit



dockerfile: instructions for docker to run when containerizing the application
requirements.txt: python libraries and their respective versions


	1. build docker image : docker build -t flask-app
	2. docker image ls (list all the images locally and check if the app I created just now has been created)
	3. run docker container: docker run flask-app
	4. need to map internal docker port 5000to local machine port 5000: docker run -d -p 5000:5000 flask-app
	5. enter ip address 127.0.0.1:5000 on firefox browser
	6. pushing docker image to docker hub:
		a. docker login
			Username: daccsp
			Ps: 1nbSPDocker (blind type)
		b. tag "flask-app" docker image
			i. docker image tag flask-app daccsp/flask-app
		c. push to docker hub
			i. docker push daccsp/flask-app
![image](https://github.com/user-attachments/assets/17172efa-a853-45b6-b43b-dc386c9f42e6)

			
		
		
