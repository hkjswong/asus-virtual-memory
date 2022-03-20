# 沒有高速讀寫能力的U盤是不是就不能開啟虛擬內存了？

AC86U創建虛擬內存時對優盤的要求是读取速度要求 20M/s，写入速度要求 30M/s。可是怎麼買都買不到速度這麼快的U盤怎麼辦？ 我們可以手動將要求調低即可


### 修改写入速度限制，30替换为10
> sed -i 's/^W_LIMIT=30/W_LIMIT=10/' /koolshare/scripts/swap_make.sh

### 修改读取速度限制，20替换为10
> sed -i 's/^R_LIMIT=20/R_LIMIT=10/' /koolshare/scripts/swap_make.sh

### 聯繫方式 :bell:

- Telegram：https://t.me/xwring :point_left:
- 個人telegram:https://t.me/kwaong 👈
- 我的博客（新的,舊的被封了):https://kwaon.wordpress.com/ 👈
- :email: hello@lwky.com.hk :point_left:
- Facebook粉專：https://www.facebook.com/jsrwon :point_left:
- 微信公眾號 :point_down:

![image](https://github.com/hkjswong/shadowsocksR-setup/blob/master/%E5%BE%AE%E4%BF%A1%E5%85%AC%E7%9C%BE%E8%99%9F.jpg)
