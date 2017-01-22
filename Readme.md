Softly kills your process with SIGTERM before it runs out of memory.

Written in Rust to consume minimal resources.

Tested with Ruby to have readable / expressive tests.

### Build
 - [install rust](https://www.rust-lang.org/en-US/install.html)
 - `cargo build`

### Test
 - Build
 - `gem install bundler` ... needs [ruby](https://www.ruby-lang.org/en/) installed
 - `bundle`
 - `bundle exec rake`
 
### Release
 - `bundle exec rake bump:patch`
 - `cargo build --release`
 - take `target/release/preoomkiller` binary

### TODO
 - let through all unknown options
 - make interval configureable
 - find safe way of doing wait / kill ... http://stackoverflow.com/questions/35093869
 - make `rake bump` release for multiple targets and commit all changes
