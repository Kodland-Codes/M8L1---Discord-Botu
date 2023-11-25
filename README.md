# m8l1

## Sanal Ortam
Sanal ortam oluşturmak için bunları VSCode'daki terminalinize yazınız:

```
python -m venv <ortamın_ismi>
source <ortamın_ismi>/bin/activate
```
Terminalde solda parantez içinde ortamınızın ismini görüyor olmanız lazım.
Ortamınızın ismini venv olarak koyduğunuzu varsayalım, o zaman terminaldeki yazının böyle olması gerekiyor: 

```
(venv) cando@galaxy-a32-5g m8l1 %
```

## GitHub'ta yeni depo oluşturmak ve local'deki klasörlerinizi Github'taki depoya yüklemek için:

1. Yeni depo oluşturun, README olmadan.
2. SSH Linkini kopyalayınız
3. Bu komutları giriniz:
```
echo "# My Repository" >> README.md
  git init
  git add README.md
  git commit -m "first commit"
  git branch -M main
  git remote add origin git@github.com:cando-jo/test.git
  git push -u origin main
```



## Local'de yaptığınız değişiklikleri GitHub'a yüklemek
Projenizi güncelledikten sonra her zaman yaptığınız değişiklikleri Github'a yüklemeniz gerekiyor, aşağıdaki komutları yazarak Github'a deponuzu yükleyebilirisiniz.:

```
git add .
git commit -m "Yaptığınız değişiklikle ilgili bir yorum, örneğin: !merhaba komutu eklendi"
git push origin main
```

## Kullandığınız ortamdaki kütüphanedeki dondurmak için:
Doğru ortamı kullandığınızdan emin olun ve terminalde bunu yazınız:
```
pip freeze > requirements.txt
```

### Sanal ortamdaki kütüphaneleri indirmek için
1-Doğru ortamı kullandığınzdan emin olun
2-Bu komutları terminale yazınız
```
pip install -r requirements.txt
```
