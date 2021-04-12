# HomeEnergyUsage

Hardware Needed
Emporia Vue 2  ~ $100
Raspberry Pi ~ $40



The first thing to do is to get a 

Step 2: Get your raspberry pi running with HomeAssistant & Prometheus on it. Follow this blog post if you want to use Homeassistants OS on your Raspberry Pi (https://www.home-assistant.io/installation/raspberrypi/) or you can use Raspberry Pi OS and download docker & docker-compose.

Step 3: 

Setting up Grafana Cloud
The next step is to set up our databases and Grafana. I have decided to use Grafana Cloud — which comes with hosted Grafana, Grafana Loki, and Graphite — for our data storage and data visualization. The free tier comes with 10,000 series for Graphite metrics and 50GB for logs in Loki, which is definitely more than enough for this monitoring solution. 

I went to the Grafana Cloud signup and created a new account. As soon as I had my account all set up, I could see my portal with my hosted Grafana, Loki, and Graphite instances.




Step 3: Download and edit my prometheus.yml config file with your Grafana Cloud Metrics configuration for remote w

Step 4: Use the docker-compose.yml file to boot up HomeAssitant & Prometheus. 

Next, I had to install the Emporia Vue onto my circuit breaker. This was actually very easy and as long as you take your time doing so it is very safe. The emporia app on your phone walks you through how to do it and shows you all safety instructions, as well as will refer you to an electrician to help you get it installed if you don't feel comfortable doing it yourself!
Now that we have our devices setup we need to connect the Emporia Vue to the HomeAssistant application. To do this we follow the instructions from the website here. Next we go to HomeAssistant and search for the emporia vue integration. You login with the same credentials as your emporia vue app and it should connect right away!
