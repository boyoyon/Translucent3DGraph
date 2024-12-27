<html lang="ja">
    <head>
        <meta charset="utf-8" />
    </head>
    <body>
        <h1><center>Translucent 3D Graph</center></h1>
        <h2>なにものか？</h2>
        <p>
            半透明の3Dグラフを表示するプログラムです。<br>
            <img src="images/Translucent3DGraph.gif">
        </p>
        <h2>環境構築方法</h2>
        <p>
            pip install opencv-python PyOpenGL glfw<br>
        </p>
        <h2>使い方</h2>
        <p>
            python translucent3dgrpah.py<br>
            <br>
            defineSurface 関数で y＝f(x,y) を指定します。<br>
            <table border="1">
                <tr><th>操作</th><th>機能</th></tr>
                <tr><td>左ボタン押下＋ドラッグ</td><td>3Dモデルの回転(yaw,pitch)</td></tr>
                <tr><td>矢印キー押下</td><td>(同上)</td></tr>
                <tr><td>rキー押下＋ホイール回転</td><td>3Dモデルの回転(roll)</td></tr>
                <tr><td>右ボタン押下＋ドラッグ</td><td>3Dモデルの移動</td></tr>
                <tr><td>ホイール回転</td><td>3Dモデルの拡大・縮小</td></tr>
                <tr><td>Yキー押下</td><td>y方向の倍率を上げる</td></tr>
                <tr><td>yキー押下</td><td>y方向の倍率を下げる</td></tr>
                <tr><td>－キー押下</td><td>y方向の倍率を－1倍する</td></tr>
                <tr><td>ホイールボタン押下</td><td>慣性モードのトグル(on⇔off)</td></tr>
                <tr><td>iキー押下</td><td>(同上)</td></tr>
                <tr><td>sキー押下</td><td>スクリーンショット保存</td></tr>
                <tr><td>ウィンドウ閉じるボタン押下　</td><td>プログラム終了</td></tr>
            </table>
        </p>
    </body>
</html>
