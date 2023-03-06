Readers-Writers problem is a problem of process synchronization in operating systems. Here, a file is shared between many people. If one person edits the file, then no other person should be reading or writing at the same time. Otherwise, if a person is reading a file, then other people may also read it at the same time. In the first readers-writers problem, Readers are given more priority over writers. So, the writers starve. In second readers-writers problem, No writer should wait in the queue than necessary time. So here writers are given more priority and eventually readers starve. Therefore, in third readers-writers problem the solution is such that none of the readers or writers are given priority.This is a starve free solution.
In this solution,a reader currently reading the file will allow other readers next to it in the queue also to read. But a writer will not allow any process in the queue  while it is writing. Readers or writers will enter in first in first out order. This is maintained by the semaphore mutex. So, here neither readers or writers are given priority. Therefore, this is starvation free.
