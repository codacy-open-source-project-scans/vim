# Portable Makefile for running indent tests.

.SUFFIXES:
.PHONY: test clean testclean

VIM = vim
VIMRUNTIME = ..

# Run the tests that didn't run yet or failed previously.
# If a test succeeds a testdir/*.out file will be written.
# If a test fails a testdir/*.fail file will be written.
test:
	VIMRUNTIME=$(VIMRUNTIME) $(VIM) --clean --not-a-term -u testdir/runtest.vim


clean testclean:
	rm -f testdir/*.fail testdir/*.out
