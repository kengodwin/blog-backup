# OpenMonitors.com

One of the gaps in the FOSS community right now is a unified monitoring solution in a single dashboard/application that surfaces everything. I could daisy chain applications (NetData, [Healtchecks.io](http://Healtchecks.io), UptimeKuma, ClearStatus, etc.) or do something with [Elastic.co](http://Elastic.co) that covers more of the chain but still has obvious gaps.

What I want is a single dashboard application that ties into error management, status page, notifications, on-call management, incident management, real user monitoring, and synthetic uptime/SSL monitoring.

**Things I don’t want to build myself:**

Server Monitoring – There is an entire space for this and its a large undertaking to maintain.

Application Performance Monitoring – Same as the above.

Log management – The ELK stack is 3 applications for a reason. Its not worth trying to duplicate this entire setup.

Metrics at scale – Application and server metrics are a whole stack in and of itself. Its not feasible to build this.

**What this project encompasses in the long term:**

1. SSL Monitoring
    
2. Cron/Healthchecks
    
3. Synthetic Uptime (HTTP/HTTPS/Keyword/Ping/Port)
    
4. Real User Monitoring Application
    
5. Error Management
    
6. Incident Notification & Response (Various notification types, On Call Rotations, Status Page incidents, incident tracking)
    
7. Service Integrations to feed the private dashboard and hosted status page (i.e. Your CDN is down)
    
8. Hosted Status Page tying these elements together.
    
9. Private Dashboard tying these elements together.
    
    The MVP I intend to build will cover points 1 through 3. The rest will come later assuming the project is worth the time and has enough user interest.