
installconf:

etcfiles =
varfiles =

sbin_PROGRAMS =

bin_PROGRAMS = axgetput

dist_man_MANS = axgetput.1
dist_doc_DATA = README.axgetput TIPS.txt TODO

axgetput_SOURCES = axgetput.c axgetput.h util.h proto_bin.h util.c proto_bin.c includes.h

install-exec-hook:
	(cd $(DESTDIR)$(bindir) && ln -sf axgetput bget && ln -sf axgetput bput)

install-data-hook:
	(cd $(DESTDIR)$(mandir)/man1 && ln -sf axgetput.1 bget.1 && ln -sf axgetput.1 bput.1)

AM_CPPFLAGS = -D_GNU_SOURCE
