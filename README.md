### AuroraStore

Inclui a Aurora Store (v4.8.4, código 76) como app de sistema pré-compilado no build.

### 1. Baixar os arquivos

```bash
mkdir -p vendor/aurora/AuroraStore && cd vendor/aurora && curl -fsSLO https://raw.githubusercontent.com/WhoFoss/LOSMG/LineageOS-22.2/AuroraStore/Android.mk && curl -fsSLO https://raw.githubusercontent.com/WhoFoss/LOSMG/LineageOS-22.2/AuroraStore/CleanSpec.mk && cd ../..
```

### 2. Baixar o APK

```bash
curl -fL -o vendor/aurora/AuroraStore/AuroraStore.apk https://f-droid.org/repo/com.aurora.store_76.apk
```

### 3. Registrar no device.mk

Em `device/xiaomi/sapphire/device.mk`:

```makefile
PRODUCT_PACKAGES += AuroraStore
```
