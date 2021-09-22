# Sumlight-Lab

[sumlight-lab.com](https://www.sumlight-lab.com/)

## Install Sumlight-Lab

### Clone the repository

#### Clone with SSH

```ruby
git@gitlab.com:mistd/matchingsite/sumlight-lab.git
```
or

#### Clone with HTTPS
```ruby
https://gitlab.com/mistd/matchingsite/sumlight-lab.git
```

### Check your Ruby version

```ruby
ruby -v
```

The ouput should start with something like `ruby 2.7.0`

If not, installing Ruby with Using rbenv:

Run command
```ruby
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install 2.7.0
rbenv global 2.7.0
ruby -v
```

### Check your Rails version


```ruby
rails -v
```

The ouput should start with something like `rails 6.0.3.4`

If not, installing Ruby with Using rbenv:

Run command
```ruby
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y nodejs
 
gem install rails -v 6.0.3.4
rbenv rehash
rails -v
```

### Install dependencies

Run command
```ruby
bundle && yarn
bundle install
yarn install
```

### Initialize the database

```ruby
rails db:create 
rails db:migrate 
rails db:seed
```
or

```ruby
rails db:migrate:reset
rails db:seed
```

## Serve

```ruby
rails s
rails server 
```
