1.ping另外一台计算机

    这里我ping了我一个新加坡的服务器
    地址是 45.77.255.163

    下面展示cmd的代码：

    C:\WINDOWS\system32>ping 45.77.255.163 -t

    正在 Ping 45.77.255.163 具有 32 字节的数据:
    来自 45.77.255.163 的回复: 字节=32 时间=341ms TTL=50
    请求超时。
    来自 45.77.255.163 的回复: 字节=32 时间=364ms TTL=50
    请求超时。
    来自 45.77.255.163 的回复: 字节=32 时间=352ms TTL=50
    来自 45.77.255.163 的回复: 字节=32 时间=355ms TTL=50
    来自 45.77.255.163 的回复: 字节=32 时间=350ms TTL=50
    来自 45.77.255.163 的回复: 字节=32 时间=351ms TTL=50
    请求超时。
    请求超时。
    来自 45.77.255.163 的回复: 字节=32 时间=362ms TTL=50
    来自 45.77.255.163 的回复: 字节=32 时间=359ms TTL=50
    来自 45.77.255.163 的回复: 字节=32 时间=364ms TTL=50
    请求超时。

    45.77.255.163 的 Ping 统计信息:
        数据包: 已发送 = 14，已接收 = 9，丢失 = 5 (35% 丢失)，
    往返行程的估计时间(以毫秒为单位):
        最短 = 341ms，最长 = 364ms，平均 = 355ms
    

2.tracert一个服务器

    同样的使用以上的地址 ：45.77.255.163
    C:\WINDOWS\system32>tracert 45.77.255.163

    通过最多 30 个跃点跟踪
    到 45.77.255.163.vultr.com [45.77.255.163] 的路由:

    1     4 ms     1 ms     1 ms  192.168.3.1
    2     6 ms     3 ms     3 ms  100.64.0.1
    3    10 ms    11 ms     3 ms  193.31.175.61.dial.nb.zj.dynamic.163data.com.cn [61.175.31.193]
    4    13 ms    12 ms    11 ms  61.153.82.133
    5     *       18 ms    20 ms  202.97.92.33
    6    28 ms     *        *     202.97.94.237
    7    69 ms    81 ms     *     202.97.90.29
    8   231 ms   200 ms   181 ms  202.97.94.10
    9   195 ms   201 ms     *     ae-1.r31.tokyjp05.jp.bb.gin.ntt.net [129.250.2.153]
    10   295 ms   267 ms   272 ms  ae-4.r21.sngpsi07.sg.bb.gin.ntt.net [129.250.2.242]
    11   244 ms   246 ms   252 ms  ae-2.r00.sngpsi07.sg.bb.gin.ntt.net [129.250.3.90]
    12   249 ms   246 ms     *     ae-0.a01.sngpsi07.sg.bb.gin.ntt.net [129.250.2.122]
    13     *      374 ms   371 ms  ae-0.choopa.sngpsi07.sg.bb.gin.ntt.net [116.51.18.134]
    14     *      317 ms   321 ms  10.79.1.161
    15     *        *        *     请求超时。
    16     *        *        *     请求超时。
    17     *      366 ms   366 ms  45.77.255.163.vultr.com [45.77.255.163]

    跟踪完成。