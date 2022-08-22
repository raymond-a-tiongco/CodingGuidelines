#  MySQL5.5系、5.6系のデータベース規約

## 概要

MySQL5.5、5.6に対するデータベース規約をここに記します。

## カラム定義

* update_date

    |  項目  |  値  |
    | ---- | ---- |
    |  Type  |  timestamp  |
    |  Null  |  NO  |
    |  Default  |  CURRENT_TIMESTAMP  |
    |  Extra  |  on update CURRENT_TIMESTAMP  |

    * 注意事項
        * MySQL5.6.5より前のバージョンでは、`on update CURRENT_TIMESTAMP`を複数カラムに設定することはできません。
        * MySQL5.7より前のバージョンでは、datetime型に`on update CURRENT_TIMESTAMP`を設定することはできません。
