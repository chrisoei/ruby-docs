= OObbjjeecctt##wwiitthh__ooppttiioonnss

(from gem activesupport-3.2.8)
------------------------------------------------------------------------------
  with_options(options) { |option_merger| ... }

------------------------------------------------------------------------------

An elegant way to factor duplication out of options passed to a series of
method calls. Each method called in the block, with the block variable as the
receiver, will have its options merged with the default options hash provided.
Each method called on the block variable must take an options hash as its
final argument.

Without with_options>, this code contains duplication:

  class Account < ActiveRecord::Base
    has_many :customers, :dependent => :destroy
    has_many :products,  :dependent => :destroy
    has_many :invoices,  :dependent => :destroy
    has_many :expenses,  :dependent => :destroy
  end

Using with_options, we can remove the duplication:

  class Account < ActiveRecord::Base
    with_options :dependent => :destroy do |assoc|
      assoc.has_many :customers
      assoc.has_many :products
      assoc.has_many :invoices
      assoc.has_many :expenses
    end
  end

It can also be used with an explicit receiver:

  I18n.with_options :locale => user.locale, :scope => "newsletter" do |i18n|
    subject i18n.t :subject
    body    i18n.t :body, :user_name => user.name
  end

with_options can also be nested since the call is forwarded to its receiver.
Each nesting level will merge inherited defaults in addition to their own.


