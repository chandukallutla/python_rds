# python_rds

  for python 

	step:1 # Create Security Groups
		
		  	ssh = 22
		  	flask = 5000
		  	RDS = 3306


	step:2 # Create Rds =		create rds – mysql 

    1. connect to the ec2 and install mysql client  =
                      dnf install mariadb105-server-y
    2. connect to the database (in the rds console click on the database you created ,in the details section u will get the endpoint of rds and in the configuration section u will find username , db name …etc password u have to store somewhere else). 
                      Mysql -h host -u username -p
    3. show databases;
    4. create database;
    5. show databases;
    6. use   <database Name>;
    
    7. create table (u can replace name,roll,grade column names as u needed ) =
                      CREATE TABLE <tableName>  (     name VARCHAR(50) NOT NULL,     roll INT NOT NULL,     grade CHAR(1) NOT NULL );
                      
                      
    8. insert values (whatever u gave above give the values for it) = 
                      INSERT INTO <tableName> (name, roll, grade) VALUES ('leo hank', 103, 'A');
                      
                      
    9. exit 

Step: 3
	
	# Install dependencies

		1.yum install python3
		2.yum install python3-pip
		3.pip install flask
		4.pip install mysql-connector-python


		

step:4
	
	# create flask app

    1. create a folder =  mkdir <folderName>
    2. goto that folder = cd <folderName>
    3.  create a file with .py extension =  vi app.py ( code is in repo)
                                           = paste the below  flask code to ur app.py file
                 
                 then create templates directory from this directory
    4. create another folder = mkdir templates
    5. create a html code to get the tabular form output.make sure that u have to add  the html code in the templates directory only. below are the two files u can copy and paste it 




	Step: 5 # Change the directory = Cd templates
	Step: 6 #  vi table.html (code is in repo)


   


    • get back to the directory where app.py is present and start the code
    • cd ..

Step: 7
    • python3 app.py
    • now u can access this from the browser with publicIp:5000

