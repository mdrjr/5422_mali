libdir := /usr/lib/arm-linux-gnueabihf/mali-egl
includedir := /usr/include
pkgconfigdir := /usr/lib/arm-linux-gnueabihf/pkgconfig

install:
	# Mali Binaries
	mkdir -p $(libdir)
	cp -aRP lib* $(libdir)
	cp -aRP ld.so.conf $(libdir)
	
	# Mali Headers
	rm -rf $(includedir)/EGL $(includedir)/GLES $(includedir)/GLES2 $(includedir)/GLES3 $(includedir)/KHR $(includedir)/C1 $(includedir)/CL_1_2
	cp -aRP ../headers/* /usr/include
	
	# PKG Config
	rm -fr $(pkgconfigdir)/glesv*.pc $(pkgconfigdir)/egl.pc $(pkgconfigdir)/opencl.pc
	cp -aRP ../pkgconfig/* $(pkgconfigdir)
