NINSTALL	= ../../ninstall

build:
	@echo ">>> Making build in `pwd`"

install:
	@echo ">>> Making install in `pwd`"
	mkdir -p $(DESTDIR)$(BINDIR)
	$(NINSTALL) -m 0755 \
		-e 's|%NMLIBDIR%|$(NMLIBDIR)|' \
		-e 's|%BINDIR%|$(BINDIR)|' \
		$(SUBST) metro* $(DESTDIR)$(BINDIR)

clean:
