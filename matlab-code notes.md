2025/3/5  
matlab的linspace函数用于生成指定范围内线性等间距的向量。  
y = linspace(a, b, n)  
其中a为起始值，b为结束值，n（可选）为生成点的总数。  

timeseries 是一种用于存储时间序列数据的对象类型，专门处理随时间变化的数据（如传感器信号、实验测量数据或仿真结果）。它结合了时间向量和对应的数据值，支持数据操作、可视化和分析。  
ts = timeseries(Data, Time)  
其中data是与时间对应的观测值（支持标量、向量、矩阵或多维数组），time是数据点的时间戳（均匀或非均匀分布）  
示例，创建一个包含温度和时间的序列  
time = [0, 1, 2, 3, 4];    % 时间向量（单位：秒）  
temperature = [20, 22, 25, 23, 21]; % 温度数据（单位：°C）  
ts = timeseries(temperature, time, 'Name', 'Temperature');  
ts.DataInfo.Units = '°C';  % 添加单位  




