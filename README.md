# GitHub Pages – Doodle Animate

Bu klasördeki dosyaları `yilmaz0emre.github.io` adlı yeni bir **public** GitHub reposuna yükleyin.

## Klasör yapısı

```
yilmaz0emre.github.io/          ← repo adı (tam olarak bu olmalı)
├── share/
│   └── index.html              ← landing page
└── .well-known/
    ├── apple-app-site-association
    └── assetlinks.json
```

## Eksik değerleri doldurma

### 1. apple-app-site-association
`YOURTEAMID` → Apple Developer hesabınızdaki 10 haneli Team ID
- developer.apple.com → Membership → Team ID

### 2. assetlinks.json
`REPLACE_WITH_YOUR_SHA256_FINGERPRINT` → Keystore SHA-256 parmak izi
```bash
keytool -list -v -keystore android/app/upload-keystore.jks -alias upload
```
Çıktıdan `SHA256:` ile başlayan satırı alın.

### 3. index.html
`YOUR_IOS_APP_STORE_ID` → App Store Connect'teki numerik uygulama ID'si
(örn. `https://apps.apple.com/app/id1234567890`)

## Paylaşım linki formatı

```
https://yilmaz0emre.github.io/share/?v=<generationId>
```
