# Windows Anaconda Python3 遇到 ImportError : No module named 'XXX.pyd' 問題

### 當遇到此次問題的環境及當前狀況

1. 使用Windows環境
2. 個人使用Anaconda python 3.6 來進行開發
3. 使用`pip setup.py install` 來安裝軟體包

4. 出問題的檔案是.pyd檔案

問題原因:

很明顯的在軟體包已安裝，且確認有裝好的狀況下，這種錯誤其實不應該出現，而這個錯誤發生的幾個關鍵點就是**Anaconda**及**pyd檔**，這是Windows的Anaconda出現錯誤所導致的，簡單來說就是在安裝時pyd\(Python3.dll\)這類的檔案沒有辦法正確安裝到檔案中，因此安裝好的軟體包裡面並沒有該檔案，導致無法Import。

解決方式：

以手動的方式將pyd檔案複製到原本軟體包的位置。

