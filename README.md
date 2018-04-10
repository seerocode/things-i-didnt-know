# things-i-didnt-know
Hodge podge of coding snippets that I didn't know before and have proved useful.

### How to view the processes running during a homebrew install 
#### Why: because I was running brew install postgresql and it took like a bajillion years (more than 5 hours) and I had no GD clue why. Thought it just got stuck on `make`. Turns out, a crap ton of processes were running and I just couldn't see them in the console.
`brew install -v packagename
`
