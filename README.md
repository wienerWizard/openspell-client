# openspell client

attempt at deobfuscating and adding new features to the openspell client, to promote development on the existing client.

the original highspell client seems to have been written in typescript and compiled to js, which involves a lot of minification and logic obfuscation.
the first 180k~ lines are renderer code (babylon.js), and won't be touched... works just fine as-is :)

not all features require full deobfuscation to implement, if they're similar to existing features.

ultimate goal is to add vanilla-esque features, and open the way to making future changes easier.

---

### how to test with this client
1. open your webbed browser of choice and navigate to openspell dot dev slash play, pick a world
2. open dev tools (f12) and go to the debugger
3. find the vanilla client.61.js, right click, select "add script override"
- <img width="274" height="211" alt="image" src="https://github.com/user-attachments/assets/d6590095-943b-407e-8d49-98ae130a6fbb" /> (here's what it looks like in firefox)
4. save the file somewhere safe. this is the vanilla client we'll be overwriting.
5. download client.61.js from this repo
6. delete vanilla file, drop the new file in its place
7. reload the page
8. wa la

----

### completed so far
- light deobfuscation: some low-hanging class names, functions, etc
- chat mute toggles in chat settings, to temporarily hide global/private/public chats 
- taller bank toggle in main settings, to make bank take up more space on bigger screens

### todo: deobfuscation
- readable class names
  - most of the useful stuff has been defined already by the highlite project, but i'd like to work towards everything being legible
  - many verbose errors in code already state the name of their parent class which is nice
  - deobfuscation will p much just happen naturally as i explore more of the code and need to understand vanilla to add my own stuff
- readable variables
  - starting with the more useful functions, or those being worked on to add new features
  - most will need to be implied or remain vague
- cleaner logic
  - convert weird && and || operations into equiv if() else{} statements
  - clean up the billions of redundant commas and semicolons
- comments! i love comprehending!!

### todo: new features
- remember "toggle minimap" setting so i don't gotta keep toggling it on login
- some better way to actually use this file in a browser without having to do the js override thing
