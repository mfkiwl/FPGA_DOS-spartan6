Build a DOS machine with FPGA.


Move "[next186](https://opencores.org/projects/next186_soc_pc)" on the board cut by CNC.
<br> Even if the software is existing and reliable, there is no guarantee that the hardware will work, so take the following steps.
<br> Step-1 Connect memory, IO, etc. to a commercially available FPGA (xc6lx9) board, move it with CP / M, and check the hardware operation.
<br> * Even with CP / M, the main memory is not static but DRAM.
<br> However, since burst access is not performed, defect verification is easy.
<br> Step-2 Operate as a DOS system on the above hardware.
<br> * Actually, the memory (DRAM) did not work properly, and I stepped on here for several months. How it works.
<br> Step-3 Create a printed circuit board with CNC, first verify the operation of the hardware with CP / M, and then operate the DOS system.
<br>
<br> Describe the hardware / software to be used for reference.
<br> [lx9-Step-1-io] Expansion platform used in Steps 1 and 2. It is operated by piercing a commercially available board (XC6SLX9 Mini Board).
<br> [MAIN-BOARD] Motherboard with FPGA and DRAM.
<br> [PMOD-IO] A board that connects the SD card and keyboard. Stick in MAIN-BOARD.
<br> [PMOD-VGA6] VGA display output. Stick in MAIN-BOARD.
<br> [lx9-Step1-CPM80] Circuit for operating CP / M (verilog)
<br> [lx9-Next186_SoC] Circuit for operating DOS (verilog)
<br>「[SD2G_Dos_F.zip] free MS-DOS SD-image

<br> For details, see "[Qiita](https://qiita.com/hi631/items/e8e0db06a52938b57632)".


<br>DOSマシンをFPGAで作る。

<br>　「[next186](https://opencores.org/projects/next186_soc_pc)」をCNCで切削した基板上で動かす。
<br>　ソフトが既存で信頼できても、ハードが動作する保証は無いので、次のようなステップを踏む。
<br>　Step-1　市販FPGA(xc6lx9)基板にメモリ、IO等を繋ぎ、CP/Mで動かしハード動作を確認。
<br>　　　　　※CP/Mでも、メインメモリはスタティックでは無くDRAMで構成する。
<br>　　　　　　但し、バーストアクセスは行わないので、不具合検証はやり易い。
<br>　Step-2　上記ハード上で、DOSシステムとして動作させる。
<br>　　　　　※実際の所、メモリ(DRAM)が正常に動作せず、ここで数か月足踏みした。しくしく。
<br>　Step-3　CNCでプリント基板を作成し、先にCP/Mでハードの動作検証を行い、その後DOSシステムを動作させる。
<br>
<br>　使用するハード/ソフトを参考まで記載。
<br>　　[lx9-Step-1-io]　　Step-1,2で使用する拡張基盤。市販基板(XC6SLX9 Mini Board)に刺して動作させる。
<br><img width="200" alt="Step-1" src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/159764/3c7e845c-c3a0-6303-06d6-d18d02afaaf1.jpeg">
<br>　　[MAIN-BOARD]　FPGAとDRAMを乗せた基盤。
<br><img width="500" alt="Tang-Nano" src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/159764/f87d2da4-aaef-c7c1-e055-eb6868db76e1.jpeg">
<br>　　[PMOD-IO]　　SDカードとキーボードを繋ぐ基板。MAIN-BOARDに刺す。
<br>　　[PMOD-VGA6]　VGAディスプレイ出力。MAIN-BOARDに刺す。
<br><img width="200" alt="Tang-Nano" src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/159764/b981d67e-58ef-c116-0807-cbbf22ec1e3a.jpeg">
<br>　　[lx9-Step1-CPM80]　CP/Mを動作させる為の回路(verilog)
<br>　　[lx9-Next186_SoC]　DOSを動作させるための回路(verilog)
<br>「[SD2G_Dos_F.zip](https://github.com/hi631/FPGA_DOS/blob/master/SD2G_Dos_F.zip)　free MS-DOS SDイメージ

<br>詳細は　「[Ｑｉｉｔａ](https://qiita.com/hi631/items/e8e0db06a52938b57632)」を見てください。
