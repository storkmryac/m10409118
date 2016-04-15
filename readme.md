# 第一次作業

##### Data Sources 

---
從哪個API來的？
  > TwitterAPI

  內容主題為何？
  > 政治和科技
  
  下哪個查詢字串？
  > #Obama, #Alphago`

##### 收集到的 Data Format(JSON的欄位架構）
　
```
 * "contributors": 使用者物件的集合，象徵幫助Tweet的人，代表官方tweet創辦人
 * "truncated": tweet是否被裁切掉，超過140字會被切掉
 * "text": 文字內容
 * "is_quote_status": 是否被引用的狀態
 * "in_reply_to_status_id": 若這篇Tweet為回覆別人的Tweet才會顯示被回覆的Tweet的ID（以整數表示）
 * "id":這篇Tweet的ID（以整數表示），數字會大於53bit造成有些程式語言難以解譯 
 * "favorite_count": 這篇Tweet有多少個喜歡
 *  "entities": 
    * "symbols": 類似hashtag，但是以錢號($)表示
    * "user_mentions": 有無提到其他的Twitter使用者
    * "hashtags": 被解析出來的標籤
    * "urls": 包含在這篇Tweet裡面的網址
 *  "retweeted": 這篇Tweet是否有被其他Twitter使用者轉發
 *  "coordinates": 這篇Tweet的發文座標
 *  "source": 
 *  "in_reply_to_screen_name": 可為空值，若這篇Tweet為回覆別人的Tweet，會顯示原Tweet名稱
 *  "in_reply_to_user_id": 可為空值，若這篇Tweet為回覆別人的Tweet，會顯示原Tweet的使用者ID（以整數表示）
 *  "retweet_count": 這篇Tweet被轉發的次數
 *  "id_str": 這篇Tweet的ID
 *  "favorited": 這篇Tweet是否有被其他已驗證的使用者按喜歡
 *  "user": 
    * "follow_request_sent": 可為空值，是否有已驗證的使用者要求追蹤受到保護的使用者帳戶
    * "has_extended_profile": 有沒有擴展的profile
    * "profile_use_background_image": 使用者是否同意可以使用他們上傳的背景圖片
    * "default_profile_image": 使用者是否有上傳他們的照片，沒有的話則以預設的圖案代替
    * "id": 使用者的ID（以整數表示），數字會大於53bit造成有些程式語言難以解譯
    * "profile_background_image_url_https":使用者背景圖片的網址（基於HTTPS）
    * "verified": 使用者是否有通過驗證
    * "profile_text_color": 使用者使用的的字體顏色（十六進位）
    * "profile_image_url_https":使用者照片的網址（基於HTTPS）
    * "profile_sidebar_fill_color": 使用者使用的側邊欄位的背景顏色（十六進位）
    * "entities": Entity會提供metadata及額外關於這篇Tweet的相關資訊
       * "description": 
          * "urls": 這篇Tweet涵蓋的網址
    * "followers_count": 追蹤這個使用者帳號的人數
    * "profile_sidebar_border_color": 使用者使用的側邊欄位的邊框顏色（十六進位）
    * "id_str": 使用者（以字串表示）
    * "profile_background_color": 使用者使用的的背景顏色（十六進位）
    * "listed_count": 使用者擁有的list數量
    * "is_translation_enabled": 使用者是不是允許翻譯
    * "utc_offset": 與GMT標準時間的時差（以秒顯示）
    * "statuses_count": 使用者發出的Tweet數量
    * "description": 使用者自介
    * "friends_count": 使用者追蹤其他使用者的數量
    * "location": 使用者可自行定義的地區位置
    * "profile_link_color": 使用者使用的的連結顏色（十六進位）
    * "profile_image_url":使用者照片的網址（基於HTTP）
    * "following": 使用者是否有被其他已驗證的使用者追蹤
    * "geo_enabled": 使用者是否同意將地理位置顯示於照片上
    * "profile_background_image_url":使用者背景圖片的網址（基於HTTP）
    * "screen_name": 使用者自行定義的名稱，可以做更改
    * "lang": 使用者自行選擇顯示介面的語言，以BCP47編碼顯示
    * "profile_background_tile": 是否顯示使用者背景圖片的網址
    * "favourites_count": 使用者喜歡的Tweet數量
    * "name":使用者顯示的名稱，可以做更改
    * "notifications": 當該使用者發佈新的Tweet時，是否同意收到SMS的更新通知
    * "url": 使用者所提供的網址
    * "created_at": 使用者創辦帳號的時間
    * "contributors_enabled": 使用者是否有連結貢獻者模式
    * "time_zone": 使用者自行定義的時區位置
    * "protected": 使用者是否有選擇保護他們的Tweet
    * "default_profile": 使用者是否使用預設的照片
    * "is_translator": 使用者是否有參與幫助翻譯Twitter的工作
 *  "geo": 不贊同使用，現在都使用coordinates欄位紀錄
 *  "in_reply_to_user_id_str": 若這篇Tweet為回覆別人的Tweet，會顯示被回覆的Tweet的作者ID（以字串表示）
 *  "lang": 根據機器偵測自動判斷出該Tweet的語言
 *  "created_at": 使用者發出Tweet的時間
 *  "in_reply_to_status_id_str": 若這篇Tweet為回覆別人的Tweet，會顯示被回覆的Tweet的ID（以字串表示）
 *  "place": 該Tweet是否有與某地連結
 *  "metadata": 
    * "iso_language_code": 該網站使用的語系
    * "result_type": Tweet的型態為何，是熱門Tweet還是近期所發出的Tweet
```
