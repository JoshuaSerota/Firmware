Command line used to find this crash:

afl-fuzz -f ./afl/input_file -i ./afl/in -o ./afl/out4 -t 10000+ -m 2500 /home/josh/Documents/CSE637/px4/firmware_fork/build/px4_sitl_default/bin/px4 /home/josh/Documents/CSE637/px4/firmware_fork/ROMFS/px4fmu_common -s etc/init.d-posix/rcS -t /home/josh/Documents/CSE637/px4/firmware_fork/test_data

If you can't reproduce a bug outside of afl-fuzz, be sure to set the same
memory limit. The limit used for this fuzzing session was 2.44 GB.

Need a tool to minimize test cases before investigating the crashes or sending
them to a vendor? Check out the afl-tmin that comes with the fuzzer!

Found any cool bugs in open-source tools using afl-fuzz? If yes, please drop
me a mail at <lcamtuf@coredump.cx> once the issues are fixed - I'd love to
add your finds to the gallery at:

  http://lcamtuf.coredump.cx/afl/

Thanks :-)
