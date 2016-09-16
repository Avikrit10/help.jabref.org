---
title: リモート操作
---

# リモート操作

本機能は、**設定→詳細設定**で入切したり設定したりすることができます。

*Windows XP SP2(恐らく他のシステムでも)で本機能を有効にすると、このプログラムの機能のうち、Windowsファイアウォールによってブロックされる機能があるかもしれないというメッセージボックスが表示されることがあるかもしれません。この場合、ファイアウォールにブロックを続けさせるように返答して構いません。ファイアウォールは、JabRefのリモート操作と干渉しません。*

リモート操作の待ち受けを有効にすると、JabRefは、起動時に特定のポートでの待ち受けを開始するように試みます。つまり、他のアプリケーションが、このポートを通じてJabRefに情報を送ることができるようになります。JabRefは、外部からの干渉リスクを回避するため、ローカル接続のみを許可します。

このポートにバインドすると、2つめのJabRefインスタンスが、最初のインスタンスが実行中であることを発見できるようになります。この場合、明示的にスタンド・アローン・モードで実行するように指示しない限り、2つめのJabRefインスタンスは、最初のJabRefインスタンスに、コマンドラインオプションをこのポートを通じて渡した後、直ちに終了します。

最初のJabRefインスタンスは、このコマンドラインオプションを読み、ファイルを開いたり読み込んだり等、指定された動作を実行します。ファイルが、コマンドラインオプション`--importToOpen`を使って読み込まれる場合、読み込まれた項目は、現在表示されているデータベースに追加されます。データベースが開かれていない場合には、新規に作成します。