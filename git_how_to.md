
# Quy tắc chung
## I. Sử dụng 3 branches

- development
> dùng cho việc phát triển của team dev, bao gồm: new task, bug fix
- stagging
> dùng để build project để tester test
- master
> dùng cho việc release project

## II. Tạo branch cho từng task

Mội project chứa nhiều task lớn, mỗi task lớn có nhiều task nhỏ.
Việc tạo branch cho từng task nhỏ giúp việc quản lí task dễ dàng hơn, và hạn chế conflict khi merge code vào branch chính.

## III. Các lệnh git cơ bản

### 1. clone source code từ branch mặc định master					
	git clone URL				
					
### 2. tao branch cho rieng minh					
	git checkout -b asiantech_name				
					
### 3. gitignore
add file database, temp... ko cần thiết vào file .gitignore để tránh commit lên ảnh hưởng đến người khác					
					
### 4. Kiểm tra file đã sửa, chuẩn bị cho commit					
	git status -s				
					
### 5. git add
Chỉ add những file mình đã sửa và cần thiết để commit lên 

	git add path_file_1 path_file_2 ...				
					
### 6. git commit
commit các file đã add, cần ghi nội dung  rõ ràng, ví dụ "finish task #123", trong đó 123 là ID của issue trên Redmine

	git commit -m "finish task #123"				
					
### 7. git push					
	git push origin asiantech_name				
					
### 8. pull request
vào trang repository của project, gửi pull request de merge branch cua minh vao branch master

### 9. tiep tuc lam task khac

	git checkout master
	git pull origin master
	Quay lai buoc 2