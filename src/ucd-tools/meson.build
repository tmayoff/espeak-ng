ucd_lib = library(
    'ucd',
    'src/case.c',
    'src/categories.c',
    'src/ctype.c',
    'src/proplist.c',
    'src/scripts.c',
    'src/tostring.c',
    include_directories: 'src/include',
)
ucd_dep = declare_dependency(
    include_directories: 'src/include',
    link_with: ucd_lib,
)


test(
    'printcdata',
    executable(
        'printcdata',
        'tests/printcdata.c',
        include_directories: '../windows',
        dependencies: ucd_dep,
        c_args: '-DHAVE_ISWBLANK',
    ),
)

test(
    'printucddata_cpp',
    executable(
        'printucddata_cpp',
        'tests/printucddata_cpp.cpp',
        include_directories: '../windows',
        dependencies: ucd_dep,
        c_args: '-DHAVE_ISWBLANK',
    ),
)

test(
    'printucddata',
    executable(
        'printucddata',
        'tests/printucddata.c',
        include_directories: '../windows',
        dependencies: ucd_dep,
        c_args: '-DHAVE_ISWBLANK',
    ),
)
