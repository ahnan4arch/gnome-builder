# --enable-file-search-plugin=yes/no
AC_ARG_ENABLE([file-search-plugin],
              [AS_HELP_STRING([--enable-file-search-plugin=@<:@yes/no@:>@],
                              [Build with support for searching files in global search.])],
              [enable_file_search_plugin=$enableval],
              [enable_file_search_plugin=yes])

# for if ENABLE_FILE_SEARCH_PLUGIN in Makefile.am
AM_CONDITIONAL(ENABLE_FILE_SEARCH_PLUGIN, test x$enable_file_search_plugin != xno)

# Ensure our makefile is generated by autoconf
AC_CONFIG_FILES([plugins/file-search/Makefile])
