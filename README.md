ECC_Scalar_Multiplication on TI DSP TMS320C6678

This file dscribes about:
  1.what's the ECC Scalar Multiplication(ECCSM)
  2.contribution of each files in this repository
  
  
1.what's the ECC Scalar Multiplication(ECCSM)
  ECCSM is one of the next-generation Pubulic-key Cryptograph.
  ECCSM is used by ECElGamal, ECDH or ECDSA et al.
  Normally, ECCSM is in affine coordination but in my program, in Jacobian coordination because of easiness of calculate.
  
2.contribution of each files in this repository
  each files in this repository are divided in two parts.
  > one part has the main function which calls fast modular multiplication(MM) written by assembly.
    and also, this part does basic ECCSM, modular addition and substraction.
  > the other part is called by the main function. this file does fast MM only.


---Japanese are bellow
---以下日本語


このファイルは：
  1.ECCスカラー倍算
  2.このレポジトリ内の各ファイル
についての説明です。


1.ECCスカラー倍算(ECCSM)
  ECCSMは次世代公開鍵暗号の一つです。
  ECCSMはElgamal暗号系、鍵共有、電子署名を行うことが可能です。
  通常、ECCSMはアフィン座標で表記されますが、このプログラムは計算の容易性からヤコビ座標で行われます。
  
2.このレポジトリ内の各ファイル
  このレポジトリ内のファイルは以下の２つに分類することができます。
  ・メイン部分：アセンブリで実装されている高速剰余乗算のライブラリを呼び出します。
  　　　　　　　　また、ECCSMの基本的な部分を行ったり、今回高速実装をしていない剰余加減算も行います。
  ・サブ部分：メイン部分に呼ばれます。このファイルは高速剰余剰余のみを行います。
