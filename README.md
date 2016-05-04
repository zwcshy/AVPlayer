# AVPlayer
基于AVPlayer的自定义播放器
    用AVPlayerLayer封装的基本视频控件，自定义度高~

演示~

基本功能

    屏幕左边上下划动调节屏幕亮度
    屏幕右边上下划动调节音量
    水平划动根据划动速率大小决定视频进退时间的长短
    屏幕跟随设备自动旋转
    可以播放网络视频~当然也可以播放本地视频
    当cell从屏幕消失时视频控件可以置顶或则放置屏幕任意角落~

使用方法
1. 创建Player

ERPlayer *player = [ERPlayer new];

2. 设置Player的Frame或则bounse、center

player.frame = CGRectMake(0, 100, SCREENW, SCREENW / 16 * 9  + 40);

3. 设置Player播放视频的URL

[player setViedoUrl:viedoUrl];

4. 添加到父控件上~

[self.view addSubview:player];

To Do~

    加入弹幕功能
    流媒体
