espeak_sources += files(
    'common.c',
    'compiledata.c',
    'compiledict.c',
    'compilembrola.c',
    'dictionary.c',
    'encoding.c',
    'error.c',
    'espeak_api.c',
    'espeak_command.c',
    'event.c',
    'fifo.c',
    'ieee80.c',
    'intonation.c',
    'klatt.c',
    'langopts.c',
    'mbrowrap.c',
    'mnemonics.c',
    'numbers.c',
    'phoneme.c',
    'phonemelist.c',
    'readclause.c',
    'sPlayer.c',
    'setlengths.c',
    'soundicon.c',
    'spect.c',
    'speech.c',
    'ssml.c',
    'synth_mbrola.c',
    'synthdata.c',
    'synthesize.c',
    'tr_languages.c',
    'translate.c',
    'translateword.c',
    'voices.c',
    'wavegen.c',
)

conf_data = configuration_data()
conf_data.set('USE_ASYNC', false)
conf_data.set_quoted('PACKAGE_VERSION', meson.project_version().underscorify())
#cmakedefine01 HAVE_MKSTEMP

#cmakedefine01 USE_KLATT
#cmakedefine01 USE_LIBPCAUDIO
#cmakedefine01 USE_LIBSONIC
#cmakedefine01 USE_MBROLA
#cmakedefine01 USE_SPEECHPLAYER
configure_file(
    output: 'config.h',
    configuration: conf_data,
)
