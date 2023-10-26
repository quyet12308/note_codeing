# Đây là phần note khi sử dụng docker 

## Build docker image
- Trước khi build docker image thì nên chú ý đến các các thư viện trong dự án , cái nào dùng thì hãy cho vào tránh nặng docker image . Và đặc biệt nên sử dụng .dockerignore để giảm gánh nặng .
- Khi build thì cũng cần chú ý đến sung đột thư viện do docker chạy trên linux mà mình lại thường dùng windown

## Docker run
- Nên thêm các cái cờ này vào : 
```cmd
--cpus 2.5 --memory 4g --restart
```
always để hạn chế việc project ăn quá nhiều tài nguyên và để nó tự động chạy khi server được khỏi động lại