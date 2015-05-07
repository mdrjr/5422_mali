libdir := /usr/lib/arm-linux-gnueabihf/
includedir := /usr/include
pkgconfigdir := $(libdir)/pkgconfig

install:
	# Mali Binaries
	rm -fr $(libdir)/libmali.so
	rm -fr $(libdir)/libOpenCL.so
	rm -fr $(libdir)/libEGL.so
	rm -fr $(libdir)/libGLESv1_CM.so
	rm -fr $(libdir)/libGLESv2.so
	rm -fr $(libdir)/mali-egl
	cp -aRP mali_libs/* $(libdir)
	
	# Mali Headers
	rm -rf $(includedir)/EGL $(includedir)/GLES $(includedir)/GLES2 $(includedir)/GLES3 $(includedir)/KHR $(includedir)/C1 $(includedir)/CL_1_2
	cp -aRP mali_headers/* /usr/include
	
	# PKG Config
	rm -fr $(pkgconfigdir)/glesv*.pc $(pkgconfigdir)/egl.pc $(pkgconfigdir)/opencl.pc
	cp -aRP ../pkgconfig/* $(pkgconfigdir)
