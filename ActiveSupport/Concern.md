# ActiveSupport::Concern

## Usage

    require 'active_support'

    module Foo

      extend ActiveSupport::Concern

      module ClassMethods

        def this_is_a_class_method
        end

      end

    end