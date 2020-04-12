# url-spyder

pip install --user --upgrade pipenv

~/projects/tys-hiroshi/url-spyder$ pipenv install
Pipfile.lock not found, creating…
Locking [dev-packages] dependencies…
Locking [packages] dependencies…
✔ Success! 
Updated Pipfile.lock (e4af75)!
Installing dependencies from Pipfile.lock (e4af75)…
  🐍   ▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉ 101/101 — 00:01:00
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.

pipenv shell

pipenv install scrapy

scrapy version
scrapy 2.0.1

scrapy startproject url_scrapy

cd url_scrapy


scrapy genspider springer_spider link.springer.com


scrapy crawl springer_spider


pipenv run


exec.sh

```
#!/bin/bash

cd /home/th4/projects/tys-hiroshi/url-spyder/url_scrapy
pipenv shell
scrapy crawl springer_spider
```

chmod 755 exec.sh


30 22 * * *   th4 /bin/bash /home/th4/projects/tys-hiroshi/url-spyder/exec.sh >> /home/th4/projects/tys-hiroshi/url-spyder/log/cron.log
