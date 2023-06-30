# README

## Failing spec
bundle exec rspec

~~~
An error occurred while loading ./spec/models/application_record_spec.rb.
Failure/Error: require_relative '../config/environment'

NameError:
  uninitialized constant HTMLSelector::Minitest

    include Minitest::Assertions
            ^^^^^^^^
  Did you mean?  MiniMime
# ./config/application.rb:7:in `<top (required)>'
# ./config/environment.rb:2:in `require_relative'
# ./config/environment.rb:2:in `<top (required)>'
# ./spec/rails_helper.rb:4:in `require_relative'
# ./spec/rails_helper.rb:4:in `<top (required)>'
# ./spec/models/application_record_spec.rb:1:in `require'
# ./spec/models/application_record_spec.rb:1:in `<top (required)>'
No examples found.


Finished in 0.00006 seconds (files took 0.55748 seconds to load)
0 examples, 0 failures, 1 error occurred outside of examples
~~~

## Passing Spec

*uncomment `gem 'rails-dom-testing', '< 2.1.0'` in Gemfile and `bundle update`*

`bundle update && bundle exec rspec`
