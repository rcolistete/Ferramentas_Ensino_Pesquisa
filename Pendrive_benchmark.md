# Pendrive Benchmark

Benchmark (análise de desempenho) de alguns modelos de pendrives (usb flash drives).

Pendrives recém-formatados com exFAT (sistema de arquivos suportado por Linux, macOS e Windows, sem as limitações de FAT32 de arquivos até 4GB, etc), ou seja, sem arquivos e diretórios. Pois pendrives têm desempenho degradado quanto maior a ocupação de arquivos (principalmente muitos arquivos pequenos) e diretórios.

## Softwares Utilizados

1. (A FAZER) CrystalDiskMark em [Microsoft Windows 10](https://pt.wikipedia.org/wiki/Windows_10) 64 bits, PC desktop com CPU [Intel i7-4770K](https://www.techpowerup.com/cpu-specs/core-i7-4770k.c1459) (2013) e placa-mãe [Asus Z97 Pro Gamer](https://hexus.net/tech/reviews/mainboard/79905-asus-z97-pro-gamer/), em porta USB 3 5 Gbps, usando resultados da 1a linha (SEQ1M Q8T1);
3. [KDiskMark](https://github.com/JonMagon/KDiskMark) em Linux [Manjaro](https://manjaro.org/products/download/x86) KDE 24.0 64 bits, notebook [Dell G3 15 3579-A30P](https://www.dell.com/support/home/pt-br/product-support/product/g-series-15-3579-laptop/docs) (de 12/2018) com CPU [Intel i7 8750H](https://www.techpowerup.com/cpu-specs/core-i7-8750h.c1992) (2018), em porta USB 3 5 Gbps, usando resultados da 1a linha (SEQ1M Q8T1);
4. [AmorphousDiskMark](https://katsurashareware.com/amorphousdiskmark/) em [macOS Sonoma 14.5](https://www.apple.com/macos/sonoma/), notebook [Apple MacBook Air M1 (2020)](https://support.apple.com/pt-br/111883), em porta Thunderbolt 3 40 Gbps com [hub Baseus USB-C 8-in-1 4K 60 Hz USB 3.1](https://www.aliexpress.com/item/1005002191569003.html) com porta USB-A 10 Gbps, usando resultados da 1a linha (SEQ1M QD8).

## Pendrives

1. [32GB Sandisk Cruzer Blade SDCZ50-032G-B35 USB 2.0, cor vermelha e preta](https://www.westerndigital.com/products/usb-flash-drives/sandisk-cruzer-blade-usb-2-0?sku=SDCZ50-032G-B35);
<img src="https://www.westerndigital.com/content/dam/store/en-us/assets/products/usb-flash-drives/cruzer-blade-usb-2-0/gallery/cruzer-blade-usb-2-0-angle.png.wdthumb.320.320.webp" alt="32GB Sandisk Cruzer Blade" style="zoom: 44%;"/>

2. [32GB Kingston DataTraveler Exodia DTX/32GB USB 3.2 Gen1, cor clara/transparente](https://www.kingston.com/br/usb-flash-drives/datatraveler-exodia-usb-3-2-usb-flash-drive);
<img src="https://m.media-amazon.com/images/I/71TB1Ti21uL._AC_SL1500_.jpg" alt="32GB Kingston DataTraveler Exodia" style="zoom: 50%;" />

3. [64GB Kingston DataTraveler Exodia DTX/64GB USB 3.2 Gen1, cor azul](https://www.kingston.com/br/usb-flash-drives/datatraveler-exodia-usb-3-2-usb-flash-drive);
<img src="https://media.kingston.com/kingston/product/ktc-product-usb-dtx-64gb-2-lg.jpg" alt="64GB Kingston DataTraveler Exodia" style="zoom:50%;" />

4. [128GB Kingston DataTraveler Exodia DTX/129GB USB 3.2 Gen1, cor amarela](https://www.kingston.com/br/usb-flash-drives/datatraveler-exodia-usb-3-2-usb-flash-drive);
<img src="https://media.kingston.com/kingston/product/ktc-product-usb-dtx-128gb-2-lg.jpg" alt="64GB Kingston DataTraveler Exodia" style="zoom:50%;" />

5. [256GB Kingston DataTraveler Exodia Onyx DTXON/256GB USB 3.2 Gen1, cor cinza](https://www.kingston.com/br/usb-flash-drives/datatraveler-exodia-onyx-moving-usb-3-2-usb-flash-drive).
<img src="https://media.kingston.com/kingston/product/ktc-product-usb-dtxon-256gb-1-lg.jpg" alt="256GB Kingston DataTraveler Exodia Onyx" style="zoom: 46%;" />

6. [256GB Kingston DataTraveler microDuo 3C DTDUO3CG3/256GB USB-A/USB-C 3.2 Gen1 200MB/s, cor violeta](https://www.kingston.com/br/usb-flash-drives/datatraveler-microduo-3c-g3?capacity=256gb).
<img src="https://i0.wp.com/pokde.net/assets/uploads/2023/10/e-20230710_153611.jpg" alt="256GB Kingston DataTraveler microDuo 3C DTDUO3CG3/256GB" style="zoom: 5%;" />

## Resultados de Desempenho

Os valores são de leitura sequencial e gravação sequencial, em MB/s. Uma medida feita, sem estatística de medidas, sendo esperado ter variação/erro de alguns %.

|            Pendrive             | CrystalDiskMark (MB/s) | KDiskMark (MB/s) | AmorphousDiskMark (MB/s) |
| :-----------------------------: | :--------------------: | :--------------: | :----------------------: |
| Sandisk Cruzer Blade 32GB USB 2 |           -            |     22,7/6,4     |         24,9/4,3         |
|     Kingston DTX/32GB USB 3     |           -            |    117,8/9,2     |        123,6/16,2        |
|     Kingston DTX/64GB USB 3     |           -            |    91,9/14,2     |        94,6/14,1         |
|    Kingston DTX/128GB USB 3     |           -            |    117,5/8,6     |        118,1/21,6        |
|   Kingston DTXON/256GB USB 3    |           -            |     84,8/6,0     |         88,3/5,8         |
| Kingston DTDUO3CG3/256GB USB 3  |           -            |        -         |            -             |

### Análise

- o pendrive USB 2 aqui analisado tem desempenho mais baixo do que o máximo da porta USB 2.0 (480 Mbps, ou aprox. 48 MB/s), principalmente em gravação; 
- mesmo em leitura sequencial, os pendrives USB 3 aqui analisados têm desempenho bem mais baixo do que o máximo da porta USB 3.0 (USB 3.2 Gen 1x1), 5 Gbps (aprox. 500 MB/s). Mas há pendrives USB 3 de alta velocidade, por isso sendo mais caros;
- **em geral os pendrives têm velocidade de gravação bem mais baixa que de leitura**;
- mesmo entre mesma família, Kingston DataTraveler Exodia DTX, o desempenho varia com a capacidade, mas pode variar com o lote de produção, etc;
- o pendrive de 256GB Kingston DataTraveler Exodia Onyx é o mais lento : um pouco em leitura e muito em gravação.

### Recomendação

1. **usar pendrives USB 3 quando o uso principal for leitura de dados**;
2. se for gravar intensivamente em **pendrives USB 3**, atentar para **baixa velocidade de gravação** (abaixo até dos 480 Mbps de USB 2.0) **e** **vida útil mediana** (**10-100 mil ciclos de gravação**, tipicamente);
3. **tem pendrives USB 3 de boas marcas custando em 2024 menos de R$0,50/GB**. Porém os de maior velocidade, com criptografia, etc, custam bem mais do que isso. Vide por exemplo :
   * tabela atual (07/2024) de [pendrives (usb flash drives) da Kingston](https://www.kingston.com/br/usb-flash-drives);
   * matéria ["The Best USB Flash Drives - Wired - 04/02/2024"](https://www.wired.com/gallery/best-usb-flash-drives/);
   * matéria ["Best Flash Drives 2024: Fast, Roomy, Pocketable USB Storage - Tom's Hardware - 18/07/2024"](https://www.tomshardware.com/best-picks/best-flash-drives);
4. SSD externo USB 3 é o mais recomendado para gravação em maior velocidade e maior vida útil (em ciclos de gravação), mas normalmente são mais caros e maiores.
5. Há vários sites com testes extensivos de pendrives, por exemplo :
   * [SSD-Tester - Thumb drive](https://ssd-tester.com/usb_flash_drive_test.php);
   * [UserBenchmark - USB flash drive](https://usb.userbenchmark.com/).

### Autoria e Versões
Autoria : [Roberto Colistete Júnior](https://github.com/rcolistete?).
Licença MIT.
[Link](https://github.com/rcolistete/Ferramentas_Ensino_Pesquisa/Pendrive_benchmark.md) no [repositório GitHub rcolistete / Ferramentas_Ensino_Pesquisa](https://github.com/rcolistete/Ferramentas_Ensino_Pesquisa).

Versões :

- 1.0 em 23/07/2024;
- (A FAZER) 1.1 em 2?/07/2024, com pendrive Kingston DataTraveler microDuo 3C de 256GB;
- (A FAZER) 1.2 em ??/08/2024, com testes no CrystalDiskMark em Windows 10.
