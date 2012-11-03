Hash
====

Passing Parameters
------------------

    def foo(options)
      options.assert_valid_keys :email, :nickname
      puts options.fetch :email
      puts options.fetch :nickname, 'John'
    end


See also: [Hash#assert_valid_keys][], [Hash#fetch][]

[Hash#assert_valid_keys]: https://github.com/chrisoei/ruby-docs/blob/master/Hash/Hash%23assert_valid_keys.md

[Hash#fetch]: https://github.com/chrisoei/ruby-docs/blob/master/Hash/Hash%23fetch.md