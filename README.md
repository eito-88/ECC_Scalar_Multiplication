ECC_Scalar_Multiplication on TI DSP TMS320C6678<br>
<br>
This file dscribes about:<br>
  1.what's the ECC Scalar Multiplication(ECCSM)<br>
  2.contribution of each files in this repository<br>
  <br>
  <br>
1.what's the ECC Scalar Multiplication(ECCSM)<br>
  ECCSM is one of the next-generation Pubulic-key Cryptograph.<br>
  ECCSM is used by ECElGamal, ECDH or ECDSA et al.<br>
  Normally, ECCSM is in affine coordination but in my program, in Jacobian coordination because of easiness of calculate.<br>
  <br>
2.contribution of each files in this repository<br>
  each files in this repository are divided in two parts.<br>
  one part has the main function which calls fast modular multiplication(MM) written by assembly. <br>
  and also, this part does basic ECCSM, modular addition and substraction.<br>  
  the other part is called by the main function. this file does fast MM only.<br>
<br>
<br>
---Japanese are bellow<br>
---以下日本語<br>
<br>
<br>
このファイルは：<br>
  1.ECCスカラー倍算<br>
  2.このレポジトリ内の各ファイル<br>
についての説明です。<br>
<br>
<br>
1.ECCスカラー倍算(ECCSM)<br>
  ECCSMは次世代公開鍵暗号の一つです。<br>
  ECCSMはElgamal暗号系、鍵共有、電子署名を行うことが可能です。<br>
  通常、ECCSMはアフィン座標で表記されますが、このプログラムは計算の容易性からヤコビ座標で行われます。<br>
  <br>
2.このレポジトリ内の各ファイル<br>
  このレポジトリ内のファイルは以下の２つに分類することができます。<br>
  ・メイン部分：アセンブリで実装されている高速剰余乗算のライブラリを呼び出します。<br>
  　　　　　　　　また、ECCSMの基本的な部分を行ったり、今回高速実装をしていない剰余加減算も行います。<br>
  ・サブ部分：メイン部分に呼ばれます。このファイルは高速剰余剰余のみを行います。<br>
<br>
