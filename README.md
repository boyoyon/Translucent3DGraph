<html lang="ja">
    <head>
        <meta charset="utf-8" />
    </head>
    <body>
        <h1><center>Translucent 3D Graph</center></h1>
        <h2>なにものか？</h2>
        <p>
            半透明の3Dグラフを表示するプログラムです。<br />
            <img src="images/Translucent3DGraph.gif">
        </p>
        <h2>環境構築方法</h2>
        <p>
            pip install opencv-python PyOpenGL glfw<br />
        </p>
        <h2>使い方</h2>
        <p>
            python 3dgrpah.py<br>
            "equation.txt" で指定されたf(x,z)の3Dグラフを表示します<br>
            <br>
            python 3dgrpah.py (equation text file)<br>
            引数で指定したテキストファイル内で指定された f(x,z)の3Dグラフを表示します<br />
        </p>
            <table border="1">
                <tr><th>操作</th><th>機能</th></tr>
                <tr><td>左ボタン押下＋ドラッグ</td><td>3Dモデルの回転(yaw,pitch)</td></tr>
                <tr><td>矢印キー押下</td><td>(同上)</td></tr>
                <tr><td>rキー押下＋ホイール回転</td><td>3Dモデルの回転(roll)</td></tr>
                <tr><td>右ボタン押下＋ドラッグ</td><td>3Dモデルの移動</td></tr>
                <tr><td>ホイール回転</td><td>3Dモデルの拡大・縮小</td></tr>
                <tr><td>Xキー押下</td><td>x 方向の範囲を広げる</td></tr>
                <tr><td>xキー押下</td><td>x 方向の範囲を狭める</td></tr>
                <tr><td>Zキー押下</td><td>z 方向の範囲を広げる</td></tr>
                <tr><td>zキー押下</td><td>z 方向の範囲を狭める</td></tr>
                <tr><td>Yキー押下</td><td>y 方向の倍率を上げる</td></tr>
                <tr><td>yキー押下</td><td>y 方向の倍率を下げる</td></tr>
                <tr><td>－キー押下</td><td>y 方向の倍率を－1倍する</td></tr>
                <tr><td>ホイールボタン押下</td><td>慣性モードのトグル(on⇔off)</td></tr>
                <tr><td>iキー押下</td><td>(同上)</td></tr>
                <tr><td>sキー押下</td><td>スクリーンショット保存</td></tr>
                <tr><td>ウィンドウ閉じるボタン押下　</td><td>プログラム終了</td></tr>
            </table>
        <p>
                おまけ：座標軸ラベルのみ表示すると･･･<br />
                python axis-label.py<br />
                <img src="images/axis-label.gif">
        </p>
        <h2>使用例</h2>
        <h3>直交するV字谷(1)</h3>
        <p>
            <img src="images/example1.gif"><br />
            1点で偏微分可能でも全微分可能にならない例。<br />
            x軸、z軸上ではy=0 → (x,z)=(0,0) では ∂y/∂x=0, ∂y/∂z=0<br />
            しかし、軸以外の方向には微分不可。
        </p>
        <h3>直交するV字谷(2)</h3>
        <p>
            <img src="images/example2.gif"><br />
            1点で偏微分可能でも全微分可能にならない例。<br />
            x軸、z軸上ではy=0 → (x,z)=(0,0) では ∂y/∂x=0, ∂y/∂z=0<br />
            しかし、軸以外の方向には微分不可。
        </p>
        <h3>y=x<sup>2</sup>+1の定義域、値域を複素数に拡張した場合の関数値の実数部</h3>
        <p>
            <img src="images/example3.gif"><br />
            x軸上では下に凸。常に0より大きい。<br />
            z軸上では上に凸。2点で0になる。<br />
        </p>
        <h3>y=x<sup>2</sup>+1の定義域、値域を複素数に拡張した場合の関数値の虚数部</h3>
        <p>
            <img src="images/example4.gif"><br />
            x軸上、z軸上で0になる。<br />
        </p>
    </body>
</html>
