# Chatbot
# Môi trường thực thi.
1. py -m venv env
2. .\env\Scripts\activate
3. conda create --name "tên" python=3.X
4. activate vào môi trường vừa tạo
4. Nang cap pip : conda install -c anaconda pip
5. cài rasa ( pip install rasa) hoặc rasa x : pip3 install rasa-x --extra-index-url https://pypi.rasa.com/simple
6. webchat : rasa run --model models --enable-api --cors "*"

# Cài đặt chatbot trên trang web
1. Trong code tải từ github index.html là trang web dùng dể test
2. Từ trang web ngẫu nhiên đoạn <script> </script> trong https://github.com/botfront/rasa-webchat, thay đổi địa api đến con chatbot của mình ( tùy theo các bạn đặt liên kết api , mặc định là socketUrl: "http://localhost:5005").
 - video kèm theo.
 - kèm theo bật action_endpoint: trong endpoints.yml nha.
3. Bật cmd lên, tùy theo môi trường các bạn tạo, ở đây mình tạo môi trường env.
- Cmd 1 : rasa run --model models --enable-api --cors "*" ,lệnh này chỉ chạy với môi trường base nha mn,vào trong môi trường của thư mục là sai nha (xem video ấy),lệnh ở đây load model từ model đã train của các bạn tương tự như rasa shell và hiển thị lên dấu tích chat.
- Cmd 2: rasa run actions nếu có action trong chatbot. 
- Mở trang index.html bằng trình duyệt và chat thử.
- video kèm theo.
Gook luck!!
Mọi người chú ý ! Từ Desktop/rasa là thư mục rasa chứa chatbot của mình nha.
- conda activate rasa ( Là mình tạo môi trường python ảo cho nó ngay từ đầu, để mọi người sau khi đã tạo chatbot mà thêm môi trường ảo mà error là tôi không chịu trách nhiệm ^^)
- conda activate ( Đối với run model ... để khởi động api của chatbot nha, là môi trường base đó. Chú ý nha!!) Thanksfor!!
Hi vọng giúp được mọi người.
