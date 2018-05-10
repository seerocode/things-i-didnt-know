# things-i-didnt-know
Hodge podge of coding snippets that I didn't know before and have proved useful.

#### How to view the processes running during a homebrew install 
**Why:** because I was running brew install postgresql and it took like a bajillion years (more than 5 hours) and I had no GD clue why. Thought it just got stuck on `make`. Turns out, a crap ton of processes were running and I just couldn't see them in the console.

```
brew install -v packagename
```
#### How to change the remote url for a repo
**Why:** I jump between org repos so sometimes I need to push as a different user and not as myself. To do this, I clone repos using HTTP because it prompts me for username and password - what I want. Other times, I need to push as myself for my own repos and I should be able to authenticate with my own username and password when I push but I use 2FA so that won't work. This forces me to change the remote URL for the repo to SSH so I can be prompted for my key instead.

Link here: [https://help.github.com/articles/changing-a-remote-s-url/](https://help.github.com/articles/changing-a-remote-s-url/)

#### How to hide API keys and secret info in github using .gitignore (Python version)
**Why:** Because I needed to hide the API key for my threeinthree web app but still be able to push the app to heroku and have it work successfully. 

Link here: [http://www.blacktechdiva.com/hide-api-keys/](http://www.blacktechdiva.com/hide-api-keys/)

#### pip install for virtualenv when you have spaces in your file path
**Why**: The person who built my laptop (it was free) created my profile using a space between my first and last name. AGHHH!!! I know you're not supposed to do that but if you have never developed an application and had to redo the entire thing because you used a space instead of a -, then you wouldn't know not to do this.

If this happens to you, you can go into ```bin/pip``` files and change the file path to add backslashes where there's a space but that didn't work for me. This did:

```
python -m pip install packagename
```
