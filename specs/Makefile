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
	@# Undocumented/internal commands:
	@echo
	xcrun simctl help addphoto
	@echo
	xcrun simctl help addvideo
	@echo
	xcrun simctl help pbinfo
	@echo
	xcrun simctl help notify_post
	@echo
	xcrun simctl help notify_get_state
	@echo
	xcrun simctl help notify_set_state
	@echo
	xcrun simctl help register
	@echo
	xcrun simctl help unregister
	@echo
	xcrun simctl help keyboard
	@echo
	xcrun simctl help monitor
	@echo
	xcrun simctl help appinfo
	@echo
	xcrun simctl help listapps
	@echo
	xcrun simctl help bootstatus
	@echo
	xcrun simctl help darwinup
	@echo
	xcrun simctl help disk
	@echo
	xcrun simctl help runtime
	@echo
	xcrun simctl help reset
