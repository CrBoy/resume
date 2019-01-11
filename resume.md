# 畢玉泉（CrBoy）
#Web #後端 #Ruby-on-Rails #JavaScript #DevOps #AWS #網管 #Linux

聯絡方式：crazyscorpio@gmail.com

## 經歷
* Sharelike 技術長 _2014 - 2018_
後端開發（CodeIgniter、Laravel、Rails）、網頁前端開發（AngularJS、Vue.js）、主機系統與雲端服務管理（VMWare ESXi、Linode、AWS、G Suite）、網路與設備管理
* COSCUP 開源人年會 總召 _2015 - 2017_
* 國立成功大學計算機中心 網頁工程師 _2013 - 2014_
開發網頁專案（PHP + 變形的 CodeIgniter）
* 國立成功大學計算機中心 網頁工程師 _2012 - 2012_
協助選課系統、導入 Git、技術分享

## 學歷
* 國立成功大學資訊工程研究所 碩士 _2009 - 2012_
* 國立成功大學資訊工程學系 學士 _2005 - 2009_

## 技術相關經驗
### 程式開發
* 曾接觸數種程式語言，如 PHP（5.x）、Python（3.x）、Ruby（2.2~）、JavaScript（ES5 ~ ES6）。
* 為 Sharelike 運行最久的產品後端部份貢獻了超過 90% 的程式碼，使用 Ruby on Rails + MySQL + Redis。
* 以 AngularJS + Bootstrap 3 製作內部管理介面，供客服工程師使用。
* 使用 Node.js 製作小工具。使用較頻繁的有：
	* 將 AWS CloudWatch Alarm 轉發到 Slack 的小工具。
	* 作為 SMS gateway 的內部服務，可將 staging 環境欲送出的簡訊，改送到 Slack 與 Telegram，以節省不必要的簡訊費用。
* 使用 Bash script、Python 或 Ruby 撰寫自用的輔助小工具，如自動更新網站內容、門票釋出時發 Telegram 訊息通知，或是搶購限量商品。也有使用 Node.js 改寫的版本，利用其 event-driven 的特性，同時發出大量 request，對於時間敏感的操作很有助益。
* 2014 年使用 Python 參加 Google Code Jam，進入 top 3000，但止步於 top 500 外。
* 創造 [NCKU CSIE Wiki](http://wiki.csie.ncku.edu.tw/)。運用 Gitit wiki 系統的 template 機制，配合 jQuery 與 Bootstrap，在不修改 server-side 的前提下將其改頭換面。
### 基礎架構維運
* 使用 GitLab 建置自動化測試、部署機制，應用於前端（基於 Vue.js 與 Webpack）與後端（基於 Rails 或 Sinatra）專案。亦有管理性質專案利用 CI 環境簡化工作。
* 維運 AWS 服務
	* 為 Sharelike 唯一的 AWS 管理員。
	* 除常見的 EC2、RDS、S3、CloudFront 外，也利用 ELB 做 load balance，提升 API throughput，同時避免 downtime。
	* 架設 ECS cluster（然而多數時候機器數量為一台）用以運行內部所需服務（如 GitLab），以及後期新開發的產品，其 staging 與 production 都運行於此。
	* 利用 SES 做為公司服務之 SMTP service。
	* 應用 API Gateway + Lambda 建立輕量級服務，以零成本運行輔助性的小工具。
	* 絕大多數的服務都儘可能上 SSL，憑證部份直接使用 AWS 簽發的免費憑證。因為使用的服務都在 AWS，設定起來很方便。少數服務因特殊原因，則使用 Let's Encrypt 簽發的憑證。
	* 為減少佈建基礎架構時的人工介入，達成 infrastructure as code，除早期已經運作的服務外，都儘可能使用 CloudFormation 進行佈建。另為了精確掌握每個資源，所有 CloudFormation 使用的 template 都是自行根據需求撰寫，不使用 CloudFormer 產生。
* Sharelike 網管，獨自佈設網路基礎建設與管理網通設備。自辦公室搬遷起，進行基礎佈線、設置有線與無線網路，以 VLAN 切割內網與聯外網路。並建置公司自有 VoIP 總機（IP-PBX），話務量雖不大，卻是很有趣的嘗試。後來更讓分機跨區域運作，運作良好。
* 2018 年擔任 COSCUP 資訊組長，負責協調網站開發事宜、開發網站。並與夥伴共同建立 COSCUP 網站自動建置、部署機制，使用 GitHub Pages + TravisCI。
### 技術分享
* 2012 年間，以「那些老師沒教的事 - Code Smart, Don't Code Hard」為主題，在不同地方演講，講授 Git 版本控制，以及 gcc、make 與 gdb 等 toolchain 的使用。
* 進行團隊內部分享，主題包含 Git、Git flow、design pattern (Java)、CA 憑證系統運作原理、AWS...等。
* 由於做的東西常跟 web 有關，2015 年的時候寫了這樣一篇整理：[HTTP 通訊簡介](http://blog.crboy.net/2015/08/http.html)。
### 綜合/其他
* 使用 tcpdump、Wireshark 與 BurpSuite 進行網路封包分析。用以分析傳輸未加密或沒有進行 certificate pinning 的手機 app，瞭解其資料傳輸。或分析 SIP 的傳輸資料，在網路層做 debugging。
* 與友人共同發現並[回報](https://zeroday.hitcon.org/vulnerability/ZD-2017-01260) 17 直播 app 中能造成重大業務損失的漏洞。
* 與友人共同發現 KTV 系統漏洞，並在[回報](https://zeroday.hitcon.org/vulnerability/ZD-2016-00074)後於 HITCON lightning talk 發表。
* 熟悉命令列操作，具備中英文盲打能力。
