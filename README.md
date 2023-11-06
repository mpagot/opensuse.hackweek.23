# Project page

Page is based on Jekyll. The page is rendered remotely by Github on 

## Prerequisite

On openSUSE TW (notice the **pattern install**)
```
# zypper install -t pattern devel_ruby devel_C_C++
```

Tune the environment with:
```
$ echo '# Install Ruby Gems to ~/gems' >> ~/.zshrc
$ echo 'export GEM_HOME="$HOME/gems"' >> ~/.zshrc
$ echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.zshrc
$ source ~/.zshrc
```

Install some gems (probably only *bundler* is needed)
```
$ gem install jekyll bundler
```

At this point
```
$ cd <THIS_REPO>
$ bundle install
```

## Render
In order to render the page locally:

```
$ cd <THIS_REPO>
$ PAGES_REPO_NWO=michelepagot/opensuse.hackweek.2022  bundle exec jekyll serve --incremental
```

Open your browser on [http://127.0.0.1:4000](http://127.0.0.1:4000)
