# openspell client

attempt at deobfuscating and adding new features to the openspell client, to promote development on the existing client.

the highspell client seems to be written in typescript and compiled to js, which involves a lot of minification and logic obfuscation.
the first 179,000 lines are all renderer code, and aren't getting touched... works just fine as-is :)

not all features require full deobfuscation to implement, if they're similar to existing features.

----

### completed
- simple true/false deobfuscation to get us goin

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
- global chat mute toggle in settings
