Chages made in /cis520/pintos/src/tests/threads directory
Created the file alarm-mega.ck similar to alarm-multiple.ck but with 70 alarms instead of 7.

Added entry in Rubric.alarm -> 4	alarm-mega

Added entry in Make.tests -> alarm-mega

Added entry in tests.c -> {"alarm-mega", test_alarm_mega},

Added entry in tests.h -> extern test_func test_alarm_mega;

Added function for test_alarm_mega in alarm-wait.c:
void
test_alarm_mega (void)
{
	test_sleep (5,70);
}
