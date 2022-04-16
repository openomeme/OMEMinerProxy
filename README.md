# OMEMinerProxy

礦場直連隧道.無需任何中轉服務器.屏蔽内核抽水,從此告別抽水代理。

僅需要簡單步驟實現直連礦池。

# 安裝要求

1.擁有雙網卡的X86設備。

1.大於2Gb儲存設備。

# 如何安裝

# windows

1.通過balenaEtcher-Portable-1.5.110寫入到儲存器。

2.或者，您可以使用Rufus作為編寫工具。

# 如何使用

將網綫插入設備LAN口,在瀏覽器中輸入後臺管理ui,地址爲10.254.10.1. 用戶名:root 密碼:password

進入後臺點擊網絡>接口>WAN>修改,將"DHCP客戶端"修改為"靜態地址"填寫上級路由器ip地址,dns服務器要改爲防污染DNS"8.8.8.8"

第一次使用請點擊:

礦工代理> 訂閲設置> 保存并開始訂閲

礦工代理> 高級設置> 啓用自動切換

礦工代理> 高級設置> 更新礦池數據庫

礦工代理> 高級設置> 更新中轉數據庫


在基本設置中 主服務器為選擇您使用的隧道地址,運行模式 一般選擇中轉礦池模式 ,如需直連礦池,請選擇直連礦池模式+高級設置中的開啓内核屏蔽設置  一般用戶不推薦選擇屏蔽内核模式,選擇該選項會無法訪問網頁.

# 注意事項

如果按照以上方法操作后,在控制台下方四個圖標變爲彩色説明已經鏈接到挖礦隧道.如果仍顯示灰色,請更換主服務器地址測試,如仍無法鏈接請加入我們的電報群組咨詢。

電報討論群:https://t.me/+MuHbULYW2DZmNTkx


# 已知問題

1.部分輕鬆礦工會提示錢包地址錯誤(解決方案:在礦工代理>高級設置>内核屏蔽設置 取消勾選内核屏蔽)

2.GMiner 在windows中GMiner會開啓抽水綫程,這樣做會暴露用戶的真實ip地址,已做屏蔽。

