# gradle-livelock
Simple gradle project to show that Buildship's Eclipse project importer is livelocked, if two subprojects configure the Eclipse project name to be the same (i.e. not the gradle project name).

To see this in action, simplay import the project tree into Eclipse using Buildship. The process will simply hang and continue to consume CPU cycles.

See [stackdump.txt] for an example of `jstack` output for the gradle process in question.
