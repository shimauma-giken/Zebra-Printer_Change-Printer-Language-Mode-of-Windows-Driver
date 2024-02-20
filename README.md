## Windows ドライバのモード（ZPL、CPCL）を切り替える方法

-----
</br>

ゼブラモバイルプリンタ向けのドライバは下記の通りZPLとCPCLの２種類が存在します。どちらのドライバにおいてもほぼ同等の機能を実装しています。

Windows によって、どちらがCPCLモード自動選択されるかはプリンタ内部のpnp_optionモードによって決まります。任意のドライバ形式に切り替える場合は下記表の設定コマンドを実施ください。



<table border="2">
<tr>
<th>
</br>
ZPLモード向けドライバ
</br>
</br>
</th>
<th>
CPCLモード向けドライバ
</th>
</tr>
<tr>
<td>
<img src="image.png">
</td>
<td>
<img src="image-1.png">
</td>
</tr>
<tr>
<td>
</br>
設定コマンド：</br>
! U1 setvar "device.pnp_option" "zpl"</br>
</br>
確認コマンド：</br>
! U1 setvar "device.pnp_option"</br>

</td>
<td>
</br>
設定コマンド：</br>
! U1 setvar "device.pnp_option" "cpcl"</br>
</br>
確認コマンド：</br>
! U1 setvar "device.pnp_option"</br>
</td>
</tr>

</table>
