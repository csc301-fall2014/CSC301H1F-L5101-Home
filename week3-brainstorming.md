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

User stories:
 * As Dan, I want to access all of the course info for courses I am registered in, so that I don't have to go to different websites.
 * As Dan, I want a calendar on the homepage, so I can view all of my deadlines, and manage my TODO items in one central place. 
 * As Dan, I want to access the website from my computer, phone and tablet, because I use all of these devices throughout the day.
 * As Dan, I would like some sort of a student-only social layer in the portal, so that I can contact students (without thinking about what the profs miht say/do).
 * A discussion board.


## MVP

An online portal for University students, with convenient schedule and time management features.
Think of Blackboard, where a calendar and a TODO list are the centre of attention.


### Release Plan

Alpha testing with volunteer students in the lab (i.e Our first release is a prototype).

User Stories
 * 2 As Dan, I want to integrate my iCal/GoogleCalendar, so that I can see my personal meetings on top of school related items.
 * 3 Link to MarkUs
 * 1 Add/remove/edit events in calendar.
 * 2 Notifications and reminders
 * 1 Courses and due dates loaded automatically
 * 2 TODO List updates automatically to reflect changes in the calendar.
  

Only items with priority 1 will make it to our first release.


## Architecture

 * Web server to serve web pages.
   * Which server?
   * It's going to server web pages.
   * It's also going to serve data (for AJAX calls)
 * Front end (i.e. HTML + CSS + JavaScript)
 * Persistent data storage

 


