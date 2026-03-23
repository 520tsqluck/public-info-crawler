# public-info-crawler
采集指定公开资讯网站的新闻标题、发布时间、来源、正文摘要等，并将数据存储为 CSV 或 JSON 文件。
markdown
# 公开资讯采集爬虫

## 简介
本项目是一个用于采集公开新闻资讯的 Python 爬虫，示例采集新浪国内新闻。代码结构清晰，包含请求、解析、存储模块，并实现了基本的反爬措施。

## 功能特性
- 自动随机 User-Agent
- 请求延时，降低服务器压力
- 支持 CSV 和 JSON 两种数据存储格式
- 模块化设计，易于扩展

## 环境要求
- Python 3.7+
- 依赖库见 `requirements.txt`
- 站大爷代理IP `(https://www.zdaye.com/sepro/xaxzdo)`

## 快速开始
1. 克隆仓库
   ```bash
   git clone https://github.com/你的用户名/public-info-crawler.git
   cd public-info-crawler
创建并激活虚拟环境（可选）

bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
安装依赖

bash
pip install -r requirements.txt
修改配置（如需采集其他网站，请修改 config.py 中的 URL 和选择器）

运行爬虫

bash
python main.py
结果将保存在 data/ 目录下
