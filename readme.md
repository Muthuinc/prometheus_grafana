#### Monitoring the application is very essential for the continuous and seamless operation of any business. It helps in address issues in real-time, thereby minimizing disruptions and maximizing productivity.

### Prometheus and Grafana
  - There are several ways to install it application among that Installing through Docker is an effective and simplest one.
  - In the same repository i have the Docker-compose file which pulls and respective latest docker images.
  - Also have the default configuration files for promethesu and grafana.

```
docker-compose up -d
```

![Image](./pictures/monitoring.png)  
  
  - Prometheus is up and running.

![Image](./pictures//proms.png)

  - Grafana is up and running.  

![Image](./pictures/grafa.png)    
  
  ---

### Metrics Collection and Visualization

  - Open the prometheus.yml file and the chanhe the IP address of the server we want to monitor.  
  ![image](./pictures/promcon.png)  
  - Prometheus now able to scrape the metrics from the endpoints.  
  - Below is the the application server status.
  ![image](./pictures/appdas1.png)  
  ![image](./pictures/appdas.png)  
    
---
  
### Alerts and Notifications

  - I configured the email notifications settings in the grafana.ini file.
  ![image](./pictures/te.png)  
  - Test notification has been received.
  ![image](./pictures/testalert.png).
  - An alert is set for the application server whenever it goes down it will notify. 
  - The application server is stopped to check for the alerts.  
  ![image](./pictures/g.png)
  - Grafana sent out an alert email regarding the application along with the dashboard.
  ![image](./pictures/firealert.png)


#### Monitoring, including the use of Prometheus and Grafana, is essential for maintaining operational excellence and responding effectively to challenges.
