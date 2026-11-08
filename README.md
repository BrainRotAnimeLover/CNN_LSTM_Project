# CNN-LSTM 完整项目

打开 `qlib_tushare_cnn_lstm_ready.ipynb`后运行全部单元。

所有数据和运行文件均在这个项目文件夹内，路径跟随项目位置。整份文件夹可以一起移动，不要单独移走Notebook或数据。

## 文件

- `qlib_tushare_cnn_lstm_ready.ipynb`：完整18特征策略，已保存执行输出和两张收益／回撤图。
- `run_project.py`、`运行完整项目.cmd`：运行入口，使用已安装的quant环境。
- `requirements-quant.txt`：环境依赖清单，当前环境已安装。
- `data/raw/`：完整原始数据。
- `data/processed/`：训练面板 `panel.parquet`、基准、交易日历和数据说明。
- `data/qlib/`：Qlib二进制数据。
- `outputs/`：64个窗口的模型、分数、订单、持仓、指标和图表。

数据覆盖2022-01-04至2026-09-11，1138个交易日、406只历史候选股票、462028行；回测2024-01-02至2026-08-14。全部64个窗口训练成功，两种策略回测完成。

再次运行会复用匹配的分数和结果；修改训练参数后会自动重新训练。组合参数可以在Notebook的CONFIG中调整。增强策略的目录名沿用原项目，实际参数以对应config.json为准。

本项目不需要下载接口密钥，也不依赖恢复脚本或原始Notebook。

## GitHub 仓库说明

本仓库包含 Notebook、项目说明、依赖清单、data/ 中的原始数据、处理后数据和 Qlib 数据，以及 outputs/ 中的训练与回测结果。请保留目录结构，下载完整仓库后按照上述说明运行。


