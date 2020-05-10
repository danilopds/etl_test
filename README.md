# etl_test

Prerequisite for Code:
- Python Basics
- Classes and Objects
- Pandas and Numpy
- API’s (request module)
- JSON and CSV files
- MongoDB (pymongo module)	

## Notes - Setup test environment #

Refs:
Python ETL Pipeline
	- https://medium.com/datadriveninvestor/complete-data-analytics-solution-using-etl-pipeline-in-python-edd6580de24b
	- https://codeburst.io/using-python-script-for-data-etl-53138c567906
Open API
	-https://docs.openaq.org/

Requiriments:
- Python + PIP (sudo apt-get install..)
- Text Editor - Sublime (via Ubuntu Software)
- Mongodb instance 
	sudo apt install mongodb-server
	sudo mongod
- Git (via apt-get install git)
	1. Create repository on github (https://github.com/danilopds/etl_test)
	2. Clone localy
		a) git clone https://github.com/danilopds/etl_test.git
	3. Test Commit (workflow)	
		a) git add .
		b) git commit -m "xx"
		c) git push (user and pass necessary)
	
Prerequisite for Code:
- Python Basics
- Classes and Objects
- Pandas and Numpy
- API’s (request module)
- JSON and CSV files
- MongoDB (pymongo module)	

Funcional rules:
Project in which we use Pollution data, Economy data and Cryptocurrency data. Let’s assume that we want to do some data analysis on these data sets and then load it into MongoDB database for critical business decision making or whatsoever.

Data sources:
API : These API’s will return data in JSON format.
	- Pollution Data: 	"https://api.openaq.org/v1/latest?country=IN&limit=10000" .
	- Economy Data: 	"https://api.data.gov.in/resource/07d49df4-233f-4898-92db-e6855d4dd94c?api-key=579b464db66ec23bdd000001cdd3946e44ce4aad7209ff7b23ac571b&format=json&offset=0&limit=100"
CSV Data
	- Crypto Currencies: "https://raw.githubusercontent.com/diljeet1994/Python_Tutorials/master/Projects/Advanced%20ETL/crypto-markets.csv"

1. Create requirements file
	sudo pip install pymongo
	sudo pip install requests
	sudo pip install pandas

2. Create extract, transform, load code		
	code examples provided