# Google Code Directory Structure & other notes #

Google Code is basically setup, and I have added you all as owners. TortoiseSVN is incredibly easy to use from what I have seen, and if you want to use SVN on a linux box you can lookup how to do it there as well (there are a few GUI's and you can always go at it from the terminal).

Here is a link to it: http://code.google.com/p/cop-ginrummy/

So here is how I am imagining our structure, and if you click the source tab you can follow along pretty easily.

**branch** - In branch I expect us to post any major releases. As this isn't really a huge project, basically I expect us to create different release versions based on the addition of new features. For example, we might create a Gin Rummy simulation but not have any AI developed for PC players, in which case we could release the simulation as a release, and in a future release add the AI.

**branches** - In branches I would like to post fixes to our releases in the branch. Say for instance Aces aren't being displayed properly on REL-1.0.0 we could post bug report online, say it gets BugID 0001, and then release it in branches as BUG-0001. This will allow us to test all bug fixes before committing them into the next release in branch. For instance, after we all tested BUG-0001 with our code to make certain it doesn't break anything else while fixing the bug, we could then add REL-1.0.1 with the fix into branch.

**trunk** - This is the branch in which we all develop our code. Everyone has a folder that uses their first name, and you can structure it however you want.  The big thing with this section is that this code is always considered to be in development, and doesn't require a version number. Obviously if we release a new version everyone should make certain the code they are developing with is adding upon the latest release version.


I'm not 100% certain how you want to structure the Wikis or documentation but we have several options. For one, everyone could document their code and include it in their directory in trunk, and then when we have a release we can merge everyone's code that is being included as well as the documentation for it. This would allow everyone to document their code however they desire, with word, notepad, etc. This also frees up Wikis for communication. If everyone reads the latest Wiki pages and we post relevant notes from meetings (online and in person) this will allow us to retain all of the information in one online location.

Also, if you setup your SVN correctly (that is you set it up to download the entire SVN directory, not just trunk like the tutorial I linked directs you to) you can update your local machine with the entire SVN directory, which would include local backups of all the Wikis and everyone else's code. Since each of us should be the only people in our own directory, our local code should never be overwritten by the update, but everyone else's directory will be updated.

**Some other features that will be helpful:**
Google code seems to store several revisions of code, so committing your code frequently can mean that you have several versions to look back on in case you find out a change you made caused issues.

Along with storing several revisions, it also has an online Diff tool that shows you the difference between different versions of code.. but I would strongly suggest that you all get a diff tool of your own liking to use on your pc. They are incredibly helpful when checking to see what another team member changed in bug fixes etc, and speed the merge process up a great deal.

For examples of the stored revisions and diff tool you can goto the Examples directory under trunk. I tossed a simple file in there and then updated it to test it out quickly.


If any of you don't know how to use TortoiseSVN or want help setting it up just let me know. I set this all up with it simply to get a feel for how it works since I'm guessing most of you will be using a Windows environment.  Sorry for the long rant-like email, but hopefully you are all content with using Google Code as I am really hoping to be able to use something online that allows me to develop on my Linux machine. We are required to provide makefiles and to compile in gcc, so I never have seen the purpose of developing in Windows only to turn around and make certain that it works in linuxland.


Any comments/feedback would be appreciated. I'm not really certain where you all stand on this solution to project management, or if you all had something different in mind, but I wanted to let you see what this would be like prior to making a decision.



Jon Calhoun