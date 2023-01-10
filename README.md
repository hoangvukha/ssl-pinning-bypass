**Bypass**
- Tải file [frida-server](https://github.com/frida/frida/releases "frida-server") tương ứng với điện thoại.
- Giải nén và đổi tên thành frida-server.
- Mở terminal.
- Đẩy fille frida-server đã giải nén vào điện thoại (chỉ chạy lần đầu):
`adb push frida-server /data/local/tmp`
- Truy cập điện thoại:
`adb shell`
- Cấp quyền Superuser cho shell:
`su`
- Duyệt vào thư mục tmp:
`cd /data/local/tmp`
- Thay đổi quyền truy cập file frida-server (chỉ chạy lần đầu):
`chmod +x frida-server`
- Chạy frida-server ở foreground:
`./frida-server`
- Mở terminal mới.
- Cài đặt objection (chỉ chạy lần đầu):
`pip3 install objection`
- Bắt đầu ssl pinning bypass với momo:

`objection -g com.mservice.momotransfer explore`

`android sslpinning disable`

**Lấy request**
- Cài đặt [Charles](https://maclife.vn/charles-web-proxy-cho-mac.html "Charles")
- Kích hoạt bản quyền (name / key):

TEAM MESMERiZE / FC91D362FB19D6E6CF ;
mac / 0E03DBE6CF143C589C ;
macos / F3637014AD798E7E66 ;
zzz / 3406585A7C044747BF ;
zuishuai / 37356FB2CE3BC243AC ;

- Thay đổi Proxy Wifi của điện thoại:

-- Tên máy chủ: IP máy tính

-- Cổng: 8888

- Install certificate:

-- Tải về [charles-proxy-ssl-proxying-certificate](http://chls.pro/ssl "charles-proxy-ssl-proxying-certificate")

-- Android: Mở Wifi -> Lưa chọn ưu tiên về mạng -> Cài đặt chứng chỉ


