project('octopus', 'cpp',
        default_options : ['warning_level=3', 'cpp_std=c++23'])

if get_option('buildtype') == 'debug'
    add_global_arguments('-DDEBUG', language : 'cpp')
endif

sfml_dep = dependency('sfml')

executable('octop',
          'src/octopus.cpp',
          'src/main.cpp',
          include_directories : 'include',
          dependencies: sfml_dep)
