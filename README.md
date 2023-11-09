# plusコマンド
[![test](https://github.com/Yusp27/robosys2023/actions/workflows/test.yml/badge.svg)](https://github.com/Yusp27/robosys2023/actions/workflows/test.yml)

標準出力から読み込んだ数字を足す。

## 必要なソフトウェア
* Python
  * テスト済み: 3.7～3.10

## テスト環境
* Ubuntu

'''bash

$#!/usr/bin/python3
# SPDX-FileCopyrightText: 2023 Yuta Ogura
# SPDX-License-Identifier: BSD-3-Clause
import sys

ans = 0
for line in sys.stdin:
    try:
        ans += int(line)
    except:
        ans += float(line)

print(ans)

'''

* このソフトウェアパッケージは、３条項BSDライセンスの下、再頒布および使用が許可されます。
* このパッケージのコードは、下記のスライド (CC-BY-SA 4.0 by Ryuichi Ueda) のものを、本人の許可を得て自身の著作としたものです。
    * [ryuichiueda/my_slides robosys_2023](https://github.com/ryuichueda/my_slides/tree/master/robosys_2023)

* © 2023 Yuta Ogura
