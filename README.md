
gitdone
A todo list for git commits.

Simple usage example:

$> gitdone add "Fix validation bug."
$> gitdone list # outputs "Fix validation bug."

... make source code changes until ready to commit ...

$> gitdone commit # equivalent of 'git commit -am "Fix validation bug."'
$> gitdone list # No tasks.

Purpose:

gitdone provides a way to keep a todo list of commits you plan to make. Each entry (made with 'gitdone add <task>') becomes the commit message when 'gitdone commit' is used. 'gitdone list' lists all the tasks. The topmost task is the current task. It is the default commit message for 'gitdone commit', however any task can be specified by line number. For example:

$> gitdone add "task a"
$> gitdone add "task b"
$> gitdone add "task c"
$> gitdone list
0 task a
1 task b
2 task c

$> gitdone commit 2 # uses 'task c' as the commit message.

gitdone provides context. Interrupted? 'gitdone top' tells you what you're working on. Want to see what's next? 'gitdone list' shows all of your tasks. Need to re-prioritize? 'gitdone edit' opens your task list in your editor of choice.
 




