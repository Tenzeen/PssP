Ran into an error when trying to access localhost/patients after running my flask app. Screenshot_1 in the error folder is a picture of the error message I recieved. 

(sqlalchemy.exc.OperationalError: (pymysql.err.OperationalError) (2003, 'Can\'t connect to MySQL server on \'("104.155.136.209")\' ([Errno 11001] getaddrinfo failed)')
(Background on this error at: https://sqlalche.me/e/14/e3q8)))

I took the following steps to attempt to resolve this error:

    - Made sure that bind address was set to 0.0.0.0 and port was set to 3306 in the mysqld.cnf file
    
    - Made sure that my GCP mysql instance connections settings was set to 0.0.0.0/0
    
    - Made sure my firewall settings were set up correctly (screenshot_3)
    
    - Ran a test in my terminal to see if I could connect to my mysql IP address. (screenshot_2)
    
        - The connection was successful

I am able to use mysql workbench and connect to my mysql database, but the flask app won't work.

Also, I was unable to access my website using 0.0.0.0 in the url. I used localhost instead. 


# Update!
## Errors have been resolved!
.env file contained syntax errors
