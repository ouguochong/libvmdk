AM_CPPFLAGS = \
	-I$(top_srcdir)/include \
	-I$(top_srcdir)/common \
	@LIBCERROR_CPPFLAGS@ \
	@LIBCTHREADS_CPPFLAGS@ \
	@LIBCDATA_CPPFLAGS@ \
	@LIBCLOCALE_CPPFLAGS@ \
	@LIBCNOTIFY_CPPFLAGS@ \
	@LIBCSPLIT_CPPFLAGS@ \
	@LIBUNA_CPPFLAGS@ \
	@LIBCFILE_CPPFLAGS@ \
	@LIBCPATH_CPPFLAGS@ \
	@LIBBFIO_CPPFLAGS@ \
	@LIBFCACHE_CPPFLAGS@ \
	@LIBFDATA_CPPFLAGS@ \
	@LIBFVALUE_CPPFLAGS@ \
	@ZLIB_CPPFLAGS@ \
	@PTHREAD_CPPFLAGS@ \
	@LIBVMDK_DLL_IMPORT@

if HAVE_PYTHON_TESTS
TESTS_PYVMDK = \
	test_python_module.sh
endif

TESTS = \
	test_library.sh \
	test_vmdkinfo.sh \
	$(TESTS_PYVMDK)

check_SCRIPTS = \
	pyvmdk_test_handle.py \
	pyvmdk_test_read.py \
	pyvmdk_test_support.py \
	test_library.sh \
	test_python_module.sh \
	test_runner.sh \
	test_vmdkinfo.sh

EXTRA_DIST = \
	$(check_SCRIPTS)

check_PROGRAMS = \
	vmdk_test_descriptor_file \
	vmdk_test_error \
	vmdk_test_extent_descriptor \
	vmdk_test_extent_file \
	vmdk_test_extent_table \
	vmdk_test_grain_data \
	vmdk_test_grain_group \
	vmdk_test_grain_table \
	vmdk_test_handle \
	vmdk_test_io_handle \
	vmdk_test_notify \
	vmdk_test_support

vmdk_test_descriptor_file_SOURCES = \
	vmdk_test_descriptor_file.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_descriptor_file_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_error_SOURCES = \
	vmdk_test_error.c \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_unused.h

vmdk_test_error_LDADD = \
	../libvmdk/libvmdk.la

vmdk_test_extent_descriptor_SOURCES = \
	vmdk_test_extent_descriptor.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_extent_descriptor_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_extent_file_SOURCES = \
	vmdk_test_extent_file.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_extent_file_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_extent_table_SOURCES = \
	vmdk_test_extent_table.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_extent_table_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_grain_data_SOURCES = \
	vmdk_test_grain_data.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_grain_data_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_grain_group_SOURCES = \
	vmdk_test_grain_group.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_grain_group_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_grain_table_SOURCES = \
	vmdk_test_grain_table.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_grain_table_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_handle_SOURCES = \
	vmdk_test_functions.c vmdk_test_functions.h \
	vmdk_test_getopt.c vmdk_test_getopt.h \
	vmdk_test_handle.c \
	vmdk_test_libbfio.h \
	vmdk_test_libcerror.h \
	vmdk_test_libclocale.h \
	vmdk_test_libcnotify.h \
	vmdk_test_libuna.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_handle_LDADD = \
	@LIBBFIO_LIBADD@ \
	@LIBCPATH_LIBADD@ \
	@LIBCFILE_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCSPLIT_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libvmdk/libvmdk.la \
	@LIBCTHREADS_LIBADD@ \
	@LIBCERROR_LIBADD@ \
	@PTHREAD_LIBADD@

vmdk_test_io_handle_SOURCES = \
	vmdk_test_io_handle.c \
	vmdk_test_libcerror.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_memory.c vmdk_test_memory.h \
	vmdk_test_unused.h

vmdk_test_io_handle_LDADD = \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

vmdk_test_notify_SOURCES = \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_notify.c \
	vmdk_test_unused.h

vmdk_test_notify_LDADD = \
	../libvmdk/libvmdk.la

vmdk_test_support_SOURCES = \
	vmdk_test_functions.c vmdk_test_functions.h \
	vmdk_test_getopt.c vmdk_test_getopt.h \
	vmdk_test_libbfio.h \
	vmdk_test_libcerror.h \
	vmdk_test_libclocale.h \
	vmdk_test_libcnotify.h \
	vmdk_test_libuna.h \
	vmdk_test_libvmdk.h \
	vmdk_test_macros.h \
	vmdk_test_support.c \
	vmdk_test_unused.h

vmdk_test_support_LDADD = \
	@LIBBFIO_LIBADD@ \
	@LIBCPATH_LIBADD@ \
	@LIBCFILE_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCSPLIT_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libvmdk/libvmdk.la \
	@LIBCERROR_LIBADD@

MAINTAINERCLEANFILES = \
	Makefile.in

distclean: clean
	/bin/rm -f Makefile

