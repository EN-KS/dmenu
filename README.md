This is my dmenu setup, version init

#Add shellscript to dmenu and if not show
From the ArchWiki article:

dmenu will look for executables in the directories defined in your $PATH.

You might've done something wrong if you included it in your path and it's not working.

Try echo $PATH > ~/path.txt to check if it's really there

Also, from the same article:

If certain entries are missing from dmenu, the cache may be malformed. Delete it and restart dmenu.

rm ~/.dmenu_cache

rm ~/.cache/dmenu_run
