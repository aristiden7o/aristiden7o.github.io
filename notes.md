## documentation
http://docs.getpelican.com/en/stable/publish.html
http://docs.getpelican.com/en/stable/tips.html
https://github.com/EpicSoftworks/pelican-ghostwriter
example/inspiration: https://jacobian.org



## dev test URL

https://aristi-dev.de:8000


## commands

### develop

```
cd ~/WORKSPACES/aristide-n.github.io
git co dev
pelican -r content
cd output
python -m pelican.server
```


### publish

```
$ pelican content -o output -s publishconf.py
$ ghp-import -c aristi.de output
$ git push git@github.com:aristide-n/aristide-n.github.io.git gh-pages:master
# ghp-import seems to not want to add a new commit, so I use git push :/
```
