# Serverside checklist

This is a checklist for serverside of the Web App.

## Legal

 - [ ] Licences of my application's 3rd-party dependencies are not violated
 - [ ] My application does not violate cryptography policies and laws  
 - [ ] My app is compliant according to the organisation standards

## Resiliency 

* [ ] My application can retain reasonable functionality in isolation
* [ ] My application can recover from being under heavy load
* [ ] My application can reestablish all lost connections
* [ ] My application can not cause Cascading Failures to propagate through the system
 
## Load balancing

* [ ] My project can run on multiple CPUs
* [ ] My project can run behind the load balancer
* [ ] I can add a new node without system downtime

## Transparent deployment
  
* [ ] I can add a new node without stopping the application
* [ ] I can add a new node without user sessions being lost/destroyed
* [ ] I can make a rolling upgrades for my service

## Supervising

* [ ] My application can survive a server restart
* [ ] My application is restarted automatically after the crash
  

## Logging

* [ ] My application logs all errors (even "swallowed")
* [ ] My application produces log output to rotated files
  * Streams with different log levels are separated from each other
  
* [ ] My logs are aggregated to a log analysing service


## Monitoring

* [ ] I have configured the alerts for abnormal activity

  * Application restart events
  * Error rate threshold reached
  * Server resources are soon to be exhausted (CPU, memory, IO > 90%)
  * HTTP requests timeouts
  * HTTP responses with 500 status codes

* [ ] I have health checks for all parts of my system


## Metrics

* [ ] I can observe different events from my app over time
  
  * Number of requests for endpoints
  * Duration of requests for endpoints
  * Duration of business-logic operations


## High Availability

* [ ] I can run my services in different independent Data Centers


## Testing
  
* [ ] I have performed stress tests for my application
* [ ] I have performed network partitioning tests for my application


## Backuping

* [ ] I can restore all my data from backups


## Security

* [ ] I have audited my system against OWASP Top 10 Vulnerabilities
* [ ] I use TLS for all endpoints
* [ ] I have added relevant security headers to app HTTP endpoints

  * `X-Frame-Options`
  * `X-Content-Type-Options`
  * `Content-Security-Policy`
  * `X-XSS-Protection`
  * `Strict-Transport-Security`
  * `Public-Key-Pins`
  * `X-Content-Type-Options`
