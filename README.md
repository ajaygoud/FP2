# Final Project Assignment 2: Explore One More! (FP2) 
DUE March 30, 2015 Monday (2015-03-30)

This is just like FP1, but where you do a different library. (Full description of FP1 is [on Piazza.][piazza])

During this assignment, you should start looking for teammates. See the project schedule [on Piazza.][schedule]

Write your report right in this file. Instructions are below. You can delete them if you like, or just leave them at the bottom.
You are allowed to change/delete anything in this file to make it into your report. It will be public.
# I have explored opening a web browser library

#For the second library exploration, I choose open a browser, this is not all that difficult to work with because we know what is a browser and where it will be opened so we just need to write some code to work on opening browser

#the main part of the code is (require net/sendurl)
send-url is used for opening a URL in the user’s chosen web browser.
send-url command works differently in different operating systems below are some  operating systems and its working 
On Windows, send-url normally uses shell-execute to launch a browser.
On Mac OS X, send-url runs osascript to start the user’s chosen browser.
On Unix, send-url uses a user-preference, or when none is set, it will look for a known browser.

(require net/sendurl)
(send-url "https://www.youtube.com/")

when I type the above code and run in the racket environment it will open browser with youtube page as output.


(send-url/file	 path )
Similar to send-url  but accepts a path to a file to be displayed by the browser.

(send-url/contents	 	contents)
Similar to send-url/file, but it consumes the contents of a page to show and displays it from a temporary file.

the above are the commands for different operations that we can do in open a browser library.


This file is formatted with the [**markdown** language][markdown], so take a glance at how that works.

This file IS your report for the assignment, including code and your story.

Code is super easy in markdown, which you can easily do inline `(require net/url)` or do in whole blocks:
```
#lang racket

(require net/url)
```

### My Library: (library name here)
Write what you did!
Remember that this report must include:
 
* a narrative of what you did
* the code that you wrote
* output from your code demonstrating what it produced
* any diagrams or figures explaining your work 
 
The narrative itself should be no longer than 350 words. Yes, you can add more files and link or refer to them. This is github, handling files is awesome and easy!

Ask questions publicly in the Piazza group.

### How to Do and Submit this assignment

1. To start, [**fork** this repository][forking].
1. Modify the README.md file and [**commit**][ref-commit] changes to complete your solution.
  2. (This assignment is just one README.md file, so you can edit it right in github without cloning)
  3. (You may need to clone and push if you want to add extra files)
1. [Create a **pull request**][pull-request] on the original repository to turn in the assignment.

<!-- Links -->
[piazza]: https://piazza.com/class/i55is8xqqwhmr?cid=411
[schedule]: https://piazza.com/class/i55is8xqqwhmr?cid=453
[markdown]: https://help.github.com/articles/markdown-basics/
[forking]: https://guides.github.com/activities/forking/
[ref-clone]: http://gitref.org/creating/#clone
[ref-commit]: http://gitref.org/basic/#commit
[ref-push]: http://gitref.org/remotes/#push
[pull-request]: https://help.github.com/articles/creating-a-pull-request

