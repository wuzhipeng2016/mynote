svn checkout https://wzpmachine:8443/svn/hehe/pa --username wzp --password 12345
svn checkout https://wzpmachine:8443/svn/hehe/pa papa --username wzp --password 12345

svn add a.txt
svn commit b.txt -m "test"
svn commit -m "" *.txt
--delete
svn delete a.txt
svn commit -m ""
--lock
svn lock b.txt
svn unlock b.txt

svn info b.txt
svn log b.txt
svn diff b.txt
svn diff -r 3:4 b.txt

svn mkdir newdir
svn mkdir -m "Making a new dir." svn://localhost/test/newdir 
注：添加完子目录后，一定要回到根目录更新一下，不然在该目录下提交文件会提示“提交失败”
svn update

svn list svn://localhost/test
svn revert --recursive .
