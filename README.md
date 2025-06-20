更新命令：


<头>
    <meta charset="UTF-8">
    <title>命令复制示例</title>
    <样式>
        /* 命令容器整体样式 */
        .命令容器 {
            显示：弹性;
            对齐项目：居中;
            width: 500px;
            background-color: #2E3440; /* 深色背景 */
            color: #D8DEE9;           /* 浅色文字 */
            border-radius: 6px;
            padding: 12px;
            margin: 20px 0;
            font-family: "Consolas", "等宽字体", sans-serif;
            font-size: 14px;
        }
        /* 命令文本区域，让文字可选中 */
        .command-text {
            flex: 1;
            white-space: pre; /* 保留换行和空格 */
        }
        /* 复制按钮样式 */
        .复制按钮 {
            背景颜色: #58A6FF;
            颜色: #fff;
            边框：无;
             
            边框半径：4像素;
            光标：指针;
            左边距：12像素;
            过渡：背景颜色 0.2秒；
        输入：}
        .copy-btn:悬停 {
            背景颜色: #3B82F6;
        输入：}
    </样式>
</头部>
<身体>


<div class="命令容器">
    <div class="command-text" id="cmd1">apt-get update</div>
    <按钮 类="复制按钮" 点击="复制命令('命令1')">复制命令</按钮>
</div>


<div class="命令容器">
    <div class="command-text" id="cmd2">apt-get install ash</div>
    <button class="copy-btn" onclick="copyCmd('cmd2')">复制命令</button>
</div>

<脚本>
    // 通用复制函数
    函数 复制命令(元素ID) {
        // 获取命令文本
        常量 命令文本 = 文档.通过ID获取元素(元素ID).内文本;
        
        // 写入剪贴板
        导航器.剪贴板.写入文本(命令文本).然后(() => {
            警报('命令已复制到剪贴板！');
        }).catch(err => {
            控制台.错误('复制失败：', err);
            警报('复制失败，请手动选择复制');
        });
    输入：}
</脚本>

</主体>
  </html>













#ash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/MoeClub/Note/master/InstallNET.sh') -d 9 -v 64 -p 密码






命令中的 -d 后面为 Debian 版本号，-v 后面为 64 位 / 32 位，【7、8、9、10、10】
命令中的 -u 后面为 Ubuntu 版本号，-v 后面为 64 位/32 位，【14.04、16.04、18.04、20.04】


例：bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/MoeClub/Note/master/InstallNET.sh') -d 9 -v 64 -p Sdlw53953
