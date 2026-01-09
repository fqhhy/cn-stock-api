## 中国股票市场交易接口
### 券商合规接口
1. 券商 QMT
   ```
   小资金使用优先推荐，小券商门槛极低，10w即可开通
   ```
2. PTRADE
   ```
   券商服务器运行
   ```
3. 同花顺 python 接口  https://www.showdoc.com.cn/THSPythonSE/3269126718101134
4. 通达信 python 接口  2025-11-29 内测版
5. 券商自研极速柜台
   ```
   华鑫证券奇点、中泰证券xtp
   ```
6. 第三方技术柜台
   ```
   宽睿OES、华锐ATP、华宝LTS、恒生UFT/UST/LDP、顶点HTS、金证快订、FPGA硬件柜台
   ```

### 模拟客户端交易
1. [ths-android-py](https://github.com/limitget/THS)  开源免费
   ```
   已知问题：
       下单接口数据包解析错误导致死循环
       ftj解析出现死循环，
       minidatahead init时属性错误
       只有下单接口、没用撤单/持仓等接口
   ```
2. [ths-android-java](https://github.com/misslng/10jqka)  开源免费
   ```
   已知问题：
       ftj解析出现溢出问题
       只有登录接口，没有券商登录、下单接口
   ```
3. [ths-pc](https://github.com/panghu1103/trade-api) 收费
   ```
   逆向版本，无源码，不建议使用
   ```

### 模拟网页交易
1. 封装好接口的git仓库
   ```
   https://github.com/wingfirefly/stock  东财，开源免费
   https://github.com/changye/AutoTrade  广发，开源免费
   ```
2. 以下券商支持网页交易
   ```
   https://jy.xzsec.com/Login
   https://weixin.citicsinfo.com/tztweb/hq/index.html
   https://trade2.guosen.com.cn/gxwt/pc/login
   https://xtrade.newone.com.cn/ssologin?t=jykstd
   https://h5jy.gszq.com
   https://m.touker.com/trading/trade/position 
   ```
   
### 交易客户端外挂
1. 模拟键盘点击
   | 客户端 | 仓库 | 优点 | 缺点 |
   | - | - | - | - |
   | Win电脑 | easytrade 等| 最早开源，最知名 | 慢，有验证码 |
   | 安卓 | [THSTrader](https://github.com/nladuo/THSTrader) | 稳定 | 慢 |
2. 使用windows事件

   无开源仓库
3. 内存操作/dll插件
   ```
   代表 https://github.com/zhaoyu162/IsaacTrade， 缺点：不开源，授权授权，使用老版本软件，不稳定。
   ```



## 交流
tg [t.me/fqhhy](https://t.me/fqhhy)


## L2行情接口

| 提供 | 价格 | 缺点 |
| - | - | - |
| qmt | 贵 | 订阅数量少，贵 |
| ptrade | 免费 | 3s一次，不能实时 |
| [未知](https://github.com/Jason4474/L2push) | 中等 | ？？ |
| [客户端插件](https://github.com/zhaoyu162/IssacLv2) | 便宜 | ？？ |
| jvquant | 贵 | |

## L1行情接口
### 券商接口
1. QMT
2. Ptrade
3. 掘金
4. 银河证券星耀数智接口
### 网页接口
1. akshare
2. qq股票、sina股票
3. 东财网页
### 服务商接口
1. gotdx、pytdx
2. thsdk
3. tushare
