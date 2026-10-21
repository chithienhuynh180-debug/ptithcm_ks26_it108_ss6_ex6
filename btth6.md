## 1. ipo
input → home, template.ps1
process → tạo thư mục, file và sao chép
output → thư mục smart-farm hoàn chỉnh

## 2. lệnh powershell

```powershell
mkdir ~/smart-farm/bin, ~/smart-farm/config, ~/smart-farm/data
New-Item ~/smart-farm/config/.env -ItemType File
attrib +h ~/smart-farm/config/.env
Copy-Item ~/Public/template.ps1 ~/smart-farm/bin/pump_control.ps1
ls ~/smart-farm -Recurse -Force
```

file .env bị ẩn nên dùng -Force để xem.

nếu lỗi quyền thì chạy powershell bằng administrator.
