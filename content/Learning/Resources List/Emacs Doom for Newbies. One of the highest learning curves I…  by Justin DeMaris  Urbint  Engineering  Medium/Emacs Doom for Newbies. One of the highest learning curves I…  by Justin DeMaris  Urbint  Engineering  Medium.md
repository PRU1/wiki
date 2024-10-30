---
Link: https://medium.com/urbint-engineering/emacs-doom-for-newbies-1f8038604e3b
---
Good overview

![[1O1-Yh0sIgux7urNNcdgkNA.jpeg]]

One of the highest learning curves I have ever had to deal with was getting into Emacs. Thanks to all of my colleagues at [Urbint](https://urbint.com/), I’ve finally cracked the first level of concepts and am actually able to be a productive developer all within the bounds of this immense editor (or, *cough* operating system).

After spending a while struggling to build my own dotfiles from scratch, the team discovered an amazing package of configuration called Doom (a huge thank you to [Henrik Lissner](https://twitter.com/vnought) for putting it together). For any Emacs purists reading this, you can probably close the tab in disgust now. Doom is very much built around [Evil Mode](https://www.emacswiki.org/emacs/Evil) and is meant to make VI users feel at home. For anybody looking to really get started being productive with Emacs, I thought it would be helpful to compile the most common functions that I use, and how they are configured in Doom. If you are an Emacs pro and just want to learn about Doom, some of this will be repetitive, and you would probably be better served just to read the README on the Doom project, but if you are looking to started and still feel a bit lost in Emacs, hopefully this will help you out.

To get started, make sure you have [Emacs installed](https://www.gnu.org/software/emacs/download.html) and then follow the Doom installation guide: [https://github.com/hlissner/.emacs.d#installation](https://github.com/hlissner/.emacs.d#installation)

Source: Henrik Lissner — [https://github.com/hlissner/.emacs.d/tree/screenshots](https://github.com/hlissner/.emacs.d/tree/screenshots)

![[1I6svBlHhkufsMTYbC5YFUw.png]]

# Emacs Key Binding Philosophy

The three core concepts for Emacs key bindings are _**modifiers**_, _**chords**_ and _**sequences**_.

A [_**modifier**_](https://www.emacswiki.org/emacs/ModifierKeys) key is any one of the following. Anything else is a “non-modifer key”:

![[1IV-oNecF-hVgi9vInBxWZA.png]]

A _**chord**_ is made up of zero or more modifier keys pressed at the same time as a single non-modifier key. For example, “C-x” is a chord for pressing Ctrl and “x” at the same time and then releasing them. “C-s-v” is a chord for pressing Ctrl, Command (or Windows), and v at the same time.

A [_**sequence**_](https://www.gnu.org/software/emacs/manual/html_node/elisp/Key-Sequences.html) is a series of chords, pressed and released in a row. The most important command in Emacs, “C-x C-c”, is a great example of a sequence. You press “Ctrl” and “x” at the same time, then release them, then press “Ctrl” and “c” at the same time and then release them and voila, you are in the process of exiting Emacs.

**Doom Note:** Emacs has a special extension called “evil mode” that emulates a lot of vi like functionality. Doom is very strongly centered around evil mode, and a lot of the rest of this article involves using the various key bindings that are configured with it. The biggest piece is the concept of an “evil leader” which is basically a key that you press as the first step in a sequence that then opens up a new branch of possible commands. In Doom, the evil leader is set to the Space Bar by default. So, for example, to split the screen into two side-by-side windows, you would press “SPC w v”. Keep this concept of the leader key in mind as we go through practical examples.

# Setting Up Projects

If you are more familiar with IDEs like Eclipse or IntelliJ, you probably already have a concept of a project in your mind. It’s basically a folder for a particular codebase (probably under version control) that is pretty much a cohesive unit that you work on independently. In Emacs, this grouping and identification is usually managed by [Projectile](https://github.com/bbatsov/projectile). With Doom, this is installed by default.

In order to make use of this functionality with the projects that you already have, you need to let Projectile know where the projects reside. Inside of Doom, you do this by modifying the init.el inside your own custom configuration folder:

> ~/.emacs.d/modules/private/<your-user-name>/init.el

For example, my username is “jdemaris” so my folder is ~/.emacs.d/modules/private/jdemaris is my custom folder. Keeping all of your changes in here makes it safer to update the Doom config whenever new versions come out. Inside of my init.el file, I have added a number of Projectile projects:

> (projectile-add-known-project “~/Projects/playground/elixir”)
> 
> (projectile-add-known-project “~/Projects/playground/otp”)
> 
> (projectile-add-known-project “~/Projects/playground/expostal”)
> 
> (projectile-add-known-project “~/Projects/playground/benchfella”)

You should be able to make the folder and add an init.el file for yourself as well, pointing to one or two projects that you would like to be editing with Emacs.

# Opening & Navigating Projects

Once you have this in place, open up Emacs and we can try switching to the project! Once emacs is open, try executing the following sequence:

> SPC p p

That is, press space bar, release it, press p, release it and then press p again and release it. You will see a small modal slide up from the bottom, listing out the projects you defined!

[![](https://miro.medium.com/v2/resize:fit:700/1*tOzQBow5203PvlZAspZUrg.png)](https://miro.medium.com/v2/resize:fit:700/1*tOzQBow5203PvlZAspZUrg.png)

You can pick amongst them using the arrow keys, or (if you’re already familiar with some common key bindings) ctrl-j to move down and ctrl-k to move up. Better still, if you have a long list of projects to switch between, you can start typing the name to filter down the list! Once you’ve found the project that you want to work on and selected it, you can hit Enter.

This won’t open the project up directly, so don’t be surprised when you don’t see content up top yet. Instead, this will open the list of files in that project in that small modal in the bottom (called the “mini buffer”). Again, you can use the same navigation methods listed above to select the first file that you want to open. Once you’ve found the file and hit enter, you will see the file in the main window and you can get started editing on it.

[![](https://miro.medium.com/v2/resize:fit:700/1*CDYqiJhJngADI-kPBavomA.png)](https://miro.medium.com/v2/resize:fit:700/1*CDYqiJhJngADI-kPBavomA.png)

By default, the screen will be in “normal” mode, which means that it is expecting commands (just like if you opened up vi). If you hit the “i” key, it will convert to INSERT mode and you can type text as you normally would in vi. To go back to normal mode, hit the Escape key. Once you’re back in normal mode, you can navigate to other files within the same project by using the sequence:

> SPC SPC

This opens up the already familiar navigator and lets you pick another file to switch to within the same project. If you want to open a file from a different project, you can use the “SPC p p” sequence from earlier again. If you would like to switch between files that you have already opened (these currently open screens are called “buffers” in Emacs) then you can use:

> SPC ,

Evil mode emacs is so vi-esque that your old friends “:w” and “:q” are available to save and quit as well.

# Window Management and Navigation

What good is an editor if you can only have a single thing on screen at one time? Not much good, and it makes your 4k monitor cry to be so underutilized. In Emacs, you can easily split the screen horizontally and/or vertically into different [_**windows**_](https://www.gnu.org/software/emacs/manual/html_node/emacs/Split-Window.html) that contain different data. In the background, Emacs has a bunch of [_**buffers**_](https://www.gnu.org/software/emacs/manual/html_node/emacs/Buffers.html) open, one for each file you have opened to edit. When you open a window, it assigns a buffer to that window. If you happen to have the same file open in two different windows, then you are actually editing the same buffer! So if you edit the contents of one window, you’d see that change happening on all of the other windows with that same file. This can actually be super useful if you have a long file and you want to look at one part of it while you edit the other part.

So how do you create these new windows? To split your current window into two side-by-side windows with Doom, press:

> SPC w v

This will open up a split window for you like this with the same buffer open in both windows:

[![](https://miro.medium.com/v2/resize:fit:700/1*OyIGIFi32tmY0Dektz1kIg.png)](https://miro.medium.com/v2/resize:fit:700/1*OyIGIFi32tmY0Dektz1kIg.png)

You may be starting to see a pattern in these key presses. They are actually categorized! SPC is the evil leader, so it indicates that you want to execute some command. “w” is actually for the “window” category. If you forget exactly which key to press, but you can remember the category, then Doom has the plugins set up to guide you through the process. For example, pressing:

> SPC w

will open up this guidance section in the minibuffer:

![[1DMmKRCeA52Q4nT406kzd-Q.png]]

You can see that “v” executes _evil-window-vsplit_. Can you see what key to press instead of “v” if you wanted to split the window into top and bottom? I’ll give you a hint — it’s just called _evil-window-split_.

Once you have some windows open, you need to be able to move in between them. Your mouse will actually work, but that’s not very Emacs-esque. There are a few different ways, but my favorites to move around are:

[![](https://miro.medium.com/v2/resize:fit:526/1*zk7mvT1BG_LI_etrFM0t4A.png)](https://miro.medium.com/v2/resize:fit:526/1*zk7mvT1BG_LI_etrFM0t4A.png)

And what if you want to get rid of some of these windows? To close the currently selected window:

> SPC w c

You can also use Ctrl-X 0 (zero). There are a ton of other things you can do with these windows. Go through the list of options shown after pressing “SPC w” and try them out!

# File Structure Navigation (neotree)

What if you don’t quite know what your project layout looks like and you’re more comfortable seeing a tree of your file system? Fear not! [Neotree](https://github.com/jaypei/emacs-neotree) is one of the most widely used file system tree views in Emacs, and it comes preconfigured with Doom.

To open the Neotree view:

> SPC o n

You can do this from pretty much anywhere (except insert mode — so think anywhere you would be able to use :w or :q). The really great part is that this is actually a smart open! If you are not currently inside of a Projectile project, then it will start with your home folder. If, however, you already selected a project and are working in that context, it will open up the tree view of just that project.

![[18TaQ2orqNYBpX771y-VrlQ.png]]

You can use the arrow keys to move up and down on tree, or if you’re already used to it — h,j,k and l also work. Pressing ENTER on a file will open it up in the original window and move the focus of your cursor over to that window.

To create a new file in neotree so you can start editing it, press the “c” key. It will open up a dialog in the minibuffer to let you specify the path to the file. Once you are done typing the path, hit enter and it will close the minibuffer and create the file (and any parent folders) in neotree for you to select and open.

To delete a file or folder that you have selected in neotree, press:

> C-c C-d

If you are currently in the neotree window and you want to close it, you can just press the Escape key or the “q” key. “SPC w c” will still work, but escape is a lot more intuitive to me since I feel like I am closing out a temporary dialog.

# Using the terminal

Finally, what if you want to do something in the CLI that you don’t have (or don’t know) the keybinding for yet? Do you have to leave Emacs for this? Fear not!! You can open up a terminal instance right in Emacs as one of its windows. I personally find this handy for doing git-related commands since my muscle memory for git is much more tied to the CLI than to the editor.

To open up a CLI window, press:

> SPC o t

You may have gotten the idea of those categories from earlier. Since we use “SPC o t” for the terminal and “SPC o n” for neotree, you can probably guess that “o” is the category for opening popup windows.

[![](https://miro.medium.com/v2/resize:fit:700/1*WUHya8OHwNoAw_uFdvEHFg.png)](https://miro.medium.com/v2/resize:fit:700/1*WUHya8OHwNoAw_uFdvEHFg.png)

You can perform whatever CLI operations you want in here, and even use the window navigation keys to switch between your editing windows and the CLI window. Once you are done with the terminal, you can close it by pressing:

> C-x 0 (zero)

This will close it back out and return you to your normal editing.

# Conclusion

One final tip — if you are sure that a command must exist for something but you aren’t sure what it’s called, press Alt-X (or “M-x”) on your keyboard and you will get the buffer to actually type the named commands into Emacs. Each of the key sequences listed here is actually tied to essentially a function name, and you can call that function by searching for it as well. If you decide that you don’t actually want to call a function after all, you can always press Ctrl-G to cancel whatever you were in the middle of doing.

This is only barely scratching the surface of what kind of power you have available, but hopefully it can help you get over the initial learning curve and start down the path of Emacs wizardry!