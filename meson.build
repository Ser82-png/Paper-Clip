project('pdf-metadata-editor', ['c', 'vala'],
          version: '5.0',
    meson_version: '>= 0.59.0',
  default_options: [ 'warning_level=2', 'werror=false', ],
)

i18n = import('i18n')
gnome = import('gnome')

app_id = 'io.github.diegoivan.pdf_metadata_editor'

if get_option ('profile') == 'devel'
endif

subdir('data')
subdir('src')
subdir('po')

gnome.post_install(
     glib_compile_schemas: true,
    gtk_update_icon_cache: true,
  update_desktop_database: true,
)
