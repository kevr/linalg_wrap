project('linalg_wrap', 'cpp',
  version : '0.1',
  default_options : ['warning_level=3',
                     'cpp_std=c++20']) # linalg requires C++20

# subprojects/linalg.wrap
linalg = subproject('linalg')
linalg_dep = linalg.get_variable('linalg_dep')

exe = executable('linalg_wrap', 'linalg_wrap.cpp',
  dependencies : [linalg_dep])
test('basic', exe)
