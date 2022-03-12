# DVA SDK

## developer：开发者方法 <a href="#developer" id="developer"></a>



## core：核心方法 <a href="#core" id="core"></a>



## system：系统交互方法 <a href="#system" id="system"></a>

### os：操作系统

`get_os_type()` (All)：获取操作系统类型

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_os_type())

=====================================================================
{
    "type": "Windows_NT",        // 系统类型
    "platform": "win32",        // 编译名称
    "release": "10.0.19042",    // 系统版本
    "arch": "x64"                // 系统架构
}
```

`get_os_name()` (All)：获取计算机用户名

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_os_name())

=====================================================================
DESKTOP-2PE7ADO
```

`get_cpu_name()` (Windows)： 获取CPU名称

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_cpu_name())

=====================================================================
Intel(R) Core(TM) i7-8700K CPU @ 3.70GHz
```

`get_cpu_ghz()` (Windows)： 获取CPU标定主频（GHz）

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_cpu_ghz())

=====================================================================
3.70GHz
```

`get_cpu_processors()` (All)：获取逻辑处理器个数

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_cpu_processors())

=====================================================================
12
```

`get_cpu_rate()` (All)：获取CPU当前利用率



`get_cpu_speed()` (Windows)：获取CPU当前速度（hz）

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_cpu_speed())

=====================================================================
3962
```

`get_ram_size()` (All)：获取内存大小（B）

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_ram_size())

=====================================================================
68546744320
```

`get_ram_usage()` (All)：获取内存利用率&#x20;

```javascript
let DVA_OS = this.$dva.system.os
console.log(DVA_OS.get_ram_usage())

=====================================================================
0.2728046443854797
```

`list_disk()` (Windows)：列出所有磁盘信息



`get_disk_size(tag)` (Windows)：获取选取磁盘卷标的大小



`get_disk_used(tag)` (Windows)：获取选取磁盘卷标已使用的大小



`get_storage_size()` (iOS / Android)：获取存储空间容量



`get_storage_used()` (iOS / Android)：获取存储空间的已使用容量



`get_clipboard()` (All)：读取剪贴板数据



`set_clipboard()` (All)：设置剪贴板数据



### net: 网络和位置信息

`get_speedtest()` (All)：获取主机网速数据（延迟、上行带宽、下行带宽、网络抖动）



`test_www()` (All)：测试主机是否联网



### media：多媒体设备

`list_speakers()` （Windows）：获取扬声器列表



`list_microphones()` (Windows)：获取麦克风列表



`get_speaker_wave(speaker_name)` (All)：获取扬声器的当前音量



`get_microphone_wave(microphone_name)` (All)：获取麦克风的当前音量



`set_speaker_volume(speaker_name)` (All)：设置扬声器的播放音量



`set_microphone_volume(microphone_name)` (Windows)：设置麦克风的输出音量



`list_cameras()` (All)：获取摄像头列表



调用摄像头拍照并取得返回数据（APP）



以流的形式，获取摄像头实时画面（APP）

### d3：图形设备&#x20;





## data: 数据交互方法 <a href="#data" id="data"></a>



