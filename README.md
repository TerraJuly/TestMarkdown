# TestMarkdown

# 项目说明
这是一个普通的项目 README，下面是需要被爬取的核心内容：

<!-- RTK title -->
这里是需要被 Python 爬取的核心内容：
1.  项目版本：v1.0.0
2.  发布日期：2026-02-05
3.  核心功能：数据解析、批量爬取
<!-- END_CRAWL_TARGET -->

下面是其他无关内容，无需爬取...

<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>精简版模拟案例网页（爬虫测试专用）</title>
    <style>
        /* 简单样式美化，hidden类视觉隐藏（不影响HTML结构，爬虫可正常解析） */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Microsoft YaHei", sans-serif;
        }
        body {
            padding: 50px;
            background-color: #f5f5f5;
        }
        .case-container {
            background-color: #fff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            max-width: 800px;
            margin: 0 auto;
        }
        h1 {
            color: #333;
            margin-bottom: 30px;
            text-align: center;
        }
        .case-item {
            margin-bottom: 25px;
            padding-bottom: 25px;
            border-bottom: 1px dashed #eee;
        }
        .case-item:last-child {
            border-bottom: none;
            margin-bottom: 0;
            padding-bottom: 0;
        }
        /* hidden类：视觉上隐藏，不占据页面空间，但HTML代码中仍存在 */
        .rtk_case_title_hidden,
        .rtk_case_img_hidden,
        .rtk_case_description_hidden {
            display: none;
        }
        .rtk_case_title {
            color: #2c3e50;
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .rtk_case_img {
            margin: 15px 0;
            border: 1px solid #eee;
            border-radius: 4px;
            overflow: hidden;
        }
        .rtk_case_img img {
            width: 100%;
            height: auto;
            display: block;
        }
        .rtk_case_description {
            color: #666;
            line-height: 1.6;
            font-size: 14px;
        }
    </style>
</head>
<body>
    <div class="case-container">
        <h1>模拟案例展示（爬虫测试）</h1>
        
        <!-- 案例1：核心可展示内容（对应非hidden class） -->
        <div class="case-item">
            <!-- title：非hidden -->
            <div class="rtk_case_title">智能家居系统安装案例</div>
            <!-- img：非hidden（包含绝对路径src） -->
            <div class="rtk_case_img">
                <img src="https://img95.699pic.com/photo/30010/2438.jpg_wh300.jpg!/fh/300/quality/90" alt="智能家居案例图片">
            </div>
            <!-- description：非hidden -->
            <div class="rtk_case_description">本案例为三居室住宅提供全套智能家居解决方案，包含灯光控制、窗帘自动化、安防监控三大模块，实现手机远程操控，提升居住舒适度与安全性。</div>
        </div>
        
        <!-- 案例2：隐藏内容（对应hidden class，视觉不可见，用于爬虫测试提取隐藏内容） -->
        <div class="case-item">
            <!-- title：hidden（仅保留HTML结构，页面不可见） -->
            <div class="rtk_case_title_hidden">工业设备运维监控案例</div>
            <!-- img：hidden（包含相对路径src） -->
            <div class="rtk_case_img_hidden">
                <img src="/images/industrial-monitor.jpg" alt="工业运维案例图片">
            </div>
            <!-- description：hidden（仅保留HTML结构，页面不可见） -->
            <div class="rtk_case_description_hidden">该案例服务于大型工厂生产线，部署无线传感网络，实时监控设备温度、转速等关键参数，异常时自动报警，降低设备停机故障率30%以上。</div>
        </div>
    </div>
</body>
</html>
