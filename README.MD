# BERTԤѵ��ģ����������ȡ����


BERTԤѵ��ģ����������ȡ����
�汾�� v 0.2.2
����:  2020/3/23

## ����˵��
������ֱ�Ӷ�ȡBERTԤѵ��ģ�ͣ�������ȡ�����ļ�������ʹ�õ�������������������ļ���Ϊ����ģ���ṩembdding��
������ֱ�Ӷ�ȡԤѵ��ģ�ͣ�����Ҫ������������ͬʱ������������
���ֵ��ַ���Ӧ��������ȫ����ȡ��������ģ�Ϳ��Էǳ����ٽ���embdding��
������Ҫ�Ӵ��Ԥѵ��ģ�ͻ���bert-as-service�����ˡ�

## �����ļ���ʽ 

һ��һ���ַ�����,�м�ʹ�ÿո�ָ���
��ʽΪ��

```
�ַ� 768��С����
```

���磺

```
! 0.06241071 -0.012108288 0.035899848....
```


## ����˵��

����˵����
--model_path    BERTԤѵ��ģ�ʹ�ŵ�Ŀ¼�����
--in_file       ����ȡ�������ļ�������Ŀ¼�������
--out_file      ��ȡ�󱣴�������ļ�,��ѡ�Ĭ��Ϊ'./bert_embedding.txt'
--ext           ��ָ��ΪĿ¼ʱ����ѡ�Ҫ�������ļ���׺��Ĭ��Ϊ['csv','txt']

## ʹ������

���������ӣ�

���������ļ�`./data/train_interger.csv`�����浽`./data/need_bertembedding.txt`
```bash
python BERTVector.py \
    --model_path=/mnt/sda1/models/chinese_L-12_H-768_A-12/ \
    --in_file=./data/train_interger.csv \
    --out_file=./data/need_bertembedding.txt

```

����Ŀ¼�µ�����tsv,txt�ļ�,Ĭ�ϱ���Ϊ:./need_bertembedding.txt

```bash
python BERTVector.py \
    --model_path=/mnt/sda1/models/chinese_L-12_H-768_A-12/ \
    --in_file=./data/ \
    --ext tsv txt
```