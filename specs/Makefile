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
	@echo
	-xcrun simctl help upgrade
	@echo
	-xcrun simctl help delete
	@echo
	-xcrun simctl help pair
	@echo
	-xcrun simctl help unpair
	@echo
	-xcrun simctl help pair_activate
	@echo
	-xcrun simctl help erase
	@echo
	-xcrun simctl help boot
	@echo
	-xcrun simctl help shutdown
