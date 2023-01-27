# Week 2 - Friday Retrospective

### This Week

1. Rewrote the monitoring script from golang to python.
    
    * Ran into a bug created by my mistake. Easily fixed, but the fact I wouldn't notice for 24+ hours is a problem in my view. Python works better for me in this case.
        
    * Fixed a design flaw unrelated to the language since I will now need to run several python scripts in place of 1 go binary. Proper queueing in MySQL may not be the most efficient but it limits stack complexity for HA purposes.
        
        * This will need more testing to be certain it's working correctly.
            
    * It's pretty clear the time-consuming factor is going to be the website and related API. The monitoring itself is pretty straightforward for the MVP options (SSL/Port/Ping/Http/Keyword).
        
        * It is kind of useless without an interface/alerting/etc but that comes later.
            
2. Researched options for the website itself. SaaS templates vs. SaaS frameworks vs. Scratch
    
    1. Probably going with Django and from Scratch given my choice to AGPL the source. Another learning experience, but I probably should stick with one language for the project if I can. Even if I probably won't be great at it. Learning is part of the game.
        
    2. If I am learning too slowly, I'll just do something in PHP.
        

### The future

1. Moving plans were delayed due to factors outside of my control. Retrospectives will probably vanish during the move once I do move.
    
2. I'm still limiting myself to 10 hours a week. Not a fast pace by any means but with moving and everything else I've got going on its what I can afford in terms of time.
    
    1. I didn't even spend that this week because of the packing and such.
        
3. 400hrs/project on top of maintaining two others at the pace I'm going is probably too ambitious. I think I'm going to adjust my thinking to 18 months per project or 2 projects every 3 years. That gives a project 3 years to gain traction before being dropped.
    
    1. 400hrs towards the new project
        
    2. 300hrs towards maintaining the previous project
        
        1. Customer support needs to be outsourced if the project scales at all. Otherwise, I'll have no time.
            
        2. I'm settling on [Fider](https://github.com/getfider/fider) to provide something resembling community support for non-paying accounts. Also for general feedback.
            
        3. I kinda have to provide at least e-mail support for paying accounts.
            
    3. At the end of 18 months, drop the old project and start a new one if needed. If something has traction, prioritize that project.
        
4. I'm leaning towards some limited paid QA to prep things for beta and possibly to test releases after beta. I'm not sure how much I can realistically budget for this given I've only got a budget for marketing and hosting. But quality matters so maybe it's worth downsizing the marketing budget some.
    
5. I'm probably going to be releasing code exclusively under the AGPL. Technically, it won't stop copycats that are solo pirate types but it should keep legitimate companies from simply copy-pasting the code into their service without providing their code changes.
    
    1. The logic here is people who want to self-host should self-host. It provides some certainty that if I shut a product down, the community can maintain it if it matters to them. That insurance should keep people from feeling locked into the service as well.
        
    2. Realistically, I will need help with the code. A 100hrs handling of pull requests will get these projects a lot further than 100hrs of me building and testing code on my own. No idea if I will get any help, however.
        
    3. Integration should be done via talking to the API with your code silo'd separately rather than directly modifying the source to prevent the viral nature of the AGPL from being a problem. That said, using this to bypass the AGPL'd code (i.e. rewriting the front end completely) would be just as much work as building your own service. So the moat remains intact.
        

### Musings

In other news, I've started pre-writing these during the week in Obsidian and just copy/pasting them to hashnode. Seems to work with some light editing via grammarly.