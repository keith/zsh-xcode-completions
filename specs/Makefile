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
	@echo
	-xcrun simctl help rename
	@echo
	-xcrun simctl help getenv
	@echo
	-xcrun simctl help openurl
	@echo
	-xcrun simctl help addmedia
	@echo
	-xcrun simctl help install
	@echo
	-xcrun simctl help uninstall
	@echo
	-xcrun simctl help get_app_container
	@echo
	-xcrun simctl help install_app_data
	@echo
	-xcrun simctl help launch
	@echo
	-xcrun simctl help terminate
	@echo
	-xcrun simctl help spawn
	@echo
	-xcrun simctl help list
	@echo
	-xcrun simctl help icloud_sync
	@echo
	-xcrun simctl help pbsync
	@echo
	-xcrun simctl help pbcopy
	@echo
	-xcrun simctl help pbpaste
