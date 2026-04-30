# My Favorite 4 Ruby Methods
### `thursday?`
Checkes whether the current date/time is on a Thursday
```
t = Time.utc(2000, 1, 6) # => 2000-01-06 00:00:00 UTC
t.thursday?              # => true
```
### `spell_checkers()`
Returns a list of errors and spelling mistakes (probably not actually but idk)
```
require 'did_you_mean'

checker = DidYouMean::SpellChecker.new(dictionary: ['apple', 'banana', 'orange'])
checker.correct('aple') # => ["apple"]
```
### `print()`
Prints to the console
```
cgi = CGI.new
cgi.print    # default:  cgi.print == $DEFAULT_OUTPUT.print
```
### `measure()`
Returns the time it takes to execute a certain block of code
```
require 'benchmark'

n = 1000000

time = Benchmark.measure do
  n.times { a = "1" }
end
puts time
```