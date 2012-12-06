# ActiveSupport::Concern

## Usage

    require 'active_support'

    module Foo

      extend ActiveSupport::Concern

      included do
        # Runs upon inclusion of module Foo
      end

      module ClassMethods

        def this_is_a_class_method
        end

      end

    end