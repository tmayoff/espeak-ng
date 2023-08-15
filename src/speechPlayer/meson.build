speechPlayer_lib = library(
    'speechPlayer',
    'src/frame.cpp',
    'src/speechPlayer.cpp',
    'src/speechWaveGenerator.cpp',
    include_directories: ['include', 'src'],
)

speechPlayer_dep = declare_dependency(
    include_directories: 'include',
    link_with: speechPlayer_lib,
)
