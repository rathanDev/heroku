

# replace REPLACE_ME_OS/REPLACE_ME_ARCH with values as noted below
wget https://cli-assets.heroku.com/heroku-cli/channels/stable/heroku-cli-linux-x64.tar.gz -O heroku.tar.gz
tar -xvzf heroku.tar.gz
mkdir -p /usr/local/lib /usr/local/bin
mv heroku-cli-v6.x.x-darwin-64 /usr/local/lib/heroku
ln -s /usr/local/lib/heroku/bin/heroku /usr/local/bin/heroku


wget https://cli-assets.heroku.com/heroku-cli/channels/stable/heroku-cli-linux-x64.tar.gz -O heroku.tar.gz
tar -xvzf heroku.tar.gz
sudo mkdir -p /usr/local/lib /usr/local/bin



# Run this from your terminal.
# The following will add our apt repository and install the CLI:
sudo add-apt-repository "deb https://cli-assets.heroku.com/branches/stable/apt ./"
curl -L https://cli-assets.heroku.com/apt/release.key | sudo apt-key add -
sudo apt-get update
sudo apt-get install heroku
