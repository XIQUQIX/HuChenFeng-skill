# data/

此目录存放户晨风直播对话的原始文字稿，是知识库的数据来源。

## 目录结构

```
data/
├── 2023年03月/
│   ├── 2023-03-10.md
│   ├── 2023-03-11.md
│   └── README.md
├── 2023年04月/
│   └── ...
└── ...
```

按 `YYYY年MM月` 命名文件夹，每个文件夹下存放对应月份的 .md 文件。

## 文件格式

每个 .md 文件是一场直播的对话转录，格式如下：

```
某网友：你怎么看XXX？
户晨风：我说话直接你别不爱听……
某网友：……
户晨风：……
```

## 数据来源

原始数据来自 [Olcmyk/HuChenFeng](https://github.com/Olcmyk/HuChenFeng)，收录了 2023 年至 2025 年的完整直播文字稿。

克隆后将其内容放入此目录即可：

```bash
git clone https://github.com/Olcmyk/HuChenFeng
cp -r HuChenFeng/* data/
```

## 注意

- `data/` 已加入 `.gitignore`，不会被提交到仓库
- 放入数据后运行 `python tools/build_highlights.py` 重新生成知识库
