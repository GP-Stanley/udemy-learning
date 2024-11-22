

# How to turn your EC2 Instances back on
We now have three EC2 Instances:
* Grafana.
* Prometheus.
* RDS.

Start Docker Dashboard. 
Start EC2 Instances. 

## Starting Grafana Instance
* "Connect" the instance and SSH in to a Git Bash Terminal. 
* Start Docker Service: `sudo systemctl start docker`
* Check docker status: `sudo systemctl status docker`
  * Click "q" to exit screen.

![alt text](./grafana-images/image-29.png)

* Run the Container: `sudo docker run -d -p 3000:3000 --name=grafana grafana/grafana`

![alt text](./grafana-images/image-30.png)
 
* Navigate to your web browser. 
* Check Grafana is working by taking the public IP of the instance and adding `:3000` on the end.

![alt text](./grafana-images/image-31.png)

* To log in, you can type "admin" twice and select **Skip** if prompted again. 

### The container name "grafana" is already in use
1. Stop the existing container: `sudo docker stop grafana`
2. Remove the existing container: `sudo docker rm grafana`
3. Run the new container: `sudo docker run -d -p 3000:3000 --name=grafana grafana/grafana`

<br>

## Starting Prometheus Instance
* "Connect" the instance and SSH in to a Git Bash Terminal. 
* Start Prometheus using: `sudo systemctl start prometheus`.
* Enable it using: `sudo systemctl enable prometheus`.

![alt text](./grafana-images/image-32.png)

* Navigate to your web browser. 
* Check Prometheus is working by taking the public IP of the instance and adding `:9090` on the end.

![alt text](./grafana-images/image-33.png)

<br>

## Starting RDS Instance
* "Connect" the instance and SSH in to a Git Bash Terminal. 
  * Make sure you organise your terminals as now we have three.
  * You can do this by **right clicking** on the terminal and select **Options**. 
* Once you have SSH into your instance, you can check that prometheus has been installed.
  * `cd /etc/prometheus/`
* This will help you navigate to Prometheus.

![alt text](./grafana-images/image-34.png)

Alternatively, you can check the Prometheus version, you can use the following command:
* `prometheus --version`

![alt text](./grafana-images/image-35.png)

<br>
