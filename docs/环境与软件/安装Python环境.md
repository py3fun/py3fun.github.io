# 安装 Python 环境（Windows + Anaconda）

- 下载并安装 Anaconda（64 位 Windows 安装包）。
  - 打开浏览器访问 Anaconda 官方下载页，选择 Windows x86_64 安装器。
  - 安装时一般选择“Just Me”。建议保持默认，不勾选“Add Anaconda to my PATH”，使用 Anaconda Prompt 管理环境。
- 打开 “Anaconda Prompt (Anaconda3)” 并检查版本：
  - `conda --version`
- 关闭 base 自动激活（可选，避免混用 base 环境）：
  - `conda config --set auto_activate_base false`
- 创建并管理 Python 版本（示例：创建 Python 3.11 环境）：
  - 创建：`conda create -n py311 python=3.11 -y`
  - 激活：`conda activate py311`
  - 查看：`conda env list`
  - 安装常用包：`conda install numpy pandas -y` 或使用 `pip install package`
- 切换/退出环境：
  - 切换到其他环境：`conda activate <env_name>`
  - 退出当前环境：`conda deactivate`
- 删除环境（如需）：
  - `conda remove -n py311 --all -y`
