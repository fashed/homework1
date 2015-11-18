#Unix/Linux/MacOSX Commands
* `~` : This symbol means "home" on the UNIX command line.
* `/` : This symbol means "root", the ultimate parent directory.
* `whoami` : This makes the terminal output the current user name.
* `pwd` : Print Web Directory
* `cd` : Change Directory
* `ls` :  List
* `cd ..` : Go back up a folder
* `mkdir` : Make new directory
* `touch` : "Touch filename" creates new file
* `cat` : Cat is short for concatenate. "Cat filename" prints all content in that file.
* `.` : Here/This
* `rm` : Remove 
* `rm -rf` : Remove all folders and files contained without prompting for confirmation
* `man` : "Man command" is god mode

# Basic Git commands
* `git init` : Initalize git, in a directory
* `git add .` : Git add all files to be staged
* `git add hello.txt` : Git add hello.txt to be staged
* `git status` : Check status for any modifications before committing
* `git commit -m 'created hello.txt` : Commit changes with message "hello.txt"
* `git push origin master` : Push changes up to cloud remote named origin and local branch name master

# Class 2 -- Strings and Numbers

* Ruby: ruby is an object oriented programming language
* MINASWAN: Mats is nice so we are nice
* truthy and falsey values: Something which evaluates to true. Something which evaluates to false.
* IRB: Interactive ruby shell
* variable: A placeholder to store data values
* method: A program that stores and runs code
* `def`: Defining a method
* parameters: Value passed into a method
* `=`: Assign
* `gets.chomp`: returns string without spaces or breaks
* `puts`: Put String
* String: Text
* Fixnum: Integers only
* Float: Numbers with decimal points
* String interpolation ( `#{ something in ruby }` ):Replace placeholders within a string with values they represent
* `.to_i`:Method to convert to integer
* `.to_s`:Method to convert to string
* `+` with strings:Combines strings together
* `+` with numbers:Adds numbers together
* `-`:Subtract
* `*`:Multiply
* `/`:Divide
* `%`:Modulus
* `==`:Equal
* `.class`:method to check data type
* `.reverse`:method to reverse letters in string
* `.reverse!`:reverse letters in string in place, saving over existing variable
* `.upcase`:method to convert letters in string to uppercase
* `.downcase`:method to convert letters in string to lowercase
* `.upcase!`:Convert letters in string to uppercase in place, saving over existing variable
* `.downcase!`:Convert letters in string to lowercase in place, saving over existing variable
* `<`: boolean, less than
* `>`: boolean, greater than
* `>=`: boolean, greater than or equals to 
* `<=`: boolean, less than or equals to
* `if`: conditional if condition
* `elif`: second if condition
* `else`: else is the default fallback condition if none of the above are true

#Class 3 -- Loops and Collections

* Comparison operators:
  * `==`: Equal to
  * `!=`: Not equal
  * `<=`: Less than or equal to
  * `>=`: Greater than or equal to
  * `>`: Greater than
  * `<`: Less than
* Logical operators:
  * `&&`: Logical AND operator. If both operands are non zero then condition becomes true.
  * `||`: Logical OR operator. If either operand is non zero then condition becomes true.
  * `!`: Bang, means not.
* Loops: A loop is a block that repeats operations
* `.times`: 100.times do |num| Does the same operation x.times
* `while`:while (condition): conditional loop, iterates as long as condition is true
* `until`:until (condition): conditional loop, iterates until condition is true
* `upto`: 1.upto(10) do |num|
* `downto`:10.downto(1) do |num|
* `+=`: num = num + 1
* `-=`: num = num - 1
* Arrays: a list of objects
	* How to instantiate a new one: arr = []
	* How to grab the first element in an array: arr[0] or arr.first
	* How to grab the last element: arr[-1] or arr.last
	* How to remove the last element: arr.pop
	* How to remove the first element: arr.shift
	* How to check whether the element `"odelay"` exists inside an array:arr.include?("odelay")
	* Three ways to add a new element to an array:
	1. arr << "element" - adds to end of array
	2. arr.push("element") - adds to end of array
	3. arr.unshift("a") - adds to front of array
* Hashes: a dictionary like collection of keys and values
	* How to instantiate a new one: hash = {}
	* Keys: a string used to store and reference values, strings, hashes, arrays as values
	* Values: values, strings, hashes, arrays attached to a key
	* How to retrieve the value of `"name"` in the hash `person`: person["name"]
	* How to set the value of `name` in the hash `person` person["name"]="newName"
	* How to write a hash with strings as keys:
	hash = {"name" => "value"}
	* How to write a hash with symbols as keys
	hash = {:name => "value"}
	hash[:name2] = "value2"

#Class 4 -- Iteration, Gems, APIs
* Iteration: take first and subsequent objects and do something with them repeatedly till the end of the collection is reached
* `.each`: perform an operation on each item in a collection
	* How to use .each to iterate over each item in an array:
		arr.each do |placeholder|
			puts placeholder
		end
	* How to use .each to iterate over each item in a hash:
		hash.each do |k,v|
			puts "#{k.upcase}: #{v}"
		end
* Ruby Gems:Libraries of code that can be used for free
* API: Application Programming Interface. Set of protocols for building software apps and sending messages or data between software
* JSON:  JavaScript Object Notation. JSON is a syntax for storing and exchanging data.
* What does HTTParty do exactly? Queries web services and examines the resulting output. HTTParty is a new Ruby library by John Nunemaker (of railstips.org fame) that makes it a snap to build classes that can use Web-based APIs and related services. 
* What does `require 'httparty'` do in a Ruby program? brings the httparty gem's capabilities into my application
* Explain what `response = HTTParty.get "https://itunes.apple.com/search?term=smashing%20pumpkins"` does. At its simplest, you include the HTTParty module within a class, which gives your class a "get" method that can retrieve data over HTTP, from the url.
* How do you parse `response` into a usable Ruby Hash object? 
j = JSON.parse(response)

