backgrounddir = join_paths(datadir, 'backgrounds', 'gnome47-alpha')
metadatadir = join_paths(datadir, 'gnome-background-properties')

conf = configuration_data()
conf.set('BACKGROUNDDIR', backgrounddir)
conf.set('datadir', datadir)

backgrounds = [
  'lcd-blue-d.jxl',
  'lcd-blue-l.jxl',
  'lcd-green-d.jxl',
  'lcd-green-l.jxl',
  'map-d.svg',
  'map-l.svg',
  'mollnar-d.svg',
  'mollnar-l.svg',
  'pills-d.jxl',
  'pills-l.jxl',
  'sheet-d.jxl',
  'sheet-l.jxl',
  'symbolic-soup-d.jxl',
  'symbolic-soup-l.jxl',
  'swoosh-d.jxl',
  'swoosh-l.jxl',
]

metadatas = [
  'gnome47-alpha-lcd-blue.xml',
  'gnome47-alpha-lcd-green.xml',
  'gnome47-alpha-map.xml',
  'gnome47-alpha-mollnar.xml',
  'gnome47-alpha-pills.xml',
  'gnome47-alpha-sheet.xml',
  'gnome47-alpha-symbolic-soup.xml',
  'gnome47-alpha-swoosh.xml',
]

install_data(backgrounds, install_dir: backgrounddir)

foreach metadata : metadatas
  configure_file(
    input: metadata + '.in',
    output: metadata,
    configuration: conf,
    install: true,
    install_dir: metadatadir
  )
endforeach
