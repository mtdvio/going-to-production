# Serverside checklist

This is a checklist for serverside of the Web App.


## Load balancing

  [ ] My project can run on multiple CPUs
  [ ] My project can run behind the load balancer
  [ ] I can add a new node 

## Transparent deployment
  
  [ ] I can add a new node without stopping the application
  [ ] I can add a new node without user sessions being lost/destroyed
  [ ] I can make a rolling upgrades for my service

## Supervising

  [ ] My application can survive a server restart
  [ ] My application is restarted automatically after the crash
  [ ] 