# 🧺 Stable Diffusion Lab

Stable Diffusion Lab'a hoş geldin! Bu proje, güçlü Stable Diffusion v1.5 modelini kullanarak metin girdilerinden etkileyici görseller oluşturmanı sağlayan, Google Colab tabanlı bir çalışmadır. Proje, GPU hızlandırması sayesinde yüksek performansla çalışır.

---

## 🔧 Setup

1. Notebook'u klonla ya da Google Colab üzerinde aç.
    ```python
    !pip install diffusers transformers accelerate scipy safetensors
    ```
2. Hugging Face'e giriş yap:
    ```python
    from huggingface_hub import notebook_login
    notebook_login()
    ```

---

## 🧑‍💻 Hugging Face Access Token Nasıl Alınır?

Stable Diffusion modelini kullanabilmek için Hugging Face'den bir erişim token'ı alman gerekiyor.  
Aşağıdaki adımları takip ederek kolayca token oluşturabilirsin:

### 🏃‍♀️ 1. Hugging Face'e Git

[https://huggingface.co](https://huggingface.co) adresine gidip hesabına giriş yap.

![Adım 1](assets/resim1.png)  
*Ayarlara tıkla*

### ⚙️ 2. Access Tokens Sayfasına Git

Açılan menüde **"Access Tokens"** sekmesine tıkla.

![Adım 2](assets/resim2.png)  
*Access Tokens'a tıkla*

### ⚡ 3. Yeni Token Oluştur

**"New token"** butonuna tıklayarak yeni bir token oluştur.

- **Role** kısmını `read` olarak seç ve token’a bir isim ver (örneğin: `stable-diffusion`).

![Adım 3](assets/resim3.png)  
*Read'ı seç ve isim gir*

### ➕ 4. Token'ı Oluştur

Token adını belirledikten sonra **Create Token** butonuna tıkla.

![Adım 4](assets/resim4.png)  
*Token adı "stable-diffusion" olabilir ve Create Token’e tıkla*

### ✅ 5. Token’ı Kopyala

Oluşturduğun token’ı kopyala ve ardından **Done** butonuna tıkla.

![Adım 5](assets/resim5.png)  
*Access token’i kopyala ve Done’a bas*

### 💻 6. Colab Üzerinde Giriş Yap

Notebook’ta aşağıdaki kodu çalıştır:

```python
from huggingface_hub import notebook_login
notebook_login()
 ```
### Token'ı Yapıştır

![Adım 6](assets/resim6.png)
kopyaladığın token'ı bu ekrana yapıştır.

