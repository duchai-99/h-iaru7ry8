# Phần 1:

Input của hệ thống bao gồm các cảm biến có nhiệm vụ đo đạc các thông số môi trường vi khí hậu trong nhà lưới trồng lan và chuyển đổi thành tín hiệu điện để vi điều khiển xử lý.
Output là các thiết bị thực thi nhận tín hiệu từ bộ điều khiển trung tâm để thay đổi trạng thái môi trường trong trang trại.
git clone <repository-url> cd code
python -m venv venv .\venv\Scripts\Activate.ps1
python3 -m venv venv source venv/bin/activate
pip install -r requirements.txt
python main.py
.\scripts\deploy.ps1
lưu ý 
Get-Process python | Stop-Process -Force
Get-ChildItem -Path "logs/" -Recurse | Select-Object Name, Length
Get-Content -Path "logs/app.log" -Tail 50
Remove-Item -Path "logs/*.log" -Force
