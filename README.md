# hocviencnttgittutorial
========================================================================

	     Exercise
	     
========================================================================

A va B la 2 developer lam viec tren 1 git repository https://github.com/levunguyen/hocviencnttgittutorial

Product gom co 3 chuc nang register,login,va profile

A pull code tu git ve thu muc developer A

	 git clone https://github.com/levunguyen/hocviencnttgittutorial
	 
A tao branch register

	git checkout –b register
	
A switch qua branch register

A viet code va commit 2 files : register.html va register.java len branch register

	git commit -m “register”
	
A push branch register len  git

	git push origin register
	
B pull code tu git ve thu muc developer B

	 git clone https://github.com/levunguyen/hocviencnttgittutorial
	 
B tao branch login

	git checkout –b login
	
B switch qua branch login

B viet code 2 files : login.html va login.java len branch login

	git commit -m “login”
	
B push branch login len git

	git push origin login
	
Technical lead reviews 2 commits roi merge vao master

A va B ve lai banch master

	Git checkout master
	
A va B lay code moi nhat ve

	Git pull
	
Kiem tra source cua a va b de co 4 files : logn.html,register.html,login.java,register.java

A va B cung o cùng ở trên branch master

A tạo file profile.html và enter dong profile

A commit code lên git, A cung vi lai cai fifle profile trong html

B pull code mới có profile ve

B chỉnh sửa dong số 1 chủ profile thanh profile name

B commit lên git

A them 1 dong code nữa happy

A commit lên git thi git yêu câu chạy lên pull trước khi push

A pull code về thì nhận được thông báo conflict tại file 

Auto-merging profile.html

CONFLICT (content): Merge conflict in profile.html

Automatic merge failed; fix conflicts and then commit the result.


A gedit file profile.html và sửa lại conflict

	<<<<<<< HEAD
	
profile

happy

=======

Profil

>>>>>>> 65961fa05f24158e0174ca433baac43ca145b25a

	Phần ở trên dấu ==== là của local của A. Phần ở dưới là của git
	
A remove phần conflict sau đó commit len git

	$ git add profile.html
	$ git commit -m "merge"

Sau một thời gian chaỵ thì phát hiện chứ năng login ko quan trong và muốn bỏ đi

A checkout vao branch master

A thực hiện revert tai commit login

	git revert 03b6223
	
Sau do A push len git

	git push 
	
Sau 1 thoi gian thi thay can co chuc nang login

A vào git web site và lấy cái git number của commit revert (9cce53b)
	
Sau do A chay lenh revert voi commit id

	git revert 9cce53b
	
A Push len git lai

	git push
	
=========================================================================

Rebase 

=========================================================================


Developer A pull code tu master ve

Developer A create a branch home

Developer A commit files home.html, home.js, home.css len branch

Developer B commit 1 file profile.css

Developer A switch to master branch

Developer A pull ve cai moi nhat tu master

Developer A switch nguoc lai brach home

Developer thu hien lenh rebase

git rebase –i master

Developer A push branch len master


