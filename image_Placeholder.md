### fixednav �����¼ ###
###����ҳ��ʱ��ѡ�е����ж�Ӧ��Ŀ###

* **��������** ��domready��ͼƬδ�������ʱ�Ѿ�ִ�У����������Ӧê����Ŀ�У���ͼƬwidth:100%���߶Ȳ�ȷ��ʱ������ͼƬδ������ɣ���ʼ��ʱ��ȡ���ĵ���ê���� ''<nowiki>item.offset().top</nowiki>'' �п����Ǵ���ģ������ڹ���ҳ��ʱ���������ǰѡ��ĳ��Ŀ����ʱ��δ��������Ŀ�����ݣ���
* **�������** ����δȷ���߶ȵ�ͼƬռλ����css������img�ĸ���div��padding-top:ͼƬ�߿�ȣ���������img��positionΪabsolute��

* **����ʾ��** ��
<code css>
/*padding-topΪ�߿��=ͼƬ�߶�/ͼƬ���*100 ex:203(imgh)/640(imgw)*100% = 32%*/
.item-pic{padding-top: 32%; display: block; position: relative; z-index: 2;} 
.item-pic img{width: 100%; position: absolute; left: 0; top: 0; z-index: 0;}
</code>