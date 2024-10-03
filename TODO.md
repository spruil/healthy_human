# TODO 🚧


git config receive.denyCurrentBranch ignore
    2  nano .git/hooks/post-receive
    3  chmod +x .git/hooks/post-receive
    
    setup
Has conversation started by @spruil. Original line has conversation started by @spruil.
    $ cat .git/hooks/post-receive
#!/bin/bash
unset GIT_INDEX_FILE
git --work-tree=/app  --git-dir=/app/.git checkout -f
refresh 




Your new site is all yours so it doesn't matter if you break it! Try editing the code–add a button element that moves when the user clicks it.

In `index.html`, add this code on the line after the comment with `ADD BUTTON HERE` in it (you can copy and paste the button element HTML):
$ cat .git/hooks/post-receive
#!/bin/bash
unset GIT_INDEX_FILE
git --work-tree=/app --git-dir=/app/.git checkout -f
refresh

app@healthyhuman:~ 05:59
$ ls -a
. .bash_history .git .glitch-assets index.html .nano script.js TODO.md
.. .data .github .glitchdotcom.json LICENSE README.md style.css

app@healthyhuman:~ 05:59
$ cat .github/workflows/main.yml
on: push
jobs:
git-sync:
runs-on: ubuntu-latest
steps: - name: git-sync
uses: wei/git-sync@v3
with:
source_repo: "https://github.com/spruil/healthy_human.git"
source_branch: "main"
destination_repo: ${{ secrets.glitch_git_URL }}
destination_branch: "main"

```$ cat .git/hooks/post-receive
#!/bin/bash
unset GIT_INDEX_FILE
git --work-tree=/app  --git-dir=/app/.git checkout -f
refresh

app@healthyhuman:~ 05:59 
$ ls -a
.   .bash_history  .git     .glitch-assets      index.html  .nano      script.js  TODO.md
..  .data          .github  .glitchdotcom.json  LICENSE     README.md  style.css

app@healthyhuman:~ 05:59 
$ cat .github/workflows/main.yml 
on: push
jobs:
  git-sync:
    runs-on: ubuntu-latest
    steps:
      - name: git-sync
        uses: wei/git-sync@v3
        with:
          source_repo: "https://github.com/spruil/healthy_human.git"
          source_branch: "main"
          destination_repo: ${{ secrets.glitch_git_URL }}
          destination_branch: "main"
```

Look at the page to see the button. Click it!

Open `script.js` to see the script that makes the button move.

## Keep going! 🚀

Try adding more properties to the CSS `dipped` style for the button to see how the changes appear on click.
