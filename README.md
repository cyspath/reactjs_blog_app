
### Setting Up

#### React
gems to get started:
* gem 'therubyracer', platforms: :ruby
* gem 'react-rails', '~> 1.0'

application.js
```//= require react
//= require react_ujs```

Environment:
```config.react.variant = :development```
```config.react.variant = :production```

File tree:
app/assets/javascripts/components/components.js
``//= require_tree ./components```

#### Rails

installing gems:
in case rubyracer does not install, use this
```brew install homebrew/versions/v8-315
brew link --overwrite v8-315 --force
gem install libv8 -v '3.16.14.13' -- --with-system-v8
gem install therubyracer -v '0.12.2' -- --with-system-v8```


Scaffolding
rails g resource Post title:string author:string contents:text
rails g scaffold Post title:string author:string contents:text
