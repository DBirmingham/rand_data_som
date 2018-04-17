# Random Data SOM

The SOM from my sparta_ui_testing repo. A useful self contained service for generating random form data on the fly.

## Getting Started

Clone this repo to your computer and ensure you install the faker gem.
```
gem install faker
```
I recommend looking through the (faker readme)[https://github.com/stympy/faker] if you'd like to change the behaviour of this data generator. I appreciate that eldritch deities may not be suitable for most demonstrations.

### Prerequisites

This was done in Ruby 2.4.0 older versions may not be compatible. see here for instructions on updating your Ruby version (on Mac)

Necessary Gems
* faker

## Usage

require the gen_data.rb file and create an instance of the service model class, `DataGen`, calling the `rand_form_data` method on it. Assign this to a variable and you can begin to call some of the generation methods.

```ruby
@rand_data = DataGen.new.rand_form_data
@rand_data.username
@rand_data.pass
@rand_data.country
...
```

## Running Tests

Use the command 
```
rspec
```
in the root folder of the relevant test object to run the tests located within this project

## Built With
Ruby, rspec and faker!