# Octopus Energy Monitoring with Grafana 

I had a simple project in mind: creating a system to track energy usage and costs, and displaying them on a dashboard. To make it happen, I used a few tools:

* Grafana: Used this for displaying the data nicely on dashboards. 
* MySQL: This allowed me to store all the energy data and the costs so that I can use it in Grafana.
* Python: With this I used it to connect to my energy supplier API and pull the energy consumption for my account.
* DigitalOcean - While optional I used it to deploy everything on a VM but this can be avoided and can be setup locally.

By combining these tools, I successfully built a simple script for monitoring and analysing energy consumption.

**To Do:**
*  Fix the issue with the widget that shows the price for the next 30 minutes 
*  Fix the issue with the estimate - I'm just using average here 
* Connect to Tesla API and charge the car when the price drops. 
* Pull data from LightwaveRF to see each device usage at home.

Here is an overview of the dashboard that shows the consumption

![Model](https://github.com/fjosef1/octopus/blob/main/Overview.jpg)

This dashboard is showing the tracked cost
![Model](https://github.com/fjosef1/octopus/blob/main/Cost.jpg)
