# Journal
Daniel Standage  
August 2014

Several years ago I used a full-fledged MVC framework to write myself a very simple personal journal application that I ran locally on my laptop.
Given how quickly these frameworks evolve, I was several versions behind when my laptop gave out.
It seemed like I had two options if I wanted to keep using the app: load an outdated version of the framework onto my fresh new laptop, or dig through examples/documentation to teach myself the new templating scheme, ORM syntax, etc, etc.
Neither of these options seemed appealing, and being busy with other things my journal simply fell by the wayside for 2 years.

In the mean time, I was introduced to static site/blog generators and have used them for documentation in my research.
These too seem to evolve pretty quickly, but they are much more lightweight and the core functionality seems stable enough.
Now that I'm eager to reboot my journal, I figured the popular Jekyll platform would be a good choice.
Finding a simple theme was effortless, and I had the journal configured in minutes.

Github makes it easy to host static pages, but I'm not interested in my journal being accessible anywhere other than my laptop.
It's not that my journal contains any *sensitive* or *incriminating* information, just private information that I would like to remain private.
At the same time, I would like to use version control and host a backup of my journal online so that I don't fall into the same trap that I did the last time I needed a computer upgrade.
My solution is to exclude the unencrypted **_posts** directory from the git repository, storing instead a 2048-bit RSA-encrypted archive of the directory (generated automagically by a git pre-commit hook).

Only time will tell, but I'm hoping that for this iteration of my electronic personal journal that the framework that does less is the framework that does more!