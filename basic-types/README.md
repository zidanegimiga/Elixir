## Basic Types
----------------

- Integers
- Float
- Boolean

### Atom

``` 
    Atoms are constants whose value is the name of the variable
    Example: :atom-name
    - To check if a variable is an attom, use the is-atom() function.
      e.g: is_atom(variable)
    
    - The booleans true and false are also the atoms :true and :false
      is_boolean(:true)
      :true === true
      all return true.
    
    - Names of modules in Elixir are also atoms. MyApp.MyModule is a valid atom, even if no such module has been declared yet.

    - Atoms are also used to reference modules from Erlang libraries, including built in ones.
    Example: :crypto.strong_rand_bytes 3
              <<23, 104, 108>>
```

### String
- Strings in Elixir are UTF-8 encoded and are wrapped in double quotes
- There's a difference between single and double quotes in ELixr.
  
  #### double quotes:
  - Used to represent strings whereas

  ### single quotes:
  - Represent character lists


### Boolean
Elixir provides the ||, &&, and ! boolean operators

- -20 || true --> -20
- 42 && true --> 42
- 42 && nil --> nil
- false or true --> true
- 42 and true
  ** (ArgumentError) argument error: 42
- not 42
  ** (ArgumentError) argument error


### Comparison
Elixir comes with all the comparison operators we’re used to: ==, !=, ===, !==, <=, >=, <, and >

``` 
An important feature of Elixir is that any two types can be compared; this is particularly useful in sorting. We don’t need to memorize the sort order, but it is important to be aware of it.
Example:
    :hello > 999
    true
```

### String Interpolator
>>name = "Sean"
>> "Sean"
>> "Hello #{name}"
>> "Hello Sean"

### String Interpolator
name = "Sean"
>> "Sean"
>> "Hello " <> name
>> "Hello Sean" 