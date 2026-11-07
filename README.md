# Luyện trắc nghiệm từ PDF

## Đưa lên Vercel
1. Tạo repo GitHub, đẩy cả thư mục này lên (index.html, api/solve.js, vercel.json, package.json).
2. Vào vercel.com → Add New → Project → chọn repo → Deploy (không cần build).
   Hoặc dùng CLI: `npm i -g vercel` rồi chạy `vercel --prod` trong thư mục này.

## Bật tính năng "AI giải đáp án" (tuỳ chọn)
Trong Vercel → Project → Settings → Environment Variables, thêm:
- ANTHROPIC_API_KEY: khoá API của bạn (bắt buộc nếu muốn dùng AI)
- SOLVE_PASSCODE: mật khẩu tự đặt, tránh người lạ dùng hết tiền API của bạn (nên đặt)
- ANTHROPIC_MODEL: tên model (không bắt buộc, mặc định claude-sonnet-5-5)
Sau đó bấm Redeploy.

Không có các biến này thì web vẫn chạy bình thường, chỉ là phải tự nhập đáp án.
