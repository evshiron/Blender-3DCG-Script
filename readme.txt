Blender 3DCG script

■概要
これはオープンソースの3Dソフトウェアである Blender から3Dカスタム少女の
3Dモデルファイル(.tso)の入出力、ポーズ・モーションファイル(.tmo)の入出力を
行う Python スクリプトです。


■ファイル構成

	Python\3dcg_tso_import.py      tsoファイルインポート用Pythonスクリプト
	Python\3dcg_tso_export.py      tsoファイルエクスポート用Pythonスクリプト
	Python\3dcg_tmo_import.py      tsoファイルインポート用Pythonスクリプト
	Python\3dcg_tmo_export.py      tsoファイルエクスポート用Pythonスクリプト
	Python\3dcg_armaturemimic.py   Armatureを真似させるPython用スクリプト
	Python\3dcg_weightmirror.py    3DCG用のウェイトミラーPythonスクリプト
	Python\tdcg_change_mirror_bone_name.py	左右対称のウェイト編集補助スクリプト
	
	readme.txt                     このファイル
	readme.html                    簡単なチュートリアル
	html(フォルダ)                 readme.html のデータ類
	
	Sample.blend                   モーション+リギングのサンプル


■導入方法

Blenderのスクリプトフォルダに拡張子 .py のファイルをコピーして下さい。
例    C:\Program Files\Blender Foundation\Blender\.blender\scripts   等...


■簡単な使い方

・tsoファイルのインポート
Blenderのメニューバーから File → Import → 3DCG tso file (.tso)... 
と選択すると設定を入力する為のGUIが表示されるので、取り込むデータの種類を選択、
tsoファイルの場所を選び一番下のImportボタンをクリックすると取り込まれます。

・tsoファイルのエクスポート
Blenderのメニューバーから File → Export → 3DCG tso file (.tso)... 
と選択すると設定を入力する為のGUIが表示されるので、全ての設定を終えてから
右下のExportボタンをクリック、出力先を設定しもう一度Exportボタンをクリック
すればtsoファイルを出力できます。

・tmoファイルのインポート
Blenderのメニューバーから File → Import → 3DCG tmo file (.tmo)... 
と選択すると設定を入力する為のGUIが表示されるので、「TMO file select」から
参照TMOファイルを選び「TMO Load」を押すとボタンが追加で表示されるので、
フレーム番号を選びポーズを適用するArmatureを選択してから「Pose Apply」
を押すとポーズが適用されます。

・tmoファイルのエクスポート
Blenderのメニューバーから File → Export → 3DCG tmo file (.tmo)... 
と選択すると設定を入力する為のGUIが表示されるので、Armatureオブジェクトを選択し
出力先、ノードの参考先を選んだ後、Exportボタンをクリックすればtmoファイルを
出力できます。

・Armature Mimic
二つのArmatureを選択し起動させると、最後に選択したArmatureを最初に選択した
Armatureの動きを真似させる。

・3DCG用 ウェイトミラー
メッシュオブジェクトを選択し起動すると設定画面が表示されるので、
どちらからどちらに頂点グループをコピーさせるか、しきい値、
左右対称ボーンと中央ボーンの頂点グループをそれぞれ変更するかどうかを設定し、OKを押す。

・左右対称のウェイト編集補助スクリプト
オブジェクトモードからスクリプトを起動できます。(3DCG Change mirror bone name)
メッシュオブジェクトかアーマチュアオブジェクトを選択(複数選択可)し、
変換モードを選択すれば変換できているはずです。
具体的には、例えば「shiri_Right01」と「shiri_Left01」が「shiri_01.R」と「shiri_01.L」に
変換されて、Blender上で左右対称のボーン(ウェイト)と認識されるので、鏡面編集が簡単になります。
現在カス子のノードのみの対応です。

■注意事項
Blender 2.49b、Python2.6で動作確認しています。


■変更履歴

0.1 初版
0.2 3dcg_tso_import メッシュ読み込み部分のUV・法線のバグ、レジストリファイルから情報を読み取れないバグを修正
0.21 tdcg_change_mirror_bone_name.pyを追加
