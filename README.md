# openspell client

attempt at deobfuscating and adding new features to the openspell client, to promote development on the existing client.

the highspell client seems to be written in typescript and compiled to js, which involves a lot of minification and logic obfuscation.
the first 179,000 lines are all renderer code, and aren't getting touched... works just fine as-is :)

----

### completed
- simple true/false deobfuscation to get us goin

### todo: deobfuscation
- readable class names, in line with the highlite project
  - most of the useful stuff has been defined already by highlite, but i'd like to work towards everything being legible
- readable variables (pretty huge)
  - starting with the more useful functions, or those being worked on to add new features
- comments! i love comments!!

### todo: new features
- global chat mute toggle in settings
