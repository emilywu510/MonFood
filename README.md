# MonFood
本專案為TibaMe Java養成班培訓期間團體專題

本專案主要為美食外送平台，與目前市面上外送平台不同在於具備交友聊天系統，會員彼此之間可交換美食訊息，以增加平台使用黏著度

# 主要負責功能

1. 配對系統：每日固定時間進行不重複對象配對，雙方接受配對後可成為好友。  
2. 好友列表：可查看好友詳細資訊。  
3. 聊天系統：好友可隨時互相進行即時聊天，聊天訊息亦會永久留存。  

# MySQL資料庫架構(部分)
<img width="551" alt="image" src="https://user-images.githubusercontent.com/93464862/186160284-645cec74-b65c-4989-8c76-e2ddf83c12ce.png">

# 使用技術
- Java、Servlet、JDBC
- 利用Quartz排程器實現每天午夜12:00的隨機配對
- 結合Bootstrap完成網頁版面設置
- 使用Javascript、JQuery實踐前端畫面
- 使用Redis存取聊天訊息
- 使用MySQL關聯式資料庫存取
- 使用websocket實踐聊天(訊息推送)
- 使用Ajax技術實踐前後端分離
- Git版本控制

# 功能介紹
**配對系統**  

<img width="481" alt="image (5)" src="https://user-images.githubusercontent.com/93464862/186165698-7d16fdba-caca-47d9-aa53-92115aa06066.png">

- 平台頁面右下角皆有一個橘色Icon，點擊即可看見當天配對名單
- 使用Quartz排程技術讓系統自動於每天午夜12:00進行會員隨機配對
- 每位使用者永遠不會被重複配對

**好友列表**

<img width="943" alt="image (1)" src="https://user-images.githubusercontent.com/93464862/186164084-0c770a13-9f3d-47bd-bffe-de3c9185bdd1.png"><img width="395" alt="image (2)" src="https://user-images.githubusercontent.com/93464862/186164189-799c4367-2617-4cf6-8af6-f76486e94749.png">

- 若雙方皆點擊接受配對即可成為好友，成為好友後可在好友列表中找到對方
- 好友列表可查看對方詳細資訊，如自我介紹、生日等訊息

**聊天室**

<img width="495" alt="image (3)" src="https://user-images.githubusercontent.com/93464862/186165110-1b867554-0f60-4d54-b997-1cae8512684f.png">

- 若雙方皆點擊接受配對即可成為好友並進行即時聊天
- 聊天室使用websocket技術並將歷史聊天紀錄存於Redis資料庫


