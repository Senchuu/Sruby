[![Les Laboratoires Ruby](https://invidget.switchblade.xyz/4P7XcmbDnt)](https://discord.gg/4P7XcmbDnt)
# Sruby

Sruby is a Ruby Library for easy SQLite interactions. It is a wrapper around the SQLite3 Ruby library.
Use it to create, read, update, and delete data from SQLite databases without write any query.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'sruby'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install sruby

## Usage

To use the librairy, you need to create a database:

```rb
db = Sruby::Database.new('my_database.db')
```

Then you can create a table:
```rb
db.create('my_table')
```

Table creation creates a new getter callable from `db.my_table`, which returns a `Sruby::Table` object.
To manage data you can use the `insert` or`update` methods.
You can get get the data with the `get` and `all` methods.

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/sruby. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/[USERNAME]/sruby/blob/master/CODE_OF_CONDUCT.md).

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Sruby project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/sruby/blob/master/CODE_OF_CONDUCT.md).
