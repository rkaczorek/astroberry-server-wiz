bin_PROGRAMS = astroberry-server-wiz

astroberry-server-wiz_CFLAGS = \
	-I$(top_srcdir) \
	-DPACKAGE_LIB_DIR=\""$(libdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(datadir)/astroberry-server-wiz"\" \
	-DPACKAGE_UI_DIR=\""$(datadir)/astroberry-server-wiz/ui"\" \
	-DPACKAGE_BIN_DIR=\""$(bindir)"\" \
	-DPACKAGE_LOCALE_DIR=\""$(prefix)/$(DATADIRNAME)/locale"\" \
	-I$(srcdir)/libdhcpcd \
	-I$(srcdir)/dhcpcd-gtk \
	$(PACKAGE_CFLAGS) \
	$(G_CAST_CHECKS)

astroberry-server-wiz_SOURCES = astroberry-server-wiz.c \
		libdhcpcd/config.c \
		libdhcpcd/dhcpcd.c \
		libdhcpcd/wpa.c \
		dhcpcd-gtk/wpa.c \
		dhcpcd-gtk/main.c


astroberry-server-wiz_includedir = $(includedir)/astroberry-server-wiz

astroberry-server-wiz_include_HEADERS =

astroberry-server-wiz_LDFLAGS = $(DYNAMIC_FLAGS)
astroberry-server-wiz_DEPENDENCIES_EXTRA = $(BUILTIN_PLUGINS)

astroberry-server-wiz_LDADD = \
		$(BUILTIN_PLUGINS) \
		$(PACKAGE_LIBS) \
		$(X11_LIBS) \
		$(INTLLIBS)

EXTRA_DIST =
