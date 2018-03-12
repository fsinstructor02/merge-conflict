# Example of resolving merge conflicts in git

1. Partner with the person next to you. One partner is partner A the other is partner B.
1. Partner A and partner B both fork the hussian-merge-conflict repository.
1. Both partners clone both forks of the repository. Each partner should have a hussian-merge-conflict-A and
1. hussian-merge-conflict-B repository on their local machine.
1. Partner A changes bullet 1 of the README in hussian-merge-conflict-A to read “Partner with the person behind you.”. Partner A commits this change and push it back to origin.
1. Partner B changes bullet 1 of the README in hussian-merge-conflict-A to read “Partner with person in front of you.”. Commit this change to the local clone.
1. Partner B ensures partner A has completed step 4. Now, perform a git pull. Git will now inform you that you have a merge conflict. Use the git status command to see the 
1. file in conflict. Resolve the conflict by editing the line to read “Partner with a person near you.”.  After editing, `git add` the file and commit it.
1. Partner B changes bullet 1 of the README in hussian-merge-conflict-B to read “Partner with the person behind you.”. Partner B commits this change and push it back to origin.
1. Partner A changes bullet 1 of the README in hussian-merge-conflict-A to read “Partner with person in front of you.”. Commit this change to the local clone. 
1. Partner A  ensures partner B has completed step 4. Now, perform a git pull. Git will now inform you that you have a merge conflict. Use the git status command to see 
   the file in conflict. Resolve the conflict by editing the line to read “Partner with a person near you.”.  After editing, `git add` the file and commit it.



### How do you know what line changed?

    <<<<<<<: Indicates the start of the lines that had a merge conflict. The first set of lines are the lines from the file
    that you were trying to merge the changes into.
    =======: Indicates the break point used for comparison. Breaks up changes that user has committed (above) to changes
    coming from merge (below) to visually see the differences.
    >>>>>>>: Indicates the end of the lines that had a merge conflict.  


###Test