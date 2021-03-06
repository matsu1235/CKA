※古くなっているかもしれないので、正確にはhandbookや公式を参照

### 1. 対象の試験
***
* CKA-JP
* 3時間
* 問題文と試験官は日本語
* ubuntu
* kubernetes version 1.15

### 2. 必要なもの
***
* 試験会場
	* 静かでプライベートで明るい
	* 明るい照明や窓が、受験者の後ろに無い
	* コーヒーショップとか店の公共の場はダメ
	* 受験者以外は、試験会場に居たらダメ
	* 机にはノートや電子機器類はあったらダメ
* パスポート
* マイク、ウェブカメラ、インターネット、Chromeブラウザ
* 8080/tcp、4505/tcp、4506/tcp要オープン

### 3. 事前にやること
***
* 試験環境チェックを行う [URL](https://www.examslocal.com/ScheduleExam/Home/CompatibilityCheck)
	* ローカルOS推奨
	* URLのOption3から LinuxFoundation, CKA-JPを選択
	* Install Extension
	* Run Compatibility Check
	* チェック内容は全て読んで対応しておく（BrowerSettingsはなぜかチェックつかない）
* ImportantTipsやハンドブック、FAQを確認する
	* [Important-Tips](file/Important-Tips-CKA-CKAD-Master-8.5.19.pdf)
	* [FAQ](file/CKA-CKAD-FAQ-8.5.19.pdf)
	* [Handbook](file/CKA-CKAD-Candidate-Handbook-8.5.19.pdf)
* 会議室を確保する
	* 下記などの開始時間が選べる。空いているかどうかは試験環境チェックツールから確認可能
	* am 9:00, 10:00, 11:00
	* pm 15:00, 16:00
	* 会議室に取り外せない電子機器等がある等、不安な場合は事前確認を [問い合わせ先](mailto:customersupport@rt.linuxfoundation.org)
* CKA申し込む
	* 名前類はすべてパスポート表記と合わせること
	* LinuxFoundationIDを取る
	* CKAをorderする
* Tips
	* 青山本4-13,19章
	* Udemyのmock testをやる（当日の試験ライクな問題なので、慣れておく)
	* k8s the hard way
	* v1.15のk8s.ioにどこに何が書いてあるか把握しておく、必要ならブックマークを作成しておく
	* bash completionやaliasコマンドを用意する

### 4. 当日
***
* チェックインプロセスまで
	* 試験開始30分前ぐらいにカメラ、マイク、PCなどをセッティングしておく
	* 試験開始時間になったらChromeブラウザ開いてMyPortalから"Take Exam"ボタンが押せるようになるので、押す
	* CKA-JPを選んで"Launch Exam"を押す
	* 新しいタブにExam Consoleが出る。そのタブ以外は消してもOK
* その後、試験官にてチェックインプロセスが行われるので、指示に従う
	* 画面共有、カメラ、マイク
	* パスポートと試験予約名前の突合せチェック。ウェブカメラで見せる
	* Exam Rules、CNCF規約等を読んで同意する
* チェックインプロセス後はさらに下記についてチェックが行われる
	* 受験者のPC
	* 受験者周辺の環境（ウェブカメラで周囲を映す）
* 全てのチェックが終わったら試験がリリースされ、試験コンテンツの確認やコンソール操作が出来るようになる
	* ※ここから3時間のタイマーがスタートする
* Exam Consoleについて
	* 下記の3つで構成される
	* Exam Console functions(menu bar)
		* 画面、ウェブカメラのOn/Off
		* 試験官とのチャット開始ボタン : 質問があるときはこれ
		* テストルール内容 : 試験中は何回見てもOK
		* 試験ポーズボタン : 試験官に休憩を申し入れたいときに押す許可を得てから退席（タイマーは止まらない）
		* 試験終了ボタン : 解ききったら押す
		* Exam Consoleの更新ボタン : Latency issueがあったときにこれ押すといいかもとのこと
		* Notepad
	* Content Panel(left)
		* 試験内容
		* 残り時間タイマー
		* 言語は英語や日本語に変更可能。意味取りづらい場合は英語にしてもよいかも。ContentPanel以外は全て英語固定
	* Linux Server Terminal(right)
* Exam Consoleが起動しなかったり何か問題があった場合、"試験開始予定時間から15分以内"に下記のいずれかを必ず行う
	* (チャットサポート)Online - Click hear to get help
	* (電話)Support menu item in the top nav bar
	* これを行わないと試験が無効になる

### 5. 注意事項やTips
***
* Exam Console Tips
	* VMの再起動はいつでも可能
	* certerminalプロセスは停止したらダメ絶対
	* ctrl+c/vは動作しない。あと大量の文字列もコピーできない。
	* linux : テキストを選択=コピー、マウス中央ボタン=ペースト
	* Windows : Ctrl+Insert=コピー、Shift+Insert=ペースト
	* Exam Consoleはひとつだけ、文字サイズ変更はCtrl+/-
	* 6つのクラスターがあり異なるコンテナがある
	* それぞれの設問始めるときに、対象のクラスタを扱っているか確認してね
* 注意事項
	* 試験中は、試験官以外とコミュニケーションしたらダメ
	* 試験内容をうるさく読み上げたらダメ
	* 許可無く、ウェブカメラやデスクから離れたらダメ
	*　飲食禁止、ガムも（ラベルはずした透明な飲み物であればOK)
	* 耳とか顔、体に電子機器を付けるのはダメ
	* PCから必要以上に目を背けたらダメ
	* うるさい音や繰り返しノイズ（貧乏ゆすり的な）は控える
	* 口や顔を手で覆うのは控える
	* 紙や電子機器で文字を読んだり、メモするのはダメ（Exam ConsoleのNotepadのみでメモ可）
	* 試験官に従わなかったら試験中止
* ツールやリソースの扱いについて
	* 画面共有に映らない形でツールなどを使うのはダメ
	* manとか/usr/share配下のdocはOK
	* 外部URLは、下記とサブドメイン以下のみ閲覧可能
		* https://kubernetes.io/docs/
		* https://github.com/kubernetes/
		* https://kubernetes.io/blog/
		* 上記に外部サイト含まれている場合があるけどそれはクリックしたらダメ
	* 下記は全てダメ
		* PC以外の機器、ノートやドキュメント
		* WindowsのNotepad
		* ミランティスとかのコースマニュアル
		* スマートウォッチ・グラス、スマホなど
		* 誰かがCKAの試験内容を暴露した内容
* 警告なしに試験終了
	* 試験官に従わなかった場合
	* ソフトウェアや外部デバイス、手動などによる、試験内容のコピー
	* 試験官が許可した以上の時間、ウェブカメラから外れてしまった場合
	* 誰かが試験を手助けしていることが見つかった場合
	* 受験者の所作と、画面共有の見え方に、不一致が見られた場合
* 禁止行為
	* 試験内容の、Web/チャットルーム/ディスカッショングループへの公開禁止
	* CNCFが許可した人以外への、あらゆる試験内容の伝達行為
	* ハッカー的な行為
	* などなど

### 6. 試験後
***
* 36時間以内にメールで合否が分かる
* free retakeは12ヶ月以内に行う

### Appendix
***
* コマンド  
	* man If_exam
	* sudo -i
	* alias k=kubectl
	* source <(kubectl completion bash) # completion will save a lot of time and avoid typo
	* source <(kubectl completion bash | sed 's/kubectl/k/g' ) # so completion works with the alias "k"
* etcdバックアップ
	* ETCDCTL_API=3 etcdctl --endpoints https://[127.0.0.1]:2379 --cacert /etc/kubernetes/pki/etcd/ca.crt --cert /etc/kubernetes/pki/etcd/healthcheck-client.crt --key=/etc/kubernetes/pki/etcd/healthcheck-client.key snapshot save /tmp/etcd-backup.db
* リンク
	* CKA-JP申込サイト
		* https://training.linuxfoundation.org/certified-kubernetes-administrator-cka-jp/
	* ポータル
		* https://training.cncf.io/portal
	* お役立ち
		* https://kubernetes.io/docs/tasks/
		* https://kubernetes.io/docs/reference/kubectl/conventions/#generators
