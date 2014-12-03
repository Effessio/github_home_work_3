github_home_work_3
==================
git init
echo -e 'line1\nline2\nline3\nline4' | git hash-object -w --stdin
git cat-file -p 84275f > task3.txt
git update-index --add --cacheinfo 10644 84275f9939456e87efd6932bdf7fe01d52a53116 task3.txt
git write-tree
echo "commit Effessio 1" | git commit-tree eed99f
echo -e 'line1\nline2' | git hash-object -w --stdin
git cat-file -p c0d0fb > task3_new.txt
echo -e 'newline_1\nnewline2\nnewline3\nnewline4' | git hash-object -w --stdin
git cat-file -p a57199 > task3.txt
git update-index --add --cacheinfo 10644 a57199abaff9a93e31d4cd74ca5beaa9c5293274 task3.txt
git update-index --add --cacheinfo 10644 c0d0fb45c382919737f8d0c20aaf57cf89b74af8 task3_new.txt
git write-tree
echo "commit Effessio 2" | git commit-tree 04c192 -p 7ac5d
git read-tree --prefix=gittask 7ac5d906a571265be41941108ee045ccab932465
git write-tree
echo "commit Effessio 3" | git commit-tree 7364f2 -p 6fb89c
echo "79f4d05435bb2eda989a73d53193a17ab8c642ca" > .git/refs/heads/master
f6255c8dc5862a44dad71313098bd4d8108ee08a
echo "f6255c8dc5862a44dad71313098bd4d8108ee08a" > .git/refs/heads/master
git remote add origin git@github.com:Effessio/github_home_work_3.git
git push -u origin master
