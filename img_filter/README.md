# 图片爬取+筛选

## 所需库
pip install umap-learn   
pip install opencv-python   
pip install matplotlib  
pytorch   


  
## 数据加载
修改相应文件的root_dir和file_suffix参数


## 运行   
运行初级数据筛选：
```
python img_primary_filter.py
```   
   
运行高级数据筛选：
```
python img_advanced_filter.py
```   
任务目标：爬取100张花的图片
数据源：baidu
爬取方式：模拟浏览器的方式
数据观察结果：发现一些异常数据还有假花不真实的数据
筛选目标：异常和不真实数据
筛选方式：1、通过提取图像基础信息和特征，并设置阈值来剔除异常数据 2、通过神经网咯对图像进行高层特征提取、降维再筛选出特征不符的图片
筛选结果：第一个方法成功剔除18张图片，第二个方法剔除5张图片
