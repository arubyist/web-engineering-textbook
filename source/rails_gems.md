Some Gems for Rails 
===========================

This guide lists a few valuable gems for
your first Rails Project.

After reading this guide you will

* know how to install and use a gem
* know some gems
* know where to find more gems

------------------------------------------------------------

Installing
----------

Gems are ruby packages, they are the preferred unit of code reuse in ruby.
You can install them using the command line tool `gem`:


``` shell
gem install devise
```

In a Rails project you should let bundler do the work: you just add the
gem to the `Gemfile`, and then run

``` shell
bundle install
```

Bundler will resolve version conflicts between the gems for you and 
install and use a set of gems that will work well with each other.


A word of warning: some gems are not written exclusively in ruby,
they may contain C code and use C libraries. From the [RubyGems Guides](http://guides.rubygems.org/gems-with-extensions/):

> Many gems use extensions to wrap libraries that are written in C with a ruby wrapper. 
> Examples include nokogiri which wraps libxml2 and libxslt, pg which is an interface 
> to the PostgreSQL database and the mysql and mysql2 gems which provide an interface to the MySQL database.


Some Gems
----------

This list is based on [Dwellables statistics on the Rails Rumble 2013](http://www.dwellable.com/blog/Rails-Rumble-Gem-Teardown).


### Mixins

You don't want to waste your time writing vendor-prefixes for css3 features.
Use a mixin library instead:

![bourbon screenshot](images/gem-bourbon.png)
[http://bourbon.io/](http://bourbon.io/)

### CSS Grid 

Bootstrap is used by a lot of projects. See [Kehoe(2013)](http://railsapps.github.io/twitter-bootstrap-rails.html) for help
with choosing the right bootstrap gem.

But there is a more sophisticated alternative to bootstrap: **Neat** uses a *semantic* grid system:


![neat screenshot](images/gem-neat.png)
[http://neat.bourbon.io/](http://neat.bourbon.io/)


### Testing

[factory_girl](https://github.com/thoughtbot/factory_girl) for creating test data.

[capybara](https://github.com/jnicklas/capybara) as the "browser" for acceptance tests, with
[poltergeist](https://github.com/jonleighton/poltergeist) for testing client side javascript.


### File Upload

[carrierwave](https://github.com/carrierwaveuploader/carrierwave) or
[paperclip](https://github.com/thoughtbot/paperclip)

### Authentication

[devise](https://github.com/plataformatec/devise) for login,
[omniauth](https://github.com/intridea/omniauth) to integrate authentication methods.

[cancan](https://github.com/ryanb/cancan) if you need roles and permissions [sceencast](http://railscasts.com/episodes/192-authorization-with-cancan?view=asciicast).



### Sending Mail

To send mail from Rails use [ActionMailer](http://guides.rubyonrails.org/action_mailer_basics.html).

To see the generated mails in your web browser *instead* for sending them use the gem [letter_opener](https://github.com/ryanb/letter_opener)

### Errors

![better_errors screenshot](images/gem-better_errors.png)
[carliesome/better_errors](https://github.com/charliesome/better_errors)


Finding more Gems
----------
* [Ruby Toolbox](https://www.ruby-toolbox.com/) is organized in categories that help you find alternative solutions

