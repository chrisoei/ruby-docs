Hash#assert_valid_keys
======================

(from gem activesupport-3.0.0)
------------------------------

    assert_valid_keys(*valid_keys)

Validate all keys in a hash match *valid keys, raising ArgumentError on a
mismatch. Note that keys are NOT treated indifferently, meaning if you use
strings for keys but assert symbols as keys, this will fail.

Examples
--------
    { :name => "Rob", :years => "28" }.assert_valid_keys(:name, :age) # => raises "ArgumentError: Unknown key(s): years"
    { :name => "Rob", :age => "28" }.assert_valid_keys("name", "age") # => raises "ArgumentError: Unknown key(s): name, age"
    { :name => "Rob", :age => "28" }.assert_valid_keys(:name, :age) # => passes, raises nothing


