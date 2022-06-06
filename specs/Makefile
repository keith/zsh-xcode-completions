all: simctl.txt

%.txt: FORCE
	$(MAKE) "$(basename $@)" &>$@

FORCE:

simctl:
	xcrun simctl || true
	@for command in $$(xcrun simctl | grep '^\t' | awk '{print $$1}'); do \
		echo; \
		echo xcrun simctl help $$command; \
		xcrun simctl help $$command; \
	done
	@echo
	xcrun simctl help listapps
