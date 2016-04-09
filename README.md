# Line::Bot

[![Gem Version](https://badge.fury.io/rb/line-bot.svg)](https://badge.fury.io/rb/line-bot)

A Ruby interface to Line Bot API.

## Installation

    $ gem install line-bot

## Usage

```ruby
client = Line::Bot::Client.new do |config|
  config.channel_id     = "LINE_CHANNEL_ID"
  config.channel_secret = "LINE_CHANNEL_SECRET"
  config.channel_mid    = "LINE_CHANNEL_MID"
end

client.get_profiles(mids: "uxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
```


## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake test` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment. Run `bundle exec line-bot` to use the gem in this directory, ignoring other installed copies of this gem.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/line-bot. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
