#ruby learning notes from codecademy

#Hashes and Symbols

create a hash with no nill value

```ruby
  name = Hash.new("jona")
  
  name[:hello] # "jona"
  
```

#difference between string and symbols 

They’re immutable, meaning they can’t be changed once they’re created;
Only one copy of any symbol exists at a given time, so they save memory;

```ruby
  name = {
    :name => "joy"
  }
  
  is better than 
  
  name = {
    name : "joy"
  }
  
  
```

#converting symbols and string 

```ruby
  :hello.to_s # "hello"
  
  "hello".to_sym # :hello 
  or 
  "hello".intern # :hello

```

#other ways of writing hash

```ruby

  dog = { name: "hip" , type: "puppy"  }
  
```

#select Method 

```ruby
  dog.select { |key, value| value == "hip" } # returns {name: hip}
  
  
```

#response Method

Call and Response
Remember when we mentioned that symbols are awesome for referencing method names? Well, .respond_to? takes a symbol and returns true if an object can receive that method and false otherwise.

```ruby 
[1, 2, 3].respond_to?(:push) # true

[1, 2, 3].respond_to?(:to_sym) #false

4.respond_to?(:next) #true

```
