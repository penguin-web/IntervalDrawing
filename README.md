# Interval Drawing
"Interval drawing"は，絵を描く人が一度は経験する「30秒ドローイング」の汎用性を上げたものになります．一般に30秒ドローイングと言えば，人体の３Dモデルを様々なポーズ・様々な角度から見たものが表示され，30秒のうちにスケッチすることを繰り返すものであると思います．しかしこれでは裸の人体しか練習できません．
そんなときにこのプログラムを使えば，描きたいもの（例：服，動物，家など）を入力することで，Google Chromeからそれらの画像を検索して一定時間間隔にランダムに表示させることができます．

# 必要な手順
１．右にあるReleasesからInterval Drawingを開き，IntervalDrawing.exeをダウンロードする.  
２．好きな場所（Cドライブ>ユーザー>(ユーザー名)以下が望ましい）に展開する  
３．ChromeDriverをダウンロードする（Google Chromeのページの右上の縦3点→ヘルプ→Google Chromeについて　と移動すると，バージョンが確認できる．これを記録し，次に[公式ページ](https://chromedriver.chromium.org/downloads)から，先ほど記録したChromeのバージョンよりも古い中で最も新しいバージョンのChromeDriverをダウンロードする.windowsの場合はchromedriver_win32.zip）  
４．ZIPを解凍し，先ほど展開したフォルダの中に入れる．  
５．Excelファイルを新しく作成し，適当な名前を付ける．  
６．同じくフォルダの中に入れる．  
７．IntervalDrawing.exeをダブルクリックで実行する．（実行できずに即終了してしまう場合は，↑の手順のどこかが未達成である可能性が高い）（ショートカットを作成してデスクトップ上においておくと良い）  

# 実行後の手順
以下の４つのコマンドがある．  
順番としては，g→(a)→s  

g：検索した画像のURLをExcelファイルに保存するモード．まずこれをしないと画像は表示できない．  
　１．Input the Search Words. Separete with "・"  
    描きたいものを入力する．複数条件つけたい場合は「　」で区切る（例：デニム　レディース）．一度に複数種類のものを取得したい場合は「・」で区切る（例：デニム　レディース・Tシャツ　メンズ・鹿　公園）  
　２．Input each number of items  
    取得したい数を入力する．（現状技術が足りず50くらいが限界）  
　３．Are you OK? if so, press ENTER. If you'll redo the setup, input any other words  
    大丈夫ならEnterを押して取得開始．やり直したければそのほかの適当なキーを入力する．  

a：画像の表示位置を修正するモード．  
　１．Adjust the place of \"example\" for S_mode  
    カラのウインドウが表示される．これを画像を表示したい位置に移動させたら右上の×で消す．  

s：取得したURLから画像を一定時間間隔で表示するモード．実際に絵を練習する際にはこのコマンドを使う．  
　１．Input the Search Words  
    URLを取得したものは上に表示される．その中から選んで入力する．  
　２．Input the Number of Times  
    画像を表示する回数を入力する．  
　３．Input How Long the Interval is [min]  
    一枚の画像に対して何分表示するか入力する．0.5と入力すれば30秒になる．  
　４．Are you OK? if so, press ENTER. if you'll redo the setup, input any other words  
    大丈夫ならEnterを押して練習開始．やり直したければそのほかの適当なキーを入力する．  

f：ソフトを終了するコマンド．  
