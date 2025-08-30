QUY TRÌNH LÀM VIỆC NHÓM CƠ BẢN VỚI GITHUB

TRƯỚC KHI BẮT ĐẦU LÀM CHỨC NĂNG MỚI:
git switch master //Chuyển sang nhánh master
git pull origin master //Lấy tất cả code từ nhánh master về local
git switch -c <ten_nhanh_moi> //Chuyển sang nhánh mới để phát triển chức năng mới
git merge master //Merge code từ master sang nhánh mới để đồng bộ code trước khi làm

SAU KHI LÀM XONG CHỨC NĂNG:
git add . //Thêm toàn bộ file đã làm để push lên nhánh mới
git status //Kiểm tra trạng thái (Có thể có hoặc không)
git commit -m "Your commit"
git push origin <ten_nhanh_dang_lam>

-> Sau đó tạo Pull Request(PR) trên github, trong nhóm review code trước khi xác nhận Merge Code từ
   nhánh mới sang nhánh chính (như trên là master)

SAU KHI PULL REQUEST ĐƯỢC MERGE
git switch master //Lúc commit ở trên thì đang ở nhánh bạn đang phát triển nên phải chuyển qua master
git pull origin master //Lấy code mới nhất từ nhánh chính về local để phát triển chức năng tiếp theo
git branch -d <ten_nhanh> //Xóa nhánh lúc nãy đã PR để gọn hơn
