libdir := /usr/lib/arm-linux-gnueabihf/
includedir := /usr/include
pkgconfigdir := $(libdir)/pkgconfig

install:
	# Mali Binaries
	rm -fr $(libdir)/libMali.so
	rm -fr $(libdir)/libUMP.so
	rm -fr $(libdir)/mali-egl
	cp -aRP mali_libs/* $(libdir)
	
	# Mali Headers
	rm -rf $(includedir)/EGL $(includedir)/GLES $(includedir)/GLES2 $(includedir)/ump $(includedir)/umplock
	cp -aRP mali_headers/* /usr/include
	
	# PKG Config
	rm -fr $(pkgconfigdir)/glesv*.pc $(pkgconfigdir)/egl.pc
	cp -aRP ../pkgconfig/* $(pkgconfigdir)
	

		