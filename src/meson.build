subdir('speechPlayer')
subdir('ucd-tools')

espeak_sources = files()
subdir('libespeak-ng')

espeak_lib = library(
    'libespeak-ng',
    espeak_sources,
    include_directories: ['include', 'libespeak-ng'],
    dependencies: [ucd_dep, speechPlayer_dep],
)
espeak_dep = declare_dependency(
    include_directories: 'include',
    link_with: espeak_lib,
)

executable(
    'speak-ng',
    'speak-ng.c',
    include_directories: ['windows'],
    dependencies: espeak_dep,
)
executable(
    'espeak-ng',
    'espeak-ng.c',
    include_directories: ['windows'],
    dependencies: espeak_dep,
)
