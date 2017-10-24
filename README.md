Install-Scrapy-For-Python3.X（WIN下）
===========================================
###### how to install scrapy for python3.x


-----------------------------------------------------
  ```
  直接pip3 install Scrapy失败的小伙伴请参考以下教程
  安装Scrapy的3个步骤：
  1.安装wheel
  2.安装lxml
  3.安装Twisted
  4.安装Scrapy
  5.选装pywin32
  ```

-----------------------------------------------------

  1、查看Python版本（确定是python小版本号和32/64位）</br>
  ```
  运行->CMD->
  C:\python
  ```
  
  
  2、下载Lxml、Twisted、Scrapy文件</br>
  下载网址`http://www.lfd.uci.edu/~gohlke/pythonlibs/`，请下载与Python对应的版本：</br>
  例：lxml-4.1.0-cp36-cp36m-win_amd64.whl，表示lxml的版本为4.1.0，对应的python版本为3.6-64bit。</br>
  
  3个文件名如下：</br>
  ```
  lxml-4.1.0-cp36-cp36m-win_amd64.whl</br>
  Scrapy-1.4.0-py2.py3-none-any.whl</br>
  Twisted-17.9.0-cp36-cp36m-win_amd64.whl</br>
  ```
  
  3、切换至安装文件所在目录，依次执行以下命令</br>
  ```
  cd /d e:\Scrapy\</br>
  pip3 install wheel</br>
  pip3 install lxml-4.1.0-cp36-cp36m-win_amd64.whl</br>
  pip3 install Scrapy-1.4.0-py2.py3-none-any.whl</br>
  pip3 install Twisted-17.9.0-cp36-cp36m-win_amd64.whl</br>
  ```
  
  -------------------------------------------------------------
  至此，Scrapy安装完成，可选装pywin32（Scrapy工程报错时），下载地址为（请选择最新版本及对应python版本）：</br>
  
  ```
  https://sourceforge.net/projects/pywin32/files/pywin32/
  ```
  
  
  -------------------------------------------------------------
  `附CMD命令执行结果`
  
  ```
  Microsoft Windows [版本 10.0.15063]
(c) 2017 Microsoft Corporation。保留所有权利。

e:\>cd e:\Scrapy

e:\Scrapy>pip3 install wheel
Collecting wheel
  Downloading wheel-0.30.0-py2.py3-none-any.whl (49kB)
    100% |████████████████████████████████| 51kB 169kB/s
Installing collected packages: wheel
Successfully installed wheel-0.30.0

e:\Scrapy>pip3 install lxml-4.1.0-cp36-cp36m-win_amd64.whl
Processing e:\scrapy\lxml-4.1.0-cp36-cp36m-win_amd64.whl
Installing collected packages: lxml
Successfully installed lxml-4.1.0

e:\Scrapy>pip3 install Twisted-17.9.0-cp36-cp36m-win_amd64.whl
Processing e:\scrapy\twisted-17.9.0-cp36-cp36m-win_amd64.whl
Collecting Automat>=0.3.0 (from Twisted==17.9.0)
  Downloading Automat-0.6.0-py2.py3-none-any.whl
Collecting zope.interface>=4.0.2 (from Twisted==17.9.0)
  Downloading zope.interface-4.4.3-cp36-cp36m-win_amd64.whl (139kB)
    100% |████████████████████████████████| 143kB 808kB/s
Collecting incremental>=16.10.1 (from Twisted==17.9.0)
  Downloading incremental-17.5.0-py2.py3-none-any.whl
Collecting constantly>=15.1 (from Twisted==17.9.0)
  Downloading constantly-15.1.0-py2.py3-none-any.whl
Collecting hyperlink>=17.1.1 (from Twisted==17.9.0)
  Downloading hyperlink-17.3.1-py2.py3-none-any.whl (73kB)
    100% |████████████████████████████████| 81kB 1.5MB/s
Collecting attrs (from Automat>=0.3.0->Twisted==17.9.0)
  Downloading attrs-17.2.0-py2.py3-none-any.whl
Collecting six (from Automat>=0.3.0->Twisted==17.9.0)
  Downloading six-1.11.0-py2.py3-none-any.whl
Requirement already satisfied: setuptools in c:\python\python36\lib\site-packages (from zope.interface>=4.0.2->Twisted==17.9.0)
Installing collected packages: attrs, six, Automat, zope.interface, incremental, constantly, hyperlink, Twisted
Successfully installed Automat-0.6.0 Twisted-17.9.0 attrs-17.2.0 constantly-15.1.0 hyperlink-17.3.1 incremental-17.5.0 six-1.11.0 zope.interface-4.4.3

e:\Scrapy>pip3 install Scrapy-1.4.0-py2.py3-none-any.whl
Processing e:\scrapy\scrapy-1.4.0-py2.py3-none-any.whl
Collecting PyDispatcher>=2.0.5 (from Scrapy==1.4.0)
  Downloading PyDispatcher-2.0.5.tar.gz
Collecting queuelib (from Scrapy==1.4.0)
  Downloading queuelib-1.4.2-py2.py3-none-any.whl
Collecting w3lib>=1.17.0 (from Scrapy==1.4.0)
  Downloading w3lib-1.18.0-py2.py3-none-any.whl
Requirement already satisfied: six>=1.5.2 in c:\python\python36\lib\site-packages (from Scrapy==1.4.0)
Collecting service-identity (from Scrapy==1.4.0)
  Downloading service_identity-17.0.0-py2.py3-none-any.whl
Requirement already satisfied: lxml in c:\python\python36\lib\site-packages (from Scrapy==1.4.0)
Collecting cssselect>=0.9 (from Scrapy==1.4.0)
  Downloading cssselect-1.0.1-py2.py3-none-any.whl
Requirement already satisfied: Twisted>=13.1.0 in c:\python\python36\lib\site-packages (from Scrapy==1.4.0)
Collecting parsel>=1.1 (from Scrapy==1.4.0)
  Downloading parsel-1.2.0-py2.py3-none-any.whl
Collecting pyOpenSSL (from Scrapy==1.4.0)
  Downloading pyOpenSSL-17.3.0-py2.py3-none-any.whl (51kB)
    100% |████████████████████████████████| 51kB 173kB/s
Collecting pyasn1-modules (from service-identity->Scrapy==1.4.0)
  Downloading pyasn1_modules-0.1.5-py2.py3-none-any.whl (60kB)
    100% |████████████████████████████████| 61kB 331kB/s
Requirement already satisfied: attrs in c:\python\python36\lib\site-packages (from service-identity->Scrapy==1.4.0)
Collecting pyasn1 (from service-identity->Scrapy==1.4.0)
  Downloading pyasn1-0.3.7-py2.py3-none-any.whl (63kB)
    100% |████████████████████████████████| 71kB 360kB/s
Requirement already satisfied: incremental>=16.10.1 in c:\python\python36\lib\site-packages (from Twisted>=13.1.0->Scrapy==1.4.0)
Requirement already satisfied: hyperlink>=17.1.1 in c:\python\python36\lib\site-packages (from Twisted>=13.1.0->Scrapy==1.4.0)
Requirement already satisfied: Automat>=0.3.0 in c:\python\python36\lib\site-packages (from Twisted>=13.1.0->Scrapy==1.4.0)
Requirement already satisfied: zope.interface>=4.0.2 in c:\python\python36\lib\site-packages (from Twisted>=13.1.0->Scrapy==1.4.0)
Requirement already satisfied: constantly>=15.1 in c:\python\python36\lib\site-packages (from Twisted>=13.1.0->Scrapy==1.4.0)
Collecting cryptography>=1.9 (from pyOpenSSL->Scrapy==1.4.0)
  Downloading cryptography-2.1.1-cp36-cp36m-win_amd64.whl (1.3MB)
    100% |████████████████████████████████| 1.3MB 142kB/s
Requirement already satisfied: setuptools in c:\python\python36\lib\site-packages (from zope.interface>=4.0.2->Twisted>=13.1.0->Scrapy==1.4.0)
Collecting asn1crypto>=0.21.0 (from cryptography>=1.9->pyOpenSSL->Scrapy==1.4.0)
  Downloading asn1crypto-0.23.0-py2.py3-none-any.whl (99kB)
    100% |████████████████████████████████| 102kB 186kB/s
Collecting idna>=2.1 (from cryptography>=1.9->pyOpenSSL->Scrapy==1.4.0)
  Downloading idna-2.6-py2.py3-none-any.whl (56kB)
    100% |████████████████████████████████| 61kB 172kB/s
Collecting cffi>=1.7; platform_python_implementation != "PyPy" (from cryptography>=1.9->pyOpenSSL->Scrapy==1.4.0)
  Downloading cffi-1.11.2-cp36-cp36m-win_amd64.whl (166kB)
    100% |████████████████████████████████| 174kB 218kB/s
Collecting pycparser (from cffi>=1.7; platform_python_implementation != "PyPy"->cryptography>=1.9->pyOpenSSL->Scrapy==1.4.0)
  Downloading pycparser-2.18.tar.gz (245kB)
    100% |████████████████████████████████| 256kB 246kB/s
Building wheels for collected packages: PyDispatcher, pycparser
  Running setup.py bdist_wheel for PyDispatcher ... done
  Stored in directory: C:\Users\Mar\AppData\Local\pip\Cache\wheels\86\02\a1\5857c77600a28813aaf0f66d4e4568f50c9f133277a4122411
  Running setup.py bdist_wheel for pycparser ... done
  Stored in directory: C:\Users\Mar\AppData\Local\pip\Cache\wheels\95\14\9a\5e7b9024459d2a6600aaa64e0ba485325aff7a9ac7489db1b6
Successfully built PyDispatcher pycparser
Installing collected packages: PyDispatcher, queuelib, w3lib, pyasn1, pyasn1-modules, asn1crypto, idna, pycparser, cffi, cryptography, pyOpenSSL, service-identity, cssselect, parsel, Scrapy
Successfully installed PyDispatcher-2.0.5 Scrapy-1.4.0 asn1crypto-0.23.0 cffi-1.11.2 cryptography-2.1.1 cssselect-1.0.1 idna-2.6 parsel-1.2.0 pyOpenSSL-17.3.0 pyasn1-0.3.7 pyasn1-modules-0.1.5 pycparser-2.18 queuelib-1.4.2 service-identity-17.0.0 w3lib-1.18.0

e:\Scrapy>
  ```
  
