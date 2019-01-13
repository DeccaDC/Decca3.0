# Decca3.0
Decca is Maven plugin which detects dependency conflict issues between Java projects and third party libraries and assesses the issues’ severity levels to warn developers whether the issues are benign or harmful (e.g., causing runtime exceptions).

建议在Docker环境下使用，jvm虚拟机Xmx参数最好设置为运行电脑的最大（建议大于4000M，例 -Xmx8192m），保持网络连接，docker的images文件过大没有上传。
