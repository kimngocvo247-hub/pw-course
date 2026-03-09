# Lesson 3: Git and JavaScript (Continue)

This file is created to note down the major points in Lesson 3. 

## 1. Git Knowledge
### Goal: 
1. how to change the commit message when the commit is incorrectly sent. 
2. Un-stage a file (from staging to working directory)
3. Un-commit
    1. from repository from staging
    2. from repository to working directory

### Remember: Un-stage
1. **git commit --amend -m"latest message"**
Vd: Minh muon doi file5 thanh file6 => 
git commit --amend -m"feat: add file6.txt"

2. **git restore --staged <file name>**
Vd git restore --staged file5.txt
Dem file5 tu staging ve working directory

3. **git restore --staged .** 
Dem tat ca cac file tu staging ve working directory

### Remember: Un-commit
1. **git reset --soft HEAD~1**
Dua 1 commit gan nhat (latest) tu repository ve staging

2. **git reset HEAD~1**
Due 1 commit gan nhat (latest) tu repository ve working directory

3. **Vd muon dua 2 hay 3, 4, 5... commit gan nhat ve thi thay doi so 1 thanh 2**
git reset --soft HEAD~2
git reset HEAD~2

### Remember: Branching
1. Branch is a pointer to a commit

2. **git branch**
Dung de xem danh sách nhánh, cần có ít nhất 1 nhánh thì mới hiện danh sách nhánh

3. **git branch ngoc/product**
Tạo nhánh, chưa đi đến nhánh đó

4. **git checkout <branch name> => git checkout ngoc/product**
Đi đến nhánh đó

5. **git checkout -b ngoc/product** => vừa tạo nhánh, vừa chuyển sang nhánh mới tạo

6. **git branch -D <branch name> => git branch -D ngoc/product**
Xoa nhánh, lưu ý phải đứng ở nhánh khác mới xóa được, không xóa được nhánh mình đang ở

7. **git push origin <branch name> => git push origin ngoc/product**
đưa nhánh lên online (remote)

8. **git push -D origin <branch name> => git push -D origin ngoc/product**
xóa nhánh online (remote)

6. **git status** => xem status hiện tại ở git

7. **git log** => xem lại log

## 2. JavaScript Knowledge
### Remember: Conditional Type
`
let a = some value;
**if (condition) {
    do something
}**

let a = 9
if ( a > 10) {
    console.log("Welcome")
}
`

### Loop
** for (dieu kien khoi tao; dieu kien lap; cap nhat) {code gi do} **

for ( let i = 0; i <5; i++) {
    console.log("Xin chao!")
}


