### AnLayer ʹ��˵��

> ���������

```
import anLayer from '@/components/an-layer/an-layer'

export default {
	components:{
		anLayer
	},
}
```

> ʹ�����

```
<an-layer ref="anRef" autoClose="true" timer="3" type="info">
	<text>Hello Andot</text> <!-- ���Զ�����������Ҳ�Ƿϻ�����֪��{{message}} -->
</an-layer>

//���� ���������autoClose ���Զ��ر�
this.$refs.anRef.show();
//�ر�
this.$refs.anRef.close();
```

> ����

������ | ���� | Ĭ��ֵ | ˵�� | ƽ̨����˵�� 
-|-|-
showPop | Boolean | false | �Ƿ���ʾ�ڸǲ� | ��
direction | String | "top" | �������� | ��
autoClose | Boolean | true | �Ƿ��Զ��رղ� | ��
timer | Number | 2 | �Զ��رյ���ʱ������Ĭ��2�� | ��
type | String | false | �������Ͷ�Ӧ��ͬ��ɫ��info��success�� warn��error��| ��

### 1.1 ���°汾˵��

#### ����show����ֱ�Ӵ�����ʾ��Ϣ����

> ����

���� | ���� | Ĭ��ֵ | ˵�� | ƽ̨����˵�� 
-|-|-
message | String | false | ��show()����ֱ�Ӵ��룬���ȼ��ߣ������ǩҲ�У�show����Ҳ�в�������ʾshow()�������Ϣ | ��

> ʹ�÷���

```
<an-layer ref="anRef" autoClose="true" timer="3" :type="type">
	<text>Hello Andot</text>   <!-- д��show�����Ͳ�Ҫд�����ˣ�����ط�д��д��Ҳ��������ν���������ǿ��֢��д��Ҳû�£�����������ʾ-->
</an-layer>

//���� ���������autoClose ���Զ��ر�
this.$refs.anRef.show(��'Hello Lucas');
//�ر�
this.$refs.anRef.close();

//������ʾЧ��Ϊ Hello Lucas 
```

#### 1.2���°汾˵��

> ���ӵ����������������䶯��

#### 1.3��2019-07-03��

> ����-��show������Ӳ������� 1.1�汾��1.2�汾��һ�����ϰ棬�Ƽ�ʹ��

#### 1.4��2019-07-04��

> �޸����º��ҷ��򵯳����ֵ�bug ��������

#### 1.5��2019-07-05��

> 1���޸�����bug
> 2��������ࡢ�Ҳ൯���ı���
> 3��������ࡢ�Ҳ൯�������ݳ������Խ��й���