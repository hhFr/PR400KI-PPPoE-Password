# PR400KI-PPPoE-Password

PR-400KI

http://192.168.1.1/cgi-bin/paractl.cgi?st_ppp1.html

URL:
view-source:http://192.168.1.1/cgi-bin/paractl.cgi?st_ppp1.html

`〜`

`<INPUT TYPE="hidden" NAME="CGI_DATA_CHANGE" VALUE="">`

`<INPUT TYPE="hidden" NAME="CGI_DATASET_MOD" VALUE="">`

`<INPUT TYPE="hidden" NAME="PPPOE_NAME_1" VALUE="株式会社ＸＸＸＸ">`

`<INPUT TYPE="hidden" NAME="PPPOE_USER_1" VALUE="xxxxxxxx@one.ocn.ne.jp">`

`<INPUT TYPE="hidden" NAME="PPPOE_PASS_1" VALUE="50617373777264495331323334">`

`<INPUT TYPE="hidden" NAME="PPPOE_SPECIFIC_1" VALUE="0">`

`〜`

"PPPOE_PASS_1"
VALUE=
"50617373777264495331323334"


`50 61 73 73 77 72 64 49 53 31 32 33 34	← ASCII 文字コード`

`P  a  s  s  w  r  d  I  S  1  2  3  4	← ASCII 文字に変換`

`PasswrdIS1234	← パスワード`


# 簡単に得る方法

macOS/Linux (要 xxd コマンド)

$ echo "50617373777264495331323334" | xxd -r -p ; echo

PasswrdIS1234

 xxd は
 
 macOS では標準で入っている。
 
 Linux では vim に含まれているので
 
 yum install vim
 
 すればよい

ファイルのパッケージ確認

$ rpm -qf /usr/bin/xxd

vim-common-7.4.629-5.el6_10.2.x86_64
