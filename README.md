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

```
  dog = { name: "hip" , type: "puppy"  }
  
```
