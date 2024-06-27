<p align="center">
  <p align="center">
    <a href="https://www.youtube.com/channel/UC7m0x5NHiHz4VemPFVaS98A" target="_blank">
      <img src="https://raw.githubusercontent.com/codingforinnovations/Django-on-Vercel/main/.static/Logo-Light.png?token=GHSAT0AAAAAABXU4AJBD6OH7Z33MGA7X2EYY3HPGAA" height="72" />    
    </a>
  </p>
  <p align="center">
    For Programmers, By Programmers.
  </p>
</p>

# Django with Vercel

This repository is the final code for the Django with Vercel Project Demo.

---

## Running the Project

**Step 1** . Vào trang [Fire base](https://firebase.google.com/), sau đó tạo kho lưu trữ ảnh cho ứng dụng như sau:

  - Nhấn `Go to console` phía trên bên phải màn hình
    
  ![image](https://github.com/anhhducnguyen/Django-on-Vercel/assets/97099707/9dfcdce6-b0fd-4b0a-b510-d91a93227061)

  - Thêm dự án
    
  ![image](https://github.com/anhhducnguyen/Django-on-Vercel/assets/97099707/a285d19d-cadb-4f71-ac31-da9ae76fea01)

  - Tạo dự án
    
  ![image](https://github.com/anhhducnguyen/Django-on-Vercel/assets/97099707/87134ee8-9d0e-4726-9ed2-8b5e604d9759)

  - Tạo thành công
    
  ![image](https://github.com/anhhducnguyen/Django-on-Vercel/assets/97099707/43e1decd-2049-417b-b173-4c1cb049843e)

  - Nhấn tiếp tục và cuộn xuống chon `Storage`, sau đó nhấn `Get started` hiển thị `Set up Cloud Storage`

    Secure rules for Cloud Storage: chọn `Start in production mode`
    
    Set Cloud Storage location: Giữ nguyên

    Nhấn `Done`, và kết quả như hình dưới

    ![image](https://github.com/anhhducnguyen/Django-on-Vercel/assets/97099707/ffcb3449-c483-4fe1-8151-358bd353d3f0)

  - Trên icon `Setting`, chọn `Project settings` sau đó chọn `Generate new private key` để tạo kết nối và tải file `json`

    ![image](https://github.com/anhhducnguyen/Django-on-Vercel/assets/97099707/f8448bf8-188d-4d87-9bef-9b06d59be80c)

  - Ở link của dự án, mẫu của tôi `https://console.firebase.google.com/u/0/project/test-7b47d/storage/test-7b47d.appspot.com/files` hãy sao chép `test-7b47d.appspot.com` để tùy chỉnh trong file `settings.py` của dự án
    
    ```
    cred = credentials.Certificate('authentication.json')
    firebase_admin.initialize_app(cred, {
        'storageBucket': 'authentication-28e57.appspot.com'
    })
    ```


     



 

#### Create a Folder & Clone the Repository.
```
mkdir ~/Dev/django-on-vercel
cd ~/Dev/django-on-vercel
```

#### Create A Virtual Environment.
```
python3.9 -m virtualenv .
```

#### Activate the Virtual Environment.
```
source bin/activate
```

**In Windows use `.\Scripts\activate`**

#### Install Required Dependencies 
```
pip install -r requirements.txt
```

#### Make Migrations
```
python manage.py migrate
```

#### Run the Server
```
python manage.py runserver localhost:8000
```

_Open [localhost:8000](http://localhost:8000) in Your Browser_


<div align="center">
<i>Other places you can find us:</i><br>
<a href="https://www.youtube.com/channel/UC7m0x5NHiHz4VemPFVaS98A" target="_blank"><img src="https://img.shields.io/badge/YouTube-%23E4405F.svg?&style=flat-square&logo=youtube&logoColor=white" alt="YouTube"></a>
</div>
