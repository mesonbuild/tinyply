project('tinyply', 'cpp',
    version: '2.0',
    default_options: ['cpp_std=c++11'])
pkg = import('pkgconfig')

i = include_directories('source')
tinyply_lib = library('tinyply', 'source/tinyply.cpp')
install_headers('source/tinyply.h')
tinyply_dep = declare_dependency(include_directories: i,
    link_with: tinyply_lib)

pkg.generate(tinyply_lib)
