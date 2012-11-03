Hash < Object
=============

Includes
--------
Enumerable (from ruby site)

A Hash is a collection of key-value pairs. It is similar to an Array, except
that indexing is done via arbitrary keys of any object type, not an integer
index. Hashes enumerate their values in the order that the corresponding keys
were inserted.

Hashes have a default_value that is returned when
accessing keys that do not exist in the hash. By default, that value is nil.

Class methods
-------------
    []
    new
    try_convert

Instance methods
----------------

    ==
    []
    []=
    assoc
    clear
    compare_by_identity
    compare_by_identity?
    default
    default=
    default_proc
    default_proc=
    delete
    delete_if
    each
    each_key
    each_pair
    each_value
    empty?
    eql?
    fetch
    flatten
    has_key?
    has_value?
    hash
    include?
    initialize_copy
    inspect
    invert
    keep_if
    key
    key?
    keys
    length
    member?
    merge
    merge!
    pretty_print
    pretty_print_cycle
    rassoc
    rehash
    reject
    reject!
    replace
    select
    select!
    shift
    size
    store
    to_a
    to_hash
    to_s
    update
    value?
    values
    values_at


Class methods
-------------

  from_xml

Instance methods
----------------

  assert_valid_keys
  deep_merge
  deep_merge!
  diff
  encode_json
  except
  except!
  extract!
  extractable_options?
  reverse_merge
  reverse_merge!
  reverse_update
  slice
  slice!
  stringify_keys
  stringify_keys!
  symbolize_keys
  symbolize_keys!
  to_options
  to_options!
  to_param
  to_query
  to_xml
  with_indifferent_access


Instance methods
----------------

  symbolize_keys!


Class methods
-------------

  []
  create
  create_186

