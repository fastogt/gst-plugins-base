http_sources = [
  'gsthttpsink.c',
]

gsthttp = library('gsthttp',
  http_sources,
  c_args : gst_plugins_base_args,
  include_directories: [configinc, libsinc],
  dependencies : [gio_dep, gst_base_dep, gst_net_dep],
  install : true,
  install_dir : plugins_install_dir,
)
pkgconfig.generate(gsthttp, install_dir : plugins_pkgconfig_install_dir)
plugins += [gsthttp]
