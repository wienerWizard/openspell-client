# openspell client

attempt at deobfuscating and adding new features to the openspell client, to promote development on the existing client.

the original highspell client seems to have been written in typescript and compiled to js, which involves a lot of minification and logic obfuscation.
the first 180k~ lines are renderer code, and won't be touched... works just fine as-is :)

not all features require full deobfuscation to implement, if they're similar to existing features.

----

### completed so far
- light deobfuscation: some low-hanging class names, functions, etc
- global chat mute toggle in chat settings
    - could be better... global messages get completely discarded when setting enabled, unlike the highlite plugin which only temporarily hides them...

### todo: deobfuscation
- readable class names
  - most of the useful stuff has been defined already by the highlite project, but i'd like to work towards everything being legible
  - many verbose errors in code already state the name of their parent class which is nice
- readable variables
  - starting with the more useful functions, or those being worked on to add new features
  - most will need to be implied or remain vague
- cleaner logic
  - convert weird && and || operations into equiv if() else{} statements
  - clean up the billions of redundant commas
- comments! i love comprehending!!

### todo: new features
- better global chat mute
  - maybe the toggle adds a css rule to temporarily hide global messages instead...
