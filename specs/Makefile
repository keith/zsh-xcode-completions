all: simctl.txt

%.txt: FORCE
	$(MAKE) "$(basename $@)" >$@

FORCE:

simctl:
	-xcrun simctl
