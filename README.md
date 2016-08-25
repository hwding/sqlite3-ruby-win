# sqlite3-ruby-win
How to install sqlite3 gem on Windows without LOAD_ERROR

### Steps
##### First
- Download the latest sqlite3-ruby, https://github.com/sparklemotion/sqlite3-ruby
- unzip the package

##### Second
- run command-line in the extracted dir
- make sure you have your C compiler installed and added to PATH
- `gem install bundler`
- `bundle install`
- `rake native gem`
- after it is done, you'll find a dir named pkg was generated

##### Third
- go in to this directory
- `gem install --local sqlite3-xxx.gem` ('xxx' is version code)

##### Fourth
- `irb`
- `require 'sqlite3'`
