## C#�е�`IDisposable`�ӿ�

���ȣ�����Ӧ����ȷ��һ���ǣ�`IDisposable`��C#�����ͷŷ��й���Դ��һ�ֽӿڡ�

[MSDN - IDisposable Interface (System)](https://docs.microsoft.com/en-us/dotnet/api/system.idisposable?redirectedfrom=MSDN&view=netframework-4.8)
> The primary use of this interface is to release unmanaged resources. 

��仰�ص�����<u>release</u>��<u>unmanaged</u>���㡣
IDispose�ӿ����������Ҫ�Ķ�λ���ǹ�����CLR���Ƶ���Դ��

---

#### `Dispose()`����������������

 �ںܶ�ʵ����`IDisposable`�ӿڱ�һ���̶��������ˡ�<br />
ֵ��ע���,`Dispose()`����������˵�͵�ͬ��C�����е�`free()`��<br />
�����й���Դ�Ļ�����GC�����ڴ����ʱ��ʱ�����̵���`Dispose()`������ ����
��ֵ��Ϊ`null`�����ܼ�ʱ�����ڴ档

��C++�У���������(Destructor)�����������һ�ຯ��

> a destructor (dtor) is a method which is automatically invoked 
> when the object is destroyed.

C++�����Ե���������������C#һ����`Dispose()`�����������������������ơ�
��Ϊ���������������С���Ⱦ�ԡ���C\+\+����û���������ջ��ƣ����е�
Cleanup��������Ҫ��������ȥ��ɡ�<br />

������C#�У��й���Դ��Cleanup������GCȥ��ɣ�`IDisposable`�ӿ�ֻӦ������
���й���Դ ���ͷš�

C#�����ͷ�Ϊ��ͨ���ͺͷ���ͨ���ͣ�����ͨ���Ͱ�����ͨ����������ͷ��й���Դ��
��ô��������ĳ���ֶλ������Ƿ���ͨ���ͣ���ô�������ҲӦ���Ƿ���ͨ���ͣ�
ҲӦʵ��IDisposable�ӿڡ�

�������`IDisposable`�ӿڵ�**��Ⱦ��**��

>����΢��ı�̹淶����������ʵ����`IDisposable`�ӿڵĶ���
��������ʽ����������Щ�����`Dispose()`���������ͷţ�����������GC���л��ա�
�ڸ��������£���ʹ��`Dispose()`�������õ�ʱ����������жϡ�����C�����й����
`free()` һ���ڴ�һ�������ܻᵼ�����ض����ε��ڴ����

��΢������ೣ�ÿ��ж���`IDisposable`�ӿڵ�����������������һ�㡣



*δ���������*

[Back to HomePage](https://blog.mizumoto.ml)
