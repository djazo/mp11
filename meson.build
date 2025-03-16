project('boost_mp11',
  ['cpp'],
  version: '1.88.0',
  default_options : ['cpp_std=c++20']
  )

cpp = meson.get_compiler('cpp')

assert(cpp.get_define('__cxx_alias_templates') == '','cxx_alias_templates not defined')
assert(cpp.get_define('__cxx_variadic_templates') == '','cxx_variadic_templates not defined')
assert(cpp.get_define('__cxx_decltype') == '','cxx_decltype not defined')

inc = include_directories('include')

boostmp11_dep = declare_dependency(
  include_directories : inc,
  )
