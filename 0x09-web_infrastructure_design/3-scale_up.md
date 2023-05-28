# Scaled Up Web Infrastructure

<p align="center">
  <img src="https://github.com/KBryt/alx-system_engineering-devops/blob/master/0x09-web_infrastructure_design/3-scale_up.PNG"
       alt="dashboard logo"
       width="750"
  >
</p>

## Description

This web infrastructure is a scaled up version of the infrastructure described [here](2-secured_and_monitored_web_infrastructure.md). In this version, all SPOFs have been removed and each of the major components (web server, application server, and database servers) have been moved to separate GNU/Linux servers. The SSL protection isn't terminated at the load-balancer and each server's network is protected with a firewall and they're also monitored.

## Specifics About This Infrastructure

+ The addition of a firewall between each server.<br/>This protects each server from unwanted and unauthorized users rather than protecting a single server.

## Issues With This Infrastructure

+ High maintenance costs.<br/> If each major components are moved to it own server, more servers would have to be bought leading to an incrase in the company's electricity bill along with the introduction of new servers. Some of the company's funds would have to be used to buy the servers and pay for the electricity consumption needed to keep both servers (including the new and old ones) running.
