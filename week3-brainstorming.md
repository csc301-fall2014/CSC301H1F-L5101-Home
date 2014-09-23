## Initial Discussion

 * Do you have any technical background?
   * No
 * Who is it for? Students, teachers?
   * Not sure, for now, let's say both.
 * What is bad with the current system?
   * Everything
   * User exeprience is not great. (too many clicks to get where you're going)
   * No mobile website (but there is an app)
   * Hard to find what you're looking for.
   * On-line assignment submission is buggy.
   * No integration with external resources (e.g. websites not on the current system)
   * Features that nobody uses (e.g. group voting)
   * Slow loading
   * Bad notification centre.
   
   
-----

## Personas

 * [Dan The Commuter](https://docs.google.com/presentation/d/17jIrffuu78dUq_fd4ukuH9L3xPvWo3TN2b28jYHhILA#slide=id.g476953abc_091)
 
 * Rez Clare 
   * 20 years old, from West Toronto.
   * Sexual Diversity studies
   * Lives in the residence building at New College.
   * Usually wakes up late, works as a bartender twice a week on College St.
   * When she's not working, she usually hangs out with friends, and play the Ukulele.
   
 * Joey from Korea
   * 24 years old, from Korea.
   * M.Ba student in Eco
   * Lives in an apartment near campus with a roommate, cat and a fish.
   * Enjoys Kareoke, online games, archery.
   



## Desinging our MVP

We will focus on *Dan the commuter*.

Come up with some user stories:
 * As Dan, I want to access all of the course info for courses I am registered in, so that I don't have to go to different websites.
 * As Dan, I want a calendar on the homepage, so I can view all of my deadlines, and manage my TODO items in one central place. 
 * As Dan, I want to access the website from my computer, phone and tablet, because I use all of these devices throughout the day.
 * As Dan, I would like some sort of a student-only social layer in the portal, so that I can contact students (without thinking about what the profs miht say/do).
 * A discussion board.

Based on the stories we came up with, we'll decide on our MVP.

## MVP

An online portal for University students, with convenient schedule and time management features.
Think of Blackboard, where a calendar and a TODO list are the centre of attention.


### Release Plan

Alpha testing with volunteer students in the lab (i.e Our first release is a prototype).


Let's write some user stories (or features), and prioritize them:
 * I want to integrate my iCal/GoogleCalendar, so that I can see my personal meetings on top of school related items. (_med_)
 * Link to MarkUs  (_low_)
 * I want to add/remove/edit events in my calendar, so that I can manage my personal schedule and my school schedule at one place. (_high_)
 * I want to get notifications and reminders about important announcements and nearby deadlines, so that I don't miss anything important. (_med_)
 * I want my courses and deadlines to appear automatically in my calendar, so that I don't have to keep track of them myself. (_high_)
 * I want to view some of my calendar items in a TODO List, because it helps me plan my day. (_med_)
  

Only items with high priority will make it to our first release.


**NOTE:** Look at [this picture](http://keremkosaner.files.wordpress.com/2008/04/softwaredevelopment.gif) again, and compare it to our process - We started with a client saying "I want an online university portal", and ended up deciding to build a "student time management tool".    
Whether we made a good decision will remain an open question until we get students to use our product. Our goal is to release (a useful product) as soon as possible - Even if we're completely off, at least we'll discover it early (i.e. _fail fast_).


## Architecture

We didn't have time to go into enough details, but we identified the 3 main components

 * Web server
   * Which server?
   * It's going to server web pages.
   * It's also going to serve data (via AJAX calls)
 * Front end (i.e. HTML + CSS + JavaScript)
 * Persistent data storage

 


