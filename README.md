# Build your own ruby gem!

#### "Geminate: the gem I made to teach you how to build your own gems!"

## Fork this repository by clicking 'fork' at 

https://github.com/un5t0ppab13/geminate

#### lib/geminate.rb

    class geminate
    	def self.how
    		puts "Geminate: the gem I made to teach you how to build your own gems!"
    		puts "Learn how at: https://github.com/un5t0ppab13/geminate"
    	end
    end

#### geminate.gemspec

    Gem::Specification.new do |s|
      s.name        = 'geminate'
      s.version     = '0.0.0'
      s.date        = '2016-05-05'
      s.summary     = "geminate!"
      s.description = "Geminate: the gem I made to teach you how to build your own gems!"
      s.authors     = ["un5t0ppab13"]
      s.email       = 'devbrights@gmail.com'
      s.files       = ["lib/geminate.rb"]
      s.homepage    = 'http://rubygems.org/gems/geminate'
      s.license     = 'MIT'
    end

`gem build geminate.gemspec`
  
    Successfully built RubyGem
    Name: geminate
    Version: 0.0.0
    File: geminate-0.0.0.gem

`gem install ./geminate-0.0.0.gem`

  	Successfully installed geminate-0.0.0
  	Parsing documentation for geminate-0.0.0
  	Installing ri documentation for geminate-0.0.0
  	Done installing documentation for geminate after 0 seconds
  	1 gem installed

#### Start pry or irb

`pry`

`irb`
  
#### Require your new gem library

  `require 'geminate'`

#### List all method you defined in your Class (aka gem)

  `Geminate.methods(false)`

#### Call a method in your Class (aka gem)

  `Geminate.how`

#### Create an account at:

https://rubygems.org/api/v1/api_key.yaml

#### Sign in with your username and password
and save the yaml file into: ~/.gem/

#### On any Nix system:

`mv ~/Downloads/api_key.yaml ~/.gem/api_key.yaml`

## PUBLISH WITH:

`gem push geminate-0.0.0.gem`

  	enter your username
  	enter your password


#### List your gem:

`gem list -r geminate`

#### Once setup, save and push those changes:

    gem build geminate.gemspec
    gem install ./geminate-0.0.0.gem
    gem push geminate-0.0.0.gem
    gem list -r geminate

## Give us a star if you enjoyed building your own gem!
