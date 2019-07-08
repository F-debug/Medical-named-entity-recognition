# Medical-named-entity-recognition
该项目用双向长短时记忆神经网络和条件随机场(Bi-LSTM-CRF)的命名实体识别


# Introduce
data:已标注的医疗数据，O非实体部分,TREATMENT治疗方式, BODY身体部位, SIGN疾病症状, CHECK医学检查, DISEASE疾病实体.  
data_origin:项目提供的医疗数据，需要转化为目标序列标记集合  
transfer_data:目标序列化脚本  
model：训练模型需要的字向量  
<table>
    <tr>
        <th>训练集1</th>
        <th>测试集</th>
        <th>训练集准确率</th>
        <th>测试集准确率</th>
    </tr>
    <tr align="center">
        <td>6268</td>
        <td>1571</td>
        <td>0.965</td>
        <td>0.845</td>
    </tr>
</table>    
 lstm_predict.py:对训练好的实体识别模型进行测试  
 
