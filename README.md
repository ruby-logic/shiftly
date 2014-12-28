## Shiftly

[![Gem Version](https://badge.fury.io/rb/shiftly.svg)](http://badge.fury.io/rb/shiftly)
[![Build Status](https://travis-ci.org/logicorg/shiftly.svg)](https://travis-ci.org/logicorg/shiftly)
[![Code Climate](https://codeclimate.com/github/logicorg/shiftly/badges/gpa.svg)](https://codeclimate.com/github/logicorg/shiftly)

Factory shift methods collection by [RubyLogic, PL](http://rubylogic.eu)

## Usage

Add it to your Gemfile with:

```ruby
gem 'shiftly'
```

Run the bundle command to install it.

Then you have access to the following extensions.

### Time class exts

```ruby
Time.now.to_factory_date
# returns yesterday when it is before 6am and today otherwise
```

```ruby
Time.now.shift
# returns shift number for datetime
```

```ruby
Time.now.shift_beg
# returns shift beginning datetime
```

```ruby
Time.now.shift_end
# returns shift end datetime
```

### Fixnum class exts

```ruby
1.next_shift
# returns next shift for 1, 2 or 3
```

```ruby
1.prev_shift
# returns previous shift for 1, 2 or 3
```