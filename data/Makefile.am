uidir = $(datadir)/astroberry-server-wiz

ui_in_files = 	astroberry-server-wiz.ui \
				astroberry-logo.png

ui_DATA = $(ui_in_files)

desktopdir=/etc/xdg/autostart

desktop_in_files= \
	astroberry-server-wiz.desktop.in \
	$(NULL)
desktop_DATA = $(desktop_in_files:.desktop.in=.desktop)
@INTLTOOL_DESKTOP_RULE@

EXTRA_DIST = $(ui_in_files) \
			$(desktop_in_files) \
			$(desktop_DATA) \
			$(NULL)
