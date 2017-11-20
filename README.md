# ELK - Demo
![ELK - Stack ](https://logz.io/wp-content/uploads/2017/03/elk-pipeline-in-docker-environment.png)
## What's this ?
<p>This is a simple ELK Stack Demo App, it generates data based on the mouse movement done in the browser window.</p>
<p>The generated data is sent over to rest api which inturns send it to Logstash. Logstash pipes this data to ElasticSearch and finally the data is visualize in the UI using Kibana.</p>

## Move your mouse !
<p>To generate random data all you've got to do is move your mouse pointer over the empty space of the browser window (left or right part).</p>
<p>The rate at which the data is generated and sent depends upon the rate of the mouse movement.</p>

## Note to self !
<p>If you happen to get <b> "No results found " </b>, it because you've not been moving the mouse.</p>
<p>The rate at which the data is received and sent from Logstash can be seen at the top.</p>
<p>Kibana has the restriction for refresh interval, the minimum value which is possible is 5sec. Hence, the visualiation shown in UI is for the 5sec older data.</p>
<p>This app runs with single instance of Logstash and Kibana. So, even if you haven't move the mouse yet you see Logstash transfers (IN and OUT) changing, it's probably because someone else is moving mouse in his/her browser.</p>

## Install and Run
1. ```npm install```

1. ```npm start ```
