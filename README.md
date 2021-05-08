# Setup

1. Enable WSL windows component
2. Install Ubuntu 18.04 LTS
3. Launch Ubuntu and then following this guide (https://jekyllrb.com/docs/installation/ubuntu/)
- `sudo apt-get update`
- `sudo apt-get install ruby-full build-essential zlib1g-dev`
- following commands to update your `~/.bashrc` file
```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
- `gem install jekyll bundler`

# Running
- `bundle exec jekyll build` to build
- `bundle exec jekyll serve` to serve

# Resources
- https://pages.github.com/versions/

# @applyfiles error on jekyll build
- `sudo umount /mnt/d``
- `sudo mount -t drvfs D: /mnt/d -o metadata` here D: is drive that has my globeapparels folder. specify your drive.
- `sudo chmod -R 777 /mnt/d/SH/GA/globeapparels/` or `sudo chown -R rashedul /mnt/d/SH/GA/globeapparels/` here /mn/d/SH/GA/globeapparels is path to my site. specify your path. Here rashedul is my account name. specify your account name
- Refer stackoverflow - https://stackoverflow.com/questions/57243299/jekyll-operation-not-permitted-apply2files and https://stackoverflow.com/questions/46610256/chmod-wsl-bash-doesnt-work