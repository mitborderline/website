# Borderline Website

This website is hosted on scripts.mit.edu. In order to update this website, the
easiest thing to do is:

- Update this Github repository with your desired changes. [git workflow ref](https://gist.github.com/blackfalcon/8428401#commit-your-code)
- ssh to athena.dialup.mit.edu [more info](http://web.mit.edu/dialup/www/ssh.html)
- From Athena, run `cd /mit/borderline/web_scripts` (if you have trouble with this step, it's possible that you don't have the correct permissions -- ask an administrator to give you permissions according to instructions [here](https://scripts.mit.edu/faq/58/) and [fsr reference](http://kb.mit.edu/confluence/pages/viewpage.action?pageId=3907138). They should run something like `attach borderline; add consult; fs sa /mit/borderline <user kerb> all`
- Run `git pull`.
