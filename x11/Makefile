libdir := /usr/lib/arm-linux-gnueabihf/mali-egl
pkgdir := /usr/share/mali

install:
	# Mali Binaries
	mkdir -p $(libdir)
	mkdir -p $(pkgdir)/headers
	mkdir -p $(pkgdir)/pkgconfig
	
	cp -aRP lib* $(libdir)
	cp -aRP ld.so.conf $(libdir)
	
	# Mali Headers
	cp -aRP ../headers/* $(pkgdir)/headers
	
	# PKG Config
	cp -aRP ../pkgconfig/* $(pkgdir)/pkgconfig
