# things-i-didnt-know
Hodge podge of coding snippets that I didn't know before and have proved useful.

#### How to view the processes running during a homebrew install 
**Why:** because I was running brew install postgresql and it took like a bajillion years (more than 5 hours) and I had no GD clue why. Thought it just got stuck on `make`. Turns out, a crap ton of processes were running and I just couldn't see them in the console.

```
brew install -v packagename
```
#### How to change the remote url for a repo
**WHy:** I jump between org repos so sometimes I need to push as a different user and not as myself. To do this, I clone repos using HTTP because it prompts me for username and password - what I want. Other times, I need to push as myself for my own repos and I should be able to authenticate with my own username and password when I push but I use 2FA so that won't work. This forces me to change the remote URL for the repo to SSH so I can be prompted for my key instead.
Link here: [https://help.github.com/articles/changing-a-remote-s-url/](https://help.github.com/articles/changing-a-remote-s-url/)
