# nus-tss.github.io

This website uses [Jekyll](https://jekyllrb.com).

In order to test the website locally, you can use:
```
bundle exec jekyll serve
```

The website will be hosted locally under `localhost:4000`.


## Setting up for development and update

1. Install ruby version 3.3.8 (or just version 3.3). Installation guide can be found at `https://www.ruby-lang.org/en/documentation/installation/`. After installation, run `ruby -v` in terminal to check whether ruby has been installed successfully.
2. Install bundler and jekyll with `gem install bundler jekyll`.
3. In this directory, run `bundle install` to install depedencies.
4. Run `bundle exec jekyll serve` to start the server. If everything works ok, the local website can be accessed at `http://127.0.0.1:4000/`.

Now the local setup is complete. To make changes to the website, make changes to the source code and save it. The locally deployed site should automatically reflect the change after refreshing. Sometimes bigger changes may not be automatically rendered; in this case, stop the server with ctrl-c and restart it.

After checking the changes on the local server, stop the local server with ctrl-c. Commit the changes with `git add ...` and `git commit -m "..."`. Then push the committed changes to github with `git push`. The production site should be updated with the new changes after a few minutes.
