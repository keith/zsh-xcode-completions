all: simctl.txt

%.txt: FORCE
	$(MAKE) "$(basename $@)" &>$@

FORCE:

simctl:
	xcrun simctl || true
	@echo
	-xcrun simctl help help
	@echo
	-xcrun simctl help create
	@echo
	-xcrun simctl help clone
