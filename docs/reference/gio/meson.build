if get_option('gtk_doc')
  subdir('xml')

  ignore_headers = [
    'fam',
    'fen',
    'gdbus-2.0',
    'gvdb',
    'inotify',
    'kqueue',
    'libasyncns',
    'tests',
    'win32',
    'xdgmime',
    'gappinfoprivate.h',
    'gapplicationimpl.h',
    'gasynchelper.h',
    'gcontenttypeprivate.h',
    'gcontextspecificgroup.h',
    'gcredentialsprivate.h',
    'gdbus-daemon-generated.h',
    'gdbusactiongroup-private.h',
    'gdbusauth.h',
    'gdbusauthmechanismanon.h',
    'gdbusauthmechanismexternal.h',
    'gdbusauthmechanism.h',
    'gdbusauthmechanismsha1.h',
    'gdbusdaemon.h',
    'gdbusprivate.h',
    'gdelayedsettingsbackend.h',
    'gdummyfile.h',
    'gdummyproxyresolver.h',
    'gdummytlsbackend.h',
    'gfileattribute-priv.h',
    'gfileinfo-priv.h',
    'ghttpproxy.h',
    'giomodule-priv.h',
    'gioprivate.h',
    'giowin32-priv.h',
    'glocaldirectorymonitor.h',
    'glocalfileenumerator.h',
    'glocalfile.h',
    'glocalfileinfo.h',
    'glocalfileinputstream.h',
    'glocalfileiostream.h',
    'glocalfilemonitor.h',
    'glocalfileoutputstream.h',
    'glocalvfs.h',
    'gmountprivate.h',
    'gnativevolumemonitor.h',
    'gnetworkingprivate.h',
    'gnetworkmonitorbase.h',
    'gnetworkmonitornetlink.h',
    'gnetworkmonitornm.h',
    'gnetworkmonitorportal.h',
    'gnotificationbackend.h',
    'gnotification-private.h',
    'gpollfilemonitor.h',
    'gproxyresolverportal.h',
    'gregistrysettingsbackend.h',
    'gresourcefile.h',
    'gsettingsbackendinternal.h',
    'gsettings-mapping.h',
    'gsettingsschema-internal.h',
    'gsocketinputstream.h',
    'gsocketoutputstream.h',
    'gsocks4aproxy.h',
    'gsocks4proxy.h',
    'gsocks5proxy.h',
    'gsubprocesslauncher-private.h',
    'gthreadedresolver.h',
    'gunionvolumemonitor.h',
    'gunixmount.h',
    'gunixresolver.h',
    'gunixvolume.h',
    'gunixvolumemonitor.h',
    'gwin32appinfo.h',
    'gwin32mount.h',
    'gwin32registrykey.h',
    'gwin32resolver.h',
    'gwin32volumemonitor.h',
    'thumbnail-verify.h',
    'xdp-dbus.h',
  ]

  if host_system == 'windows'
    ignore_headers += [
      'gfiledescriptorbased.h',
      'gunixconnection.h',
      'gunixcredentialsmessage.h',
      'gunixmounts.h',
      'gunixfdlist.h',
      'gunixfdmessage.h',
      'gunixinputstream.h',
      'gunixoutputstream.h',
      'gunixsocketaddress.h',
      'gdesktopappinfo.h',
      'gosxappinfo.h',
    ]
  else
    if glib_have_cocoa
      ignore_headers += ['gdesktopappinfo.h']
    else
      ignore_headers += ['gosxappinfo.h']
    endif

    ignore_headers += [
      'gwin32networkmonitor.h',
      'gwin32inputstream.h',
      'gwin32outputstream.h',
    ]
  endif

  ignore_decorators = [
    'GLIB_VAR',
    'G_GNUC_INTERNAL',
    'G_GNUC_WARN_UNUSED_RESULT',
    'GLIB_AVAILABLE_IN_ALL',
    'GLIB_AVAILABLE_IN_2_26',
    'GLIB_AVAILABLE_IN_2_28',
    'GLIB_AVAILABLE_IN_2_30',
    'GLIB_AVAILABLE_IN_2_32',
    'GLIB_AVAILABLE_IN_2_34',
    'GLIB_AVAILABLE_IN_2_36',
    'GLIB_AVAILABLE_IN_2_38',
    'GLIB_AVAILABLE_IN_2_40',
    'GLIB_AVAILABLE_IN_2_42',
    'GLIB_AVAILABLE_IN_2_44',
    'GLIB_AVAILABLE_IN_2_46',
    'GLIB_AVAILABLE_IN_2_48',
    'GLIB_AVAILABLE_IN_2_50',
    'GLIB_AVAILABLE_IN_2_52',
    'GLIB_AVAILABLE_IN_2_54',
    'GLIB_AVAILABLE_IN_2_56',
    'GLIB_DEPRECATED_IN_2_26',
    'GLIB_DEPRECATED_IN_2_26_FOR',
    'GLIB_DEPRECATED_IN_2_28',
    'GLIB_DEPRECATED_IN_2_28_FOR',
    'GLIB_DEPRECATED_IN_2_30',
    'GLIB_DEPRECATED_IN_2_30_FOR',
    'GLIB_DEPRECATED_IN_2_32',
    'GLIB_DEPRECATED_IN_2_32_FOR',
    'GLIB_DEPRECATED_IN_2_34',
    'GLIB_DEPRECATED_IN_2_34_FOR',
    'GLIB_DEPRECATED_IN_2_36',
    'GLIB_DEPRECATED_IN_2_36_FOR',
    'GLIB_DEPRECATED_IN_2_38',
    'GLIB_DEPRECATED_IN_2_38_FOR',
    'GLIB_DEPRECATED_IN_2_40',
    'GLIB_DEPRECATED_IN_2_40_FOR',
    'GLIB_DEPRECATED_IN_2_42',
    'GLIB_DEPRECATED_IN_2_42_FOR',
    'GLIB_DEPRECATED_IN_2_44',
    'GLIB_DEPRECATED_IN_2_44_FOR',
    'GLIB_DEPRECATED_IN_2_46',
    'GLIB_DEPRECATED_IN_2_46_FOR',
    'GLIB_DEPRECATED_IN_2_48',
    'GLIB_DEPRECATED_IN_2_48_FOR',
    'GLIB_DEPRECATED_IN_2_50',
    'GLIB_DEPRECATED_IN_2_50_FOR',
    'GLIB_DEPRECATED_IN_2_52',
    'GLIB_DEPRECATED_IN_2_52_FOR',
    'GLIB_DEPRECATED_IN_2_54',
    'GLIB_DEPRECATED_IN_2_54_FOR',
    'GLIB_DEPRECATED_IN_2_56',
    'GLIB_DEPRECATED_IN_2_56_FOR',
  ]

  # FIXME: More win32 headers were added to fix building gio-scan

  # FIXME: ExampleAnimal docs aren't built

  docpath = join_paths(glib_datadir, 'gtk-doc', 'html')
  version_conf = configuration_data()
  version_conf.set('VERSION', meson.project_version())
  configure_file(
    input: 'version.xml.in',
    output: 'version.xml',
    configuration: version_conf
  )

  gnome.gtkdoc('gio',
    main_xml : 'gio-docs.xml',
    namespace : 'g',
    mode : 'none',
    dependencies : [libgio_dep, libgobject_dep, libglib_dep],
    src_dir : 'gio',
    scan_args : [
      '--rebuild-types',
      '--deprecated-guards=G_DISABLE_DEPRECATED',
      '--ignore-decorators=' + '|'.join(ignore_decorators),
      '--ignore-headers=' + ' '.join(ignore_headers),
    ],
    content_files : [
      'overview.xml',
      'migrating-posix.xml',
      'migrating-gnome-vfs.xml',
      'migrating-gconf.xml',
      'migrating-gdbus.xml',
      'gio-querymodules.xml',
      'glib-compile-schemas.xml',
      'glib-compile-resources.xml',
      'gapplication.xml',
      'gsettings.xml',
      'gresource.xml',
      'gdbus.xml',
      'gdbus-codegen.xml',
    ],
    expand_content_files : [
      'overview.xml',
      'migrating-posix.xml',
      'migrating-gnome-vfs.xml',
      'migrating-gconf.xml',
      'migrating-gdbus.xml',
      'gdbus-codegen.xml',
    ],
    html_assets : [
      'gvfs-overview.png',
      'menu-example.png',
      'menu-model.png',
    ],
    fixxref_args: [
      '--html-dir=' + docpath,
      '--extra-dir=' + join_paths('gio', '..', 'glib', 'html'),
      '--extra-dir=' + join_paths('gio', '..', 'gobject', 'html'),
    ],
    install: true
  )
endif


if get_option('man')
  manpages = ['gapplication', 'gio-querymodules', 'glib-compile-schemas',
              'glib-compile-resources', 'gsettings', 'gresource', 'gdbus',
              'gio', 'gdbus-codegen']
  foreach page : manpages
    custom_target(page + '-man',
      input: page + '.xml',
      output: page + '.1',
      command: xsltproc_command,
      install: true,
      install_dir: man1_dir)
  endforeach
endif
