# Pub-SubDesign

This is a Google cloud producer-consumer system. A producer reads data form a CSV file and send it to a topic. The consumer receives and process those data send by the producers. 

How It Works.

Producer:

Reads rows from Labels.csv. 

Converts each row into a JSON message.

Publishes the messages to a Pub/Sub topic.


Consumer:

Listens to the topic via a subscription.

Processes and prints each message.


Create a Pub/Sub Topic and Subscription:

In Google Cloud Console, create a topic named topicLabel and a subscription named topicLabel-sub.
Add Credentials:

Download your service account key (service-account.json) and place it in the same directory as the scrip 
Ensure the Lable.csv is in the same directory. 



Run the srcipt in the terminal. 

Producer

python producer.py


For Consumer

python consumer.py
