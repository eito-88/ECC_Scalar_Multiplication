# ECC_Scalar_Multiplication on TI DSP TMS320C6678

This file dscribes about:
1. what's the ECC Scalar Multiplication(ECCSM)
1. contribution of each files in this repository

<br>

1. what's the ECC Scalar Multiplication(ECCSM)?
    - ECCSM is one of the next-generation Pubulic-key Cryptograph.
    - ECCSM is used by ECElGamal, ECDH or ECDSA et al.
    - Normally, ECCSM is in affine coordination but in my program, in Jacobian coordination because of easiness of calculate.
1. contribution of each files in this repository
    - `kbit_loop.asm`: this file can execute fast modular multiplication. it can execute on TMS320C6678 only.


### Ja

このREADMEファイルは：
1. ECCスカラー倍算
1. このリポジトリ内のファイル
についての説明です。

<br>

1. ECCスカラー倍算(ECCSM)
    - ECCSMは次世代公開鍵暗号の一つです。
    - ECCSMはElgamal暗号系、鍵共有、電子署名を行うことが可能です。
    - 通常、ECCSMはアフィン座標で表記されますが、このプログラムは計算の容易性からヤコビ座標で行われます。
1. このリポジトリ内のファイル
    - `kbit_loop.asm`：高速な剰余剰余をアセンブリで実装してあります
