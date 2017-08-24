## D & D Magazine

1. 每一期準備時新增一個 issue，issue 的 title 就是 Medium 的 title
2. 開始撰寫內容，任何的 code block 會被上傳至 gist 並且塞入 medium 當中。
3. 撰寫完畢後，由當週的負責人檢查，確認無誤後關閉 issue
4. 關閉 issue 會觸發 webhook => API gateway => lamda function，並上傳到 medium 上面
5. Medium 上會以 `draft` 顯示，負責人確認頁面無誤後，就可以直接發佈


### 其他想法

- 因為目前只要關閉 issue 就會觸發 lamda，所以有其他討論可以先暫時到[https://github.com/DnD-mag/DnD-lamda](https://github.com/DnD-mag/DnD-lamda)
- 是否要串 mailchimp 或其他服務？還是 medium 就好
