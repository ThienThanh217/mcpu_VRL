**********************************************************************************
*** Danh Sách Lệnh cài đặt tools xmrigcc miner để đào tất cả các coin chạy cpu ***
**********************************************************************************
*** Các lệnh phụ trợ tham khảo:

    rm -f [Tên File Cần Xóa]
    
    rm -r [Tên Thư Mục Cần Xóa]
    
    mrdir [Tên Thư Mục Cần Tạo]
    
    mv [Tên File Muốn Đổi] [Tên File Mới]

**********************************************************************************
0- Lệnh Cấp Quyền Admin

    sudo su

1- Tập lệnh hệ thống update:

    apt-get update -y 
    apt-get upgrade -y
    apt-get install wget 
    apt-get install get 
    apt-get install nano
    apt-get install git -y

2- Tải và cài đặt ứng dụng xmrigcc để khai thác coin:

    git clone https://github.com/ThienThanh217/mcpu.git
    cd mcpu
    tar xvaf xmrigcc-miner-arm-android-3.4.6.tar.gz
    chmod u+x xmrigDaemon
    chmod u+x xmrigMiner
    chmod +x config.json

3- Chỉnh sửa tập tin " config.json "  trước khi khai thác:

--cc-disabled : Vô hiệu hóa tính năng CC Client
--algo=ALGO : Gán thuật toán cần đào
--coin=COIN : Gán tên coin cần đào
--url=URL : Gán địa chỉ và cổng pools hồ khai thác coin
--user=USERNAME : Gán địa chỉ ví để tra coin khai thác về
--pass=PASSWORD : Gán mật khẩu của pools hồ khai thác nếu có, mặc định không có sẽ là "x"
--rig-id=ID : Gán tên thợ đào cho tứng máy nếu bạn có nhiều hơn 1 máy để tiền khai thác
--cpu-max-cpu-usage=N : Gán số cpu để khai thác (Theo %, ví dụ bạn có 8 cpu nhưng bạn chỉ muốn chạy 6 cpu thôi thì [N= 100* 6/8] (%) )


4- Lênh Khai thác coin VRL:

Máy 01:VRL_M01_S9pX

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M01_S9pX --cpu-max-cpu-usage=80

Máy 02:VRL_M02_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M02_S9pH --cpu-max-cpu-usage=80

Máy 03:VRL_M03_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M03_S9pH --cpu-max-cpu-usage=80

Máy 04:VRL_M04_S9pX

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M04_S9pX --cpu-max-cpu-usage=80

Máy 05:VRL_M05_S9X

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M05_S9X --cpu-max-cpu-usage=80

Máy 06:VRL_M06_S10pT

./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M06_S10pT --cpu-max-cpu-usage=80

Máy 07:VRL_M07_N8

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M07_N8 --cpu-max-cpu-usage=80

Máy 08:VRL_M08_S8pT

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M08_S8pT --cpu-max-cpu-usage=80

Máy 09:VRL_M09_A72017

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M09_A72017 --cpu-max-cpu-usage=80

Máy 10:VRL_M10_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M10_S9pH --cpu-max-cpu-usage=80

Máy 11:uVRL_M11_M30s

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=uVRL_M11_M30s --cpu-max-cpu-usage=80

Máy 12:VRL_M12_G2plx

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M12_G2plx --cpu-max-cpu-usage=80

Máy 13:VRL_M13_SH701sh

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M13_SH701sh --cpu-max-cpu-usage=80

Máy 14:VRL_M14_ZFlip1

    ./xmrigDaemon --cc-disabled --algo=rx --coin=VRL --url=sg.luckypool.io:4117 --user=v226zkgvqq38d4z9hdfhvacizb5jw726lopf7koe48x --pass=x --rig-id=VRL_M14_ZFlip1 --cpu-max-cpu-usage=80

