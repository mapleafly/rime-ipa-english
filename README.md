# rime-ipa-english
 [Rime](https://rime.im)输入法英语音标输入方案。

此方案主要采用常用字母或字母组合的发音来输入音标。

比如：发/æ/ 音的字母是a。在本输入方案中，输入a就会有æ可以备选。

比如：/ɪ/，某些单词中i、ey、y三个字母和字母组合在都可以发/ɪ/音。所以输入这三种字母和字母组合都可以打出/ɪ/。

**一些辅助符号的输入：**

* 音标中的冒号用键盘的冒号表示

* 重音符号用sb（上标简写）表示

* 次重音符号用xb（下标简写）表示



此音标输入方案兼容EPD-14（dj88 )、EPD-12和KK音标。

## 安裝

與其他依託Rime的輸入法一樣，國際音標是一組獨立發行的「輸入方案」數據包（或稱「配方」）。

安裝適合您的設備及操作系統的 [Rime輸入法](https://rime.im/download) 程序後，請按照以下說明，或借助「東風破」配置管理器，或以手動方式安裝、配置國際音標輸入法。

### 

### 手動安裝及配置

1. 從 [GitHub代碼庫](https://github.com/mapleafly/rime-ipa-english) 下載全部源碼的ZIP包，或單獨下載所需的YAML文件。

2. 打開Rime輸入法 [用戶文件夾](https://github.com/rime/home/wiki/UserData)，將下載的YAML文件移到此處。

3. 啓用英语音标輸入方案。

   在用戶文件夾創建或編輯文件 `default.custom.yaml`，將所需輸入方案的ID加入「輸入方案列表」配置項：

   ```
   patch:            # 若文件中已有該行，無須重複
     schema_list/+:  # 同上；"/+" 表示追加輸入方案，若無 "/+" 則表示以下列方案替換默認列表
       - {schema: ipa_english}   # 按需選配
   ```

4. 完成以上步驟之後，[重新部署](https://github.com/rime/home/wiki/CustomizationGuide#重新佈署的操作方法)Rime輸入法的工作數據，使上述配置改動生效。

## 

## 輸入英语音标

在Rime輸入法中按 `F4` 或 `Control+` ` 打開 [方案選單](https://github.com/rime/home/wiki/UserGuide#使用方案選單)，選取國際音標輸入方案，即可輸入對應編碼獲得音標符號。

運指齊按快捷鍵 `Control+Shift+1` 在最近使用的兩個輸入方案（如常用的中文輸入法和國際音標）之間相互切換。