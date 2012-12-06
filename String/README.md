# Ruby Strings, with Rails extensions

    1.9.3p194 :001 > require 'active_support/core_ext'
    true
    1.9.3p194 :002 > "abc_def".humanize
    "Abc def"
    1.9.3p194 :003 > "abc_def".titleize
    "Abc Def"
    1.9.3p194 :004 > "abc_def".camelize
    "AbcDef"
    1.9.3p194 :005 > "abc_def".underscore
    "abc_def"
    1.9.3p194 :006 > "abc_def".upcase
    "ABC_DEF"
    1.9.3p194 :007 > "Abc_Def".downcase
    "abc_def"
    1.9.3p194 :008 > "abc_def".capitalize
    "Abc_def"
    1.9.3p194 :009 > "abc_def".dasherize
    "abc-def"
    1.9.3p194 :010 > "abc_def".pluralize
    "abc_defs"
    1.9.3p194 :011 > "men".singularize
    "man"
    1.9.3-p194 :012 >   "person".tableize
    "people"
    1.9.3-p194 :044 > "HelloController".slice(0..-11)
    "Hello"
    1.9.3-p194 :047 > "HelloController".partition("Controller")[0]
    "Hello"
    1.9.3-p194 :050 > x="HelloController"
    "HelloController"
    1.9.3-p194 :051 > x['Controller']=''
    ""
    1.9.3-p194 :052 > x
    "Hello"
