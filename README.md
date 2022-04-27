# Dockerised_Kafka #

#### This is a simple dockerised Kafka project. It can be run as follows:

1. Create a virtual environment in the project root directory
``` 
python3 -m venv venv
```
2. Activate the virtual environment
``` 
source venv/bin/activate
```
3. Install dependencies
``` 
pip install -r requirements.txt
```
4. Create Docker containers
``` 
docker-compose up
```
5. Once the server is up and running, open two additional terminal windows
6. Activate the virtual environment in both terminal windows
7. In one terminal window add the following:
``` 
python producer.py
```
8. In the other terminal window add the following:
``` 
python consumer.py
```
9. Execute the ```producer.py``` command
10. Execute the ```consumer.py``` command

In the ```consumer.py``` terminal you should see something like the following:
``` 
{'number': 6} working!
{'number': 7} working!
{'number': 8} working!
{'number': 9} working!
{'number': 10} working!
{'number': 11} working!
{'number': 12} working!
{'number': 13} working!
{'number': 14} working!
```

From here you can experiment with Kafka, including stopping and starting ```producer.py``` or adding more descriptive messages. Have fun!

