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


4- LỆNH KHAI THÁC COIN:

**********************************************
***                COIN CCX               ***
**********************************************

Máy 01:CCX_M01_S9pX

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M01_S9pX --cpu-max-cpu-usage=80

Máy 02:CCX_M02_S9pH

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M02_S9pH --cpu-max-cpu-usage=80

Máy 03:CCX_M03_S9pH

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M03_S9pH --cpu-max-cpu-usage=80

Máy 04:CCX_M04_S9pX

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M04_S9pX --cpu-max-cpu-usage=80

Máy 05:CCX_M05_S9X

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M05_S9X --cpu-max-cpu-usage=80

Máy 06:CCX_M06_S10pT

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M06_S10pT --cpu-max-cpu-usage=80

Máy 07:CCX_M07_N8

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M07_N8 --cpu-max-cpu-usage=80

Máy 08:CCX_M08_S8pT

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M08_S8pT --cpu-max-cpu-usage=80

Máy 09:CCX_M09_A72017

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M09_A72017 --cpu-max-cpu-usage=80

Máy 10:CCX_M10_S9pH

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M10_S9pH --cpu-max-cpu-usage=80

Máy 11:CCX_M11_M30s

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M11_M30s --cpu-max-cpu-usage=80

Máy 12:CCX_M12_G2plx

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M12_G2plx --cpu-max-cpu-usage=80

Máy 13:CCX_M13_SH701sh

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M13_SH701sh --cpu-max-cpu-usage=80

Máy 14:CCX_M14_ZFlip1

    ./xmrigDaemon --cc-disabled --algo=cn/ccx --coin=CCX --url=sg.fastpool.xyz:10166 --user=ccx7bV23UMHC9ifXV9Q8m5hA58mrbMTPTZgq7krvugmN6jaERQTv2FuexMyZmYUGaqGf8jFJCCRyqVFDdvXv4N6zAKPcgNwgFw --pass=x --rig-id=CCX_M14_ZFlip1 --cpu-max-cpu-usage=80

**********************************************
***                COIN NOX               ***
**********************************************

Máy 01:NOX_M01_S9pX

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M01_S9pX --cpu-max-cpu-usage=80

Máy 02:NOX_M02_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M02_S9pH --cpu-max-cpu-usage=80

Máy 03:NOX_M03_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M03_S9pH --cpu-max-cpu-usage=80

Máy 04:NOX_M04_S9pX

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M04_S9pX --cpu-max-cpu-usage=80

Máy 05:NOX_M05_S9X

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M05_S9X --cpu-max-cpu-usage=80

Máy 06:NOX_M06_S10pT

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M06_S10pT --cpu-max-cpu-usage=80

Máy 07:NOX_M07_N8

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M07_N8 --cpu-max-cpu-usage=80

Máy 08:NOX_M08_S8pT

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M08_S8pT --cpu-max-cpu-usage=80

Máy 09:NOX_M09_A72017

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M09_A72017 --cpu-max-cpu-usage=80

Máy 10:NOX_M10_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M10_S9pH --cpu-max-cpu-usage=80

Máy 11:NOX_M11_M30s

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M11_M30s --cpu-max-cpu-usage=80

Máy 12:NOX_M12_G2plx

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M12_G2plx --cpu-max-cpu-usage=80

Máy 13:NOX_M13_SH701sh

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M13_SH701sh --cpu-max-cpu-usage=80

Máy 14:NOX_M14_ZFlip1

    ./xmrigDaemon --cc-disabled --algo=rx --coin=NOX --url randomx.rplant.xyz:7107 --user=PkZuzPuXfwZWnJ7AGVUR9j2MQYjfWf6cCMwSK7YA2WUNJ6GsJ8tiwEpPCCznTveySm6VjmGpLhXaFBw7wVgJdCNg12FDn9uDP --pass=x --rig-id=NOX_M14_ZFlip1 --cpu-max-cpu-usage=80
