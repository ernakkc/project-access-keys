# Proje Erişim Anahtarları


Bu proje, uzaktan erişim anahtarlarını (access keys) saklamak ve yönetmek için oluşturulmuştur. Anahtarları raw olarak erişerek, yaptığınız uygulamaların çalışmasını engellemek veya geri çalıştırmak için kullanabilirsiniz.

## Amaç

- Uzaktan erişim anahtarlarını merkezi bir yerde saklamak.
- Uygulamaların çalışmasını kontrol etmek için anahtarları etkinleştirmek/devre dışı bırakmak.
- Kişisel projeler için hızlı erişim sağlamak.

## Kullanım

1. **Anahtar Dosyaları**: `clinic-app-access-key.txt` gibi dosyalar, erişim anahtarlarını içerir.
2. **Raw Erişim**: GitHub üzerinden raw URL kullanarak anahtarları doğrudan erişebilirsiniz (örneğin: `https://raw.githubusercontent.com/ernakkc/project-access-keys/main/clinic-app-access-key.txt`).
3. **Uygulama Kontrolü**: Anahtarları kullanarak uygulamalarınızı engelleyebilir veya çalıştırabilirsiniz. Örneğin, bir anahtar eksik olursa uygulama çalışmayabilir.

## Kullanım Örneği
#### Raw URL ile erişim:
   - Tarayıcıda: `https://raw.githubusercontent.com/ernakkc/project-access-keys/main/clinic-app-access-key.txt`
   - Kodda: Python örneği
     ```python
     import requests

     url = "https://raw.githubusercontent.com/ernakkc/project-access-keys/main/clinic-app-access-key.txt"
     response = requests.get(url)
     key = response.text.strip()
     print(f"Anahtar: {key}")
     ```

4. Uygulama kontrolü: Anahtarı kullanarak uygulamanızı kontrol edin. Örneğin, anahtar yoksa uygulamayı durdurun.

## Katkıda Bulunma

- Bu depo kişisel kullanım içindir.
- Sorularınız için issue açabilirsiniz.

