# sqlite3-ruby-win
guide for sqlite3-ruby installation on Windows without LoadError

### Steps
##### Pre
- `gem uninstall sqlite3 --all`

##### Source
- Download the latest sqlite3-ruby, https://github.com/sparklemotion/sqlite3-ruby
- unzip the package

##### Build
- run command-line in the extracted dir
- make sure you have your C compiler installed and added to PATH
- `gem install bundler`
- `bundle install`
- `rake native gem`
- you'll find a dir named 'pkg' was generated

##### Install
- enter dir 'pkg'
- `gem install --local sqlite3-xxx.gem` ('xxx' is version code)

##### Check
- `irb`
- `require 'sqlite3'`
