# XMRig-Termux


Bước 1: Tải xuống Termux.APK sau đó cài đặt
Bước 2: Mở Termux sau đó chạy các lệnh dưới đây
Bạn cần Update APT sau đó cài đặt Git và Cmake
```
apt-get update
apt-get install git (You will be asked to enter `y` after sending this command.)
pkg install cmake   (You will be asked to enter `y` after sending this command.)
```
Tiếp theo chúng ta sẽ clone xmrig từ nguồn phía dưới theo lệnh ở dưới luôn nhé

```
apt update 
apt upgrade  
git clone https://github.com/xmrig/xmrig.git 
cd xmrig
```
Trong quá trình cài đặt sẽ có nhiều lần hỏi bạn có cho phép hay không, hãy đồng ý bằng cách nhấn Y trên bàn phím rồi enter để chạy tiếp.
Sau khi hoàn tất quá trình bạn sẽ thấy kết quả như hình phía dưới

![image](https://user-images.githubusercontent.com/84473858/124390827-94fe8480-dced-11eb-9f5e-1d53497e8aa4.png)
``` 
mkdir build
cd build
cmake -DWITH_HWLOC=OFF .. 
```

![image](https://user-images.githubusercontent.com/84473858/124390943-430a2e80-dcee-11eb-95f0-2d2645faae26.png)

Sau khi chạy cmake, bạn cần 'make' nó. LƯU Ý: Bước này có thể mất một thời gian tùy thuộc vào điện thoại bạn đang sử dụng!
```
make
```
![image](https://user-images.githubusercontent.com/84473858/124390954-5f0dd000-dcee-11eb-8d4b-e47add3f8230.png)

Bây giờ bạn đã cài đặt xong mọi thứ. (Bạn có thể nhập clear để xóa màn hình để có cái nhìn tổng quan tốt hơn.)
Nhập ls và bạn sẽ nhận được một danh sách mọi thứ trong thư mục bạn đang ở.


![image](https://user-images.githubusercontent.com/84473858/124391996-a185db80-dcf3-11eb-8455-8c0360cffa20.png)

Nhập lệnh này sau đó nhấn Enter để bắt đầu máy đào.
Lưu ý: hãy sửa server mà bạn muốn đào từ Pool bạn cho là chân ái cuộc đời
À nhớ sửa địa chỉ ví của tui luôn đi nhé.
```
./xmrig -a rx/0 -o au.zephyr.herominers.com:1123 -u DIACHIVITHAYTAIDAY -p x -t 8
```
![image](https://user-images.githubusercontent.com/84473858/124391157-8f09a300-dcef-11eb-8294-144837e7b641.png)
