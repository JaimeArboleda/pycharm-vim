# An opinionated set of configurations and settings for using vim and pycharm
## Why vim and PyCharm?

Vim is a very powerful text editor, that makes the physical act of writing, navigating through and refactoring code both fun and fast. Once learned (and it takes some time to learn it properly) it becomes a very natural way of interacting with text files.

If you are curious about vim there are many books, blog posts, youtube videos, tutorials etc. to get some information. In my opinion, one of the best intro videos I've ever seen, that is informative and motivating, is this [one](https://www.youtube.com/watch?v=wlR5gYd6um0).  

However, vim is not a fully fledged IDE. It's a text editor that interacts very well with the terminal and with command line applications. Sure, with the help of plugins it's possible to create an IDE-like experience (there are distributions of vim, like spacevim, that attempt to do that), but, as far as I know, they are not yet fully mature. Some tasks, like debugging and navigating through source code (including code that does not belong to the project, like the source code of the installed packages in a Python virtual environment) will be better handled by an IDE like PyCharm. I am not advocating for the use of PyCharm, but it always has been my editor of choice for writing Python code, and I think it is a very good IDE. 

Most importantly, there is a plugin called *ideavim* that emulates most vim functionality inside PyCharm, and even more, because it makes it possible to integrate vim key bindings with actions of the IDE, which is, in my opinion, a great feature. For me, as a vim neophyte and as a PyCharm enthusiast, this plugin is a match created in heaven. I cannot express how much I love it and how much it has enhanced my daily user experience as a Python developer. However, I recognize that it's still under development, and that some issues need to be fixed and some vim features need to be added. But, as it is, it can improve the coding experience.   

After justifying the use in conjunction of both tools, I will review my configuration step by step.  

## Keyboard configuration

Let's start with the most basic aspect: the keyboard. I am not going to talk about mechanical keyboards and so on (I think a cheap keyboard can be good enough for most people). I just want to say two things that are very important in order to get the most out of vim: 
- **Touch Typing**. Vim commands require the use of lots of letters and symbols of the keyboard, and if you need to look at the keyboard when typing, it will be a tiresome experience. The ideal situation is to master (I mean, to type fast and without looking at the keyboard) all ascii symbols, and the usefulness of this knowledge applies, of course, way beyond vim. This [resource](https://docs.google.com/document/d/1D9hzmKMCWzbqIBqpA4j02a2XjuhJbILimBMAFM2Deis) has been very useful for me in the journey of practising all keys and gaining speed and accuracy.  
- **Good keyboard layout**. I am spanish and I grew up using a spanish keyboard layout. However, I have been using recently US keyboards (with QWERTY layouts) and the coding experience is way better. Lots of important symbols (brackets, curly braces and many others), which in the spanish keyboard require the use of <kbd>ALT Gr</kbd>, are more easily reached in the US layout, requiring only <kbd>⇧ Shift</kbd>. So I would recommend using the US layout for coding, and, in order not to lose the special characters of spanish (or another language if you happen to be french, german or from another country that uses special non-ascii symbols), you can follow the steps described below. 

### OS-level key remapping 
I discovered that a very good way of changing the default behaviour of the keyboard is to perform some remappings that operate globally, instead of [AutoHotkey](https://www.autohotkey.com/)

You can find the script that runs in my PC in the file "keyboard.ahk" of the repository. 

## PyCharm configuration

In addition to install the plugin of IdeaVim and follow the instructions located in the official repository (in particular, how to install other vim plugins emulated), I tweaked the original keymaps to reduce conflicts and make some of the shortcuts clearer and more easy to memorize. 

You can find the settings and import them in the file "settings_keymaps.zip" of the repository. It only includes settings related to keymaps, so importing them should have no side effects. However, it is a good practice to export your current settings before doing that, to have a backup in case of need. 

## Vim Configuration

I have divided my configuration into two files, ".vimrc" and ".ideavimrc". It is documented. However, I will try to update the repository with more detailed instructions about how to use those configurations. You will need to change the absolute path of your home directory in both files. 
