Javaʵ�ֵ�GossipЭ�飬����CassandraV1.1.1Դ���޸�ʵ�֣�����������CassandraԴ�룩����Cassandra��GossipЭ����ز��ֳ�ȡ�˳���������Ҳο���
Ŀ¼�ṹ��cassandraԴ��һ�£�����ΪĿ¼˵����
concurrent:������������.
config:������Ϣ.
gms:gossip�ĺ���ʵ����.
io:���л����.
locator:�¼���������seed�ӿ�.
net:ͨ����أ����ô�ͳ��BIO��ʽ���ɸ�����Ŀ��Ҫ�����Լ���ͨ�ŷ����.
service:���ⲿ���õķ�����gossipЭ��ʹ�÷���ʵ������.
utils:������.

��CassandraԴ����޸���Ҫ������
1. InetAddress����InetSocketAddress������Ϊÿ��ʵ��ָ����ͬ�Ķ˿ڣ����㱾�����ö��ʵ�����ԡ�
2. ȥ������cassandraҵ����ϵ�һЩ��ͷ������Լ������ӿ����˼򻯡�
3. ��ͨ�Ų��֣������Ŀ��Ҫ�������ж�����ͨ�ŷ�����룬ֱ���滻netĿ¼�µ����ӿڼ��ɡ�


���з�����
1. �޸�������ã�
Config���е�3��ip����һ���������3������������ip��
DatabaseDescriptor���е�seed��ip��������һ��������ip
���ߣ�
Config���е�3��listen_adress���ñ���ͬһ��ip���˿ڻ���3����ͬ�Ķ˿ڣ�
DatabaseDescriptor���е�seed��adress��������һ��ip:port

2. run����������:
CassandraDaemon1
CassandraDaemon2
CassandraDaemon3
���ɡ����൱������server�ڵ㣩
����CassandraDaemon1�Ƚ����⣬����ʱ����applicationState���ݣ�ʹonChange�¼������������ڵ���ɲ�����һ�仯��
