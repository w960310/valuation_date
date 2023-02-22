# 月結

所有excel檔案做好先放月結資料夾(1_reserve>準備金報表)，所有連結中關聯的檔案都要打開，才能串到已更新的值
做好就先匯出pdf放到PDF資料夾留存

月結開始前先行更新sql，月份、連結可以先改(要做假檔案吃link)
切記跑更新連結巨集時不要開其他檔案，避免連結檔案位置消失變動

3號:
確認有無新商品(?)，跑check_gta_upr，做GTA保費放大比率計算，將結果(打勾的GTA部分)貼到GTA_upr_11XXX後，寄給再保科逢恩


4號:(UPR慢點放公用槽，先給鎮遠看過，其他accuracy,rein_cd,低理賠,消失保單,GTA)

1.
跑02.upr資料夾裡的A0~C+Currency (等arkt,arco_a資料庫好才可以開始)，跑comp資料夾裡的01~08 > output_comp > upr_comp >
0.2upr夾裡的upr_all(產出UPR所需txt)，跑完告知柏安。

2.
做UPR_11XXX.xls(確認sql無誤，有無新商品，再保科回傳的gta再保資料(2欄)，acurracy，學保保費(進公用槽保費收入找))

3.
將UPR_11XXX的有效統計獨立出來放在UPR有效契約檢核夾，再寄給柏安。

4.1
消失保單合理性說明:arkt,arco_a好了就可以開始，upr報表交出前一定要做好，最好五號做好，最晚七號早上。
做好印"彙整"部分成PDF(8.)放進PDF資料夾留存

4.2
低理賠準備金:UPR"有效統計"完成就可以做了，跟再保資料無關，無須等accuracy資料來。

4.3
未滿期差異表syy(保費部分(柏安))好就先做，做完匯成PDF
原因2.明年學保沒保費進來時就不會有放大比例下降所致的問題
造冊與否拆分問題從11202始就不會有，因11102開始已拆分。

其他資料做好轉
PDF放PDF資料夾留存
PDF11XXX短年期準備金(含低理賠)約5號，放公用槽RPT內，印出紙本，連同再保給的紙本資料(夾在後面)夾在一起給棟哥(科主管)

5.UPR拆分各區(先dist_ibnr > 總表(rsv_acct) > dist_upr) 6號
(吃怡方的syy_11XXX_clm和柏安的syy_11XXX、短年期保費不足準備金(要確認是否為最終版本))
ibnr做好先連到acct傳acct給怡方對total數字
總表業主權益下12月要T，給柏安確認。12月業主權益兩頁底下都有一顆亭毓要給的數字。  
總表放進公用槽後馬上知會棟哥

6.棟哥>會計部

7.
TB表確認 (約8~11號):核對TB表:等OA跳照會通知，TB照會檔全貼近TBchecking，改連結，右邊check欄為(-意即0) 合併數TRUE 就OK。OA照會單回復:112/01未滿期保費準備金確認無誤，謝謝

8.
等TB表好，email資料夾裡的兩檔案給企畫部俊豪(upr餘額:新增月份連結，要確認有無新險、欄位調整，巨集貼死存檔，
uprtogo:改月份改月份改月份改月份改月份，新險新增，巨集貼死存檔，確認與upr一致)

9.
寄給致銓協理:短年期再保UPR餘額(UPR_11110."upr".(S94))

10.TB表好之後(月結結束)可直接接著做一季做一次工作事項(財報、決算報告書、獨董)

#資訊公開_1

【資訊公開 作業流程】

1. 「資訊公開」每一季都要做(「第1、2、3季」較少，「第4季」較多)，並上傳至兩個地方：
	(1) 觀測站 - '表2-5-2'(每季都要)、'表3-1-2~3-5-2'(第四季要)。
	(2) 公司官網 - '108-....pdf'
	
<NOTE> '第1、3季'：結束的45天內要公告；'第二季'：結束的2個月內要公告；'第四季'：結束的3個月內要公告。

2. '公司首頁(http://pmwbmgm1.mli.com.tw:7003/sites/mliportal/home)'底下「資訊公開」，有說要負責哪些：
	(1) 財務概況(每季都要)：「準備金(包括保險負債、具金融商品性質之保險契約準備及外匯價格變動準備)」依會計部照會單填就好了。
	(2) 業務概況(只第4季要)：「市場占有率」、「各險別...」*2、「人壽保險個人保件...」*4。
	
<NOTE> 明確規定可Google「人身保險業辦理資訊公開管理辦法」。

3. 資訊公開folder > Replicate之前的檔案。

4. 財務：copy照會單給「會計部」'樹良經理(2730)'，要等他們「財報」完成(由第一步的決算日期推算)，電話詢問日期填寫(e.g. 12、13號左右，最晚20、21號)。

<NOTE> 記得改「日期」、「季數」、「精算一部」，列印、簽名(承辦人)。

<NOTE> Q4照會單回復日期要等董事會通過(25號左右)，壓隔一天，記得3/31前要上傳。

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

5. '資本與準備金.xls'：「準備金」TAB > 「A7」要與上傳日期一致(預估Neil看一天，協理再看一天) > 「F13」欄位有「前3年」與「最新一季」(第四季特例，填前三年就好) > 依照「會計部照會單」填上「金額(佰萬元)」

<NOTE> 用上一季的資料，再用去年的格式檢查，之後另存成pdf。

<NOTE> 公司版的「準備金」都改0不要放「-」。


	!!!以下第4季!!!

	--上傳到公司網站
	(1) 財務概況－準備金：'會計部'照會單。
	(2) 業務概況－人壽保險個人保件有效契約平均保險金額：'柏安'提供。
	(3) 業務概況－人壽保險個人保件有效契約平均保險費：'俊和'提供。
	(4) 業務概況－人壽保險個人保件新契約平均保險金額：'柏安'提供。
	(5) 業務概況－人壽保險個人保件新契約平均保險費：'俊和'提供。
	(6) 業務概況－市場占有率：'柏安'提供，用「同業業績：保險專獎 (一年一次)」的資料。
	(7) 業務概況－各險別之保費收入及保險給付：'俊和'與'怡方'提供。
	(8) 業務概況－各險別準備金：'博棟'提供(需要會計照會單核對)。
	
	--上傳到公開資訊觀測站
	(1) 表2-5-2_各種準備金(102年)(壽險)：'會計部'照會單。
	(2) 表3-1-2_市場占有率(壽險)：'柏安'提供，用「同業業績：保險專獎 (一年一次)」的資料。
	(3) 表3-2-2_直接保險業務明細表(壽險)：'柏安'與'俊和'提供(可從年度檢查報表21-1複製)。
	(4) 表3-3-2_保險給付明細表(壽險)：'怡方'提供。
	(5) 表3-4-2_各險別準備金(壽險)：'博棟'提供(需要會計照會單核對)。
	(6) 表3-5-2_財務業務指標計算表(壽險)：'柏安'與'俊和'提供(「業務員定著率」將由'業務支援部-信介'提供)，可勾稽'年度檢查報表-壽險(非RBC相關)_表29'。

<NOTE> 整理好就先列印出來給填的人蓋章！

6「資訊公開申報表」- 「合計」內：
	(1) 新契約：新年度。	(2) 有效契約：續年度。	(3) 合計：小計。

<NOTE> 用去年check，再把格式拉到今年，要取到「小數點第四位」再*100 (報表要以「小數點第二位」呈現)。>

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
	
7. '觀測站'「表2-5-2」：「C3」申報年度 >「E3」申報季 >「年度最新一期金額」依照「會計部照會單」填上「金額(仟元)」(注意順序不一致)
	(1) 空欄要填「n/a」(「附註」先留空白)。
	(2) 確認「申報年度」、「季度」，不要更動格式。
	<NOTE> 用上一季的資料，再用去年的格式檢查。
	
	
	!!!以下第4季!!!
	
8. '觀測站'「表3-4-2」：
	(1) 「準備金」copy自'108年度資訊公開底稿'「Sheet1」(官網只要藍色部分；觀測站要藍跟白色的兩格)。
	<NOTE> '工作底稿 - Sheet2(2)'中的「註二」：「特別準備金」都是負債向下。

9. '觀測站'「表3-3-2」：
	(1) 「檢查報表」copy自'108年度資訊公開底稿'。

10. '觀測站'「表3-5-2」：
	(1) 「黃色部分」copy自'108年度資訊公開底稿'「Sheet3」，全部小數點都要去掉(四捨五入)，「I行」公式也要去掉。

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

11. 將更新的檔案都印出來，附上會計部的照會單，印出給'Neil'檢查簽名(「佐證資料」由資料提供者一併提供)。










12. 開啟 'Oracle WCS 後台' > 內容樹狀結構 > Article > 關於我們 > 資訊公開 > 業務/財務狀況 > 準備金(包括保險負債、具金融商品性質)。 

13. 點選「鉛筆」進行編輯 > 名稱(自己看的)　> 「更新日期」改上傳日期 > 內容 > 移除/上傳PDF > 儲存。

14. 描述資料：開始/結束日期(不再需要，留空)，但上架時間要跟「財報」同時或晚(不能早於)，需問「會計部」'樹良經理'。

15. 最上面一排：檢視 > 狀態 > 工作流程命令 > 選取工作流程(若是退件，要選「完成指派」) > MLI:精算部審核流程 > 採取動作：110Q2 準備金。(派發布任務前須先將紙本(兩張上傳後截圖印出來的和會計部回來的一疊照會單)拿給部門主管審核)

<NOTE> 不再留上一筆紀錄，直接覆蓋即可(不再需要下架、改日期)。

<NOTE> 若有錯誤，可以從「檢視」>「狀態」取消流程。

16. 檢查'測試官網'，下載「Files」核對。

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

17. 自己應該有卡跟「讀卡機」，開啟'保險業公開資訊觀測站( https://ins-info.ib.gov.tw/ )'(要用IE)。

18. 右上角：業者登入 > PIN碼：84445511 > 使用者代號：90510 > 使用者密碼：84445511 > 「保險業資訊公開申報」(右側)。

19. 申報 > '1.檔案上傳'(財務概況,Q4另加業務狀況) > 表單類型/名稱 > 上傳並加入檔案 > 上傳確認 > PIN碼：84445511 > 檔案簽章成功。(先確認表格是否有新版本)

<NOTE> 注意名稱不要有「yyyQx」。

20. '2.上傳狀態清單' > 查詢 > 待上傳結果顯示「上傳成功，檔案處理完成」。

<NOTE> 「備註」也要打「n/a」，小數點後不能超過4位。

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

21. 寄email請'協理'確認'測試官網'與'保險業公開資訊觀測站'。

<NOTE> 或給文件時提醒。

22. 要上傳當天(財報公告後)再請'協理'發布  --'3.待發布至網站清單' > 查詢 > 全選 > 發布 > '4.發布至網站結果清單' (或'2.上傳狀態清單')

23. 上兩個網站check有沒有發布。
	https://www.mli.com.tw/sites/mliportal/about/info-publication&selectInfo=1
	https://ins-info.ib.gov.tw/customer/life.aspx?UID=84443471

24. Q4要複印'業務支援部'的簽呈，整理檔案後歸檔。



【END】

#資訊公開_2

資訊公開:
	Q1、Q3財報最晚不能超過45天，Q2兩個月，Q4三個月。Q1:01/01~03/31，依此類推。
	
Q1~Q3流程:

1.先問王振峰72233財報哪時候出，再印照會單給他，押約限一周時間內回覆。(Q1:04/26照會 Q2:08/10照會 Q3:10/26照會 Q4:03/10照會)

2.111XXQ1~3資本與準備金檔案:改日期(和財報出同一天)，依照照會單上的金額填，注意百萬元、千元切忌依照會計部給的資料填。
  表2-5-2_各種準備金(102年)(壽險):調申請年度、季度。其他依照照會單上的金額填，注意百萬元、千元切忌依照會計部給的資料填。

Q4額外流程:

進資料夾110Q4-->公司官網資料，上傳裡面的8個表，8個表
和資訊公開觀測站資料夾裡面的全部檔案
分別交給以下人員填寫

保額相關:柏安
市占率、保費相關:亭毓
給付相關:怡方
各險別準備金:鎮遠
準備金:振峰
表3-5-2的定著率:業務支援部陳信价

3.上傳到公司官網、資訊公開觀測站(上傳前要提早印出來給科主管、部門主管審核)(表出來了就先給審核，不用等上傳的時候)






















