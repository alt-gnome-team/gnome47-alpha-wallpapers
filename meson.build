project('gnome47-alpha-backgrounds',
  version: '1.0.0',
  meson_version: '>= 0.56.0',
  license: 'CC-BY-SA-3.0'
)

i18n = import('i18n')

prefix = get_option('prefix')

datadir = join_paths(prefix, get_option('datadir'))

if get_option('target_de') == 'all'
  subdir('backgrounds/gnome')
else
  subdir('backgrounds/@0@'.format(get_option('target_de')))
endif

