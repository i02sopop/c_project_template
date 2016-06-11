TESTS = check_c_project
check_PROGRAMS = check_c_project
check_c_project_SOURCES = test.c
check_c_project_CFLAGS = -I$(INCLUDE_DIR) -DLOCALEDIR=\"$(localedir)\" $(CHECK_CFLAGS)
check_c_project_LDADD = $(LIBMATH) $(LIBINTL) $(CHECK_LIBS)

