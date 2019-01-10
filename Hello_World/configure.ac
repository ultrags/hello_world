AC_PREREQ(2.61)

# package version number (not shared library version)
# odd micro numbers indicate in-progress development
# even micro numbers indicate released versions
m4_define(Hello_World_version_major, 0)
m4_define(Hello_World_version_minor, 1)
m4_define(Hello_World_version_micro, 0)

m4_define([Hello_World_version],
          [Hello_World_version_major.Hello_World_version_minor.Hello_World_version_micro])
m4_define([Hello_World_api_version],
          [Hello_World_version_major.Hello_World_version_minor])

AC_INIT(Hello_World, Hello_World_version)
AM_INIT_AUTOMAKE
AC_CONFIG_HEADERS(config.h)

# Checks for programs.
AC_PROG_LIBTOOL
AC_PROG_CXX
AC_PROG_INSTALL

# enable pkg-config
PKG_PROG_PKG_CONFIG

# Checks for library functions.
#AC_CHECK_FUNCS([memset])

AC_SUBST(Hello_World_CFLAGS)
AC_SUBST(Hello_World_LIBS)


#icondir=${datadir}/icons/hicolor/32x32/apps
#AC_SUBST(icondir)

AC_OUTPUT([
Makefile
src/Makefile
])

echo ""
echo "   Hello_World $VERSION"
echo "   ====================="
echo ""
echo "   To build the project, run \"make\""
echo ""
