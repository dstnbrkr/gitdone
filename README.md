gitdone
=========================
Plan your commits


Purpose
-------

Found a bug in code unrelated to your pending commit? Plan the next commit with gitdone. Where `git log` displays past commits, gitdone is a list of future (planned) commits. Use gitdone to manage your next commit so you don't lose focus on the present.

Simple usage example:
---------------------

Plan a commit:

    $> gitdone add "Fix validation bug."

See planned commits:

    $> gitdone list
    Fix validation bug.
    Accept command line parameter
    Whitespace
 
See next commit:

    $> gitdone next
    Fix validation bug.

Execute next commit:

    $> gitdone commit
    # equivalent of 'git commit -am "Fix validation bug."'

Edit plan:

    $> gitdone edit
    # opens $EDITOR with list of planned commits for editing / reordering.




