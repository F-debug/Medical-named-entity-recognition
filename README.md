# Medical-named-entity-recognition
该项目用双向长短时记忆神经网络和条件随机场(Bi-LSTM-CRF)的命名实体识别


# Introduce
data:已标注的医疗数据，O非实体部分,TREATMENT治疗方式, BODY身体部位, SIGN疾病症状, CHECK医学检查, DISEASE疾病实体.  
data_origin:项目提供的医疗数据，需要转化为目标序列标记集合  
transfer_data:目标序列化脚本  
model：训练模型需要的字向量  
lstm_train.py:本模型使用预训练字向量,作为embedding层输入,然后经过两个双向LSTM层进行编码,编码后加入dense层,最后送入CRF层进行序列标注.  
| 训练集     | 测试集    | 训练集准确率    | 测试集准确率    |  
| ------------- | :-------------: | :-------------: | -------------: |  
| 6268      | 1571     | 0.965      | 0.845      |    
 lstm_predict.py:对训练好的实体识别模型进行测试  
 
