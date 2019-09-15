

Undo code for uncoomitted file changes
---------------------------------------
```
	git status
	git checkout -- modifiedFile1.py
	<or>
	git checkout -- modifiedFile1.py modifiedFile2.py modifiedFile3.py ...
	<or>
	git checkout -- .
```



Undo (and commit chhanges) code for comitted file changes
---------------------------------------------------------

========================================
Tip: use [git -am""] to skip add . step
========================================

```
	git log
	git revert <commit_id_from log>

	[use :q to quit terminal window]
```


Undo (but do not commit changes) code for comitted file changes
---------------------------------------------------------------
```
	git revert -n <commit_id_from log>

	[Explicitly commit changes]
```



Reset all undos
----------------
```
	git reset --hard commit_id
```
