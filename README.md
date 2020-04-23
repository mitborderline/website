# Borderline Website

This website is hosted on scripts.mit.edu. In order to update this website, the
easiest thing to do is:

- Update this Github repository with your desired changes.
- ssh to athena.dialup.mit.edu [more info](http://web.mit.edu/dialup/www/ssh.html)
- From Athena, run `ssh -k borderline@scripts` (if you have trouble with this step, it's possible that you don't have the correct permissions -- ask an administrator to give you permissions according to instructions [here](https://scripts.mit.edu/faq/58/). They should run something like `attach womenineecs; fs sa /mit/womenineecs <user> write`
- Run `git pull`.

This website also uses SASS. See [here](https://sass-lang.com/) for details. Generally you want to edit the file `stylesheets/main.scss` while running something like `sass --watch stylesheets/scss:stylesheets/`.

