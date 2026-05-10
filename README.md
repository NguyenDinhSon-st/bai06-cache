# Bài 6: CI/CD Pipeline Optimization & Caching

## Cấu hình cache
Workflow sử dụng `actions/setup-java@v4` với `cache: 'maven'`.

## Kết quả thực nghiệm
(Sẽ cập nhật sau khi push 2 lần)

Lần push 1 (không cache) 
Thời gian: 21s
Cache hit: maven cache is not found

## Minh chứng log
Lần 1 : 
Lần 2 : 