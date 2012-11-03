Hash#fetch
==========


    hsh.fetch(key [, default] )       -> obj
    hsh.fetch(key) {| key | block }   -> obj


Returns a value from the hash for the given key. If the key can't be found,
there are several options: With no other arguments, it will raise an KeyError
exception; if default is given, then that will be returned; if
the optional code block is specified, then that will be run and its result
returned.

     h = { "a" => 100, "b" => 200 }
     h.fetch("a")                            #=> 100
     h.fetch("z", "go fish")                 #=> "go fish"
     h.fetch("z") { |el| "go fish, #{el}"}   #=> "go fish, z"

The following example shows that an exception is raised if the key is not
found and a default value is not supplied.

     h = { "a" => 100, "b" => 200 }
     h.fetch("z")

produces:

     prog.rb:2:in `fetch': key not found (KeyError)
      from prog.rb:2


