| ---- README.txt ---- |
Author: Ethan Davis
Date: 1/27/2021

To incorporate the test "alarm-mega", four files were modified
at path /src/tests/thread:

	(1) tests.h
		- test_alarm_mega of type test_func defined
		  with extern for global access

	(2) tests.c
		- Entry added to tests[] dictionary pairing
		  "alarm-mega" with function test_alarm_mega

	(3) Make.tests
		- Entry added to test/threads_TESTS array
		  of name "alarm-mega"

	(4) alarm-wait.c
		- test_alarm_mega of type void defined with
		  no parameters

		- test_alarm_mega calls test_sleep with a
		  duration of 5 ticks and 70 iterations
