Hash
====

Passing Parameters
------------------

    def foo(options)
      [assert_valid_keys][] :email, :nickname
      puts options.fetch :email
    end

[assert_valid_keys]: https://github.com/chrisoei/ruby-docs/blob/master/Hash/Hash%23assert_valid_keys.md