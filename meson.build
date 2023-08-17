project('espeak-ng', ['c', 'cpp'], version: '0.0.1')

if meson.is_subproject()
    add_project_arguments('-w', language: 'cpp')
endif

add_project_arguments(
    '-DPATH_ESPEAK_DATA="/usr/' + get_option('libdir') + '/espeak-ng-data"',
    language: ['c', 'cpp'],
)

subdir('src')
subdir('tests')
