AM_CFLAGS=-O3
AUTOMAKE_OPTIONS=std-options subdir-objects
bin_PROGRAMS=c_project

c_projectdir=$(PROJ_DIR)
c_project_SHORTNAME = cpr
c_project_CFLAGS=-I$(INCLUDE_DIR) -DLOCALEDIR=\"$(localedir)\"
c_project_LDADD=$(LIBMATH) $(LIBINTL)
c_project_LDFLAG=
c_project_SOURCES=main.c
c_project_HEADERS=$(INCLUDE_DIR)/gettext.h $(INCLUDE_DIR)/macros.h

.PHONY: check-syntax
check-syntax:
	gcc -o nul ${AM_CFLAGS} ${c_project_CFLAGS} -S ${CHK_SOURCES}
