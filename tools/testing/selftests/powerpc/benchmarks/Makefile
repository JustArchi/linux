TEST_PROGS := gettimeofday context_switch

CFLAGS += -O3

all: $(TEST_PROGS)

$(TEST_PROGS): ../harness.c

context_switch: ../utils.c
context_switch: LDLIBS += -lpthread

include ../../lib.mk

clean:
	rm -f $(TEST_PROGS) *.o
