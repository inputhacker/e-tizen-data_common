MAINTAINERCLEANFILES = Makefile.in
SUBDIRS = tizen-common

EET_EET = @eet_eet@

EXTRA_DIST = profile.src

filesdir = $(prefix)/data/config/

files_DATA = profile.cfg

SUFFIXES = .cfg

.src.cfg:
	$(EET_EET) -i \
	$(top_builddir)/default/config/$@ config \
	$< 0

clean-local:
	rm -rf *.cfg *~
