# 安装 PyCharm 软件（Windows）

- 下载并安装 PyCharm：
  - 前往 JetBrains 官网下载 PyCharm（Community 社区版或 Professional 专业版）。
  - 按安装向导完成安装，启动 PyCharm。
- 创建新项目并使用 Conda 解释器：
  - Welcome 窗口选择 “New Project”。
  - Location：选择项目保存路径。
  - Python Interpreter：点击右侧设置图标，选择 “Conda Environment”。
    - If existing：选择 “Existing environment”，从下拉框或路径中选择刚才的 `py311` 环境解释器。
    - If new（可选）：也可以让 PyCharm 基于 Conda 创建新环境并指定 Python 版本。
  - 勾选 “Create a main.py welcome script”（可选）。
  - 点击 “Create”。
- 运行测试：
  - 在 `main.py` 中输入 `print("Hello, PyCharm!")`，点击右上角运行按钮或右键 Run 运行。
- 配置终端（可选）：
  - Settings/Preferences → Tools → Terminal，将 Shell path 配置为 Anaconda Prompt 或确保激活项目对应的 Conda 环境。
