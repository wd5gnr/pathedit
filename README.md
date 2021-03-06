Pathedit by Al Williams (al.williams@awce.com)

Public Domain

This is a simple hack to let you edit your path with your favorite editor.

You can't run it as a script--it has to run in the current shell using "."

So you can say:

. pathedit

However, I usually alias it like this:

alias pathed=". pathedit"

It will pick up your editor from $EDITOR or $VISUAL. If you like, you can use

$PATHEDIT_EDITOR

If you want a special editor just for this tool.

You can source with the alias argument to automatically set up an alias:

. pathedit alias

####

You can also use envedit to edit arbitrary environment variables:

. envedit LD_PATH

Of course using envedit on PATH should be the same as using pathedit

####

Another technique that doesn't require any software at all is to edit your command
line useing Control+X Control+E. However, that doesn't preload your variable into the editor.
Sure, you could copy/paste, but now you are getting a pretty involved workflow over
just typing pathed.

If you prefer, use envedit2 the same way and you will get the environment
variable pushed into your command line buffer. This is a bit of a hack but
ought to work. There's also pathedit2.
