
# 在 Ubuntu 18.04.1 的 IBus 上安裝大易輸入法

### 下載安裝腳本
```
$ wget https://raw.githubusercontent.com/Alger23/ubuntu_dayi_for_ibus/master/dayisetup.sh
```

### 下載大易三碼字根檔
```
$ wget https://raw.githubusercontent.com/Alger23/ubuntu_dayi_for_ibus/master/dayi3.cin
```

### 執行安裝腳本
```
$ chmod u+x dayisetup.sh
$ sudo ./dayisetup.sh
```

### 直接執行Python腳本

用此方法可直接取代上述三步:
```
$ curl https://raw.githubusercontent.com/Alger23/ubuntu_dayi_for_ibus/master/dayisetup.sh | sudo python3
```

### ibus 設定大易輸入法

```
$ ibus-setup
```

* 經由 ibus-setup 指令開啟的 ibus 設定畫面

![ibus 設定畫面](images/dayi/010_ibus-setup.png)

* 切換到 Input Method 頁籤

![ibus-input method](images/dayi/020_ibus-setup-inputmethod.png)

* 選取 Chinese

![ibus-add input method](images/dayi/030_ibus-setup-addinputmethod.png)

* 選取 dayi，按下 【Add】

![ibus-add dayi](images/dayi/040_ibus-setup-selectdayi.png)

* 選取 Chinese-dayi ，設定【Preferences】

![Preferences](images/dayi/050_ibus-setup-inputmethoddayi.png)

* 將 Chinese mode: 設定為 Traditional Chinese，按下【Close】

![Chinese Mode = Traditional Chinese](images/dayi/060_ibus-setup-dayi-preferences.png)

* IBus Preferences 畫面再按下【Close】，完成 ibus 的大易輸入法設定

* 右上角的小工具，展開，選擇設定(Settings)。

![Settings](images/dayi/070_region-language-topright.png)

* 選取區域和語言(Region & Language)，在輸入來源(Input Sources)點選「加號」

![Select Plus Symbol Button](images/dayi/080_region-language-manage-language.png)

* 選擇輸入來源為「Chinese (Taiwan)」

![Select Taiwan](images/dayi/090_region-language-select-chinese-taiwan.png)

* 選擇 Chinese (dayi)，然後按下【Add】

![Select dayi](images/dayi/100_region-language-add-dayi.png)

* 此時可以在 Input Sources 的區域看到新加入的大易輸入法「Chinese (dayi)」，關閉此視窗

![dayi](images/dayi/110_region-language-close.png)

* 在右上角的輸入法已經能切換至大易輸入法了

![input method](images/dayi/120_region-language-dayi-done.png)


## 己知打不出來的字

如果在 Chinese mode 選擇繁體中文，已知下列字打不出來

```
/mo 向
o8  只
```

所以將 Chinese mode 選擇 All Chinese Characters，字會出來但排序不同

![chinese mode](images/dayi/130_ibus-chinese-mode.png)


## 已知問題

* 無法用 '[]-\ 選字，要用 Ctrl + 數字
* 

