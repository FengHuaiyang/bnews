# ����Github��Ŀ���񣬲���ʱͬ���ķ���

˵������Ϊ�����������΢�ſ��������α���Ŀ����ַ�������ƹ�ʱ��̫���㣬�����������һ������Ŀ�ľ��񣬵õ�һ���µ���ַ������ʱͬ������������ƹ㡣

1��ע��һ��github.com�˺ţ�����¼��
2���� https://github.com/fqnews/bnews/blob/master/readme.md
3�������Ͻǵ�Fork���ӣ�fork��ɺ�͵õ���һ�����Լ���git���ŵľ�����ַ��

����fork�ľ��񲻻��Զ�����Դ��Ŀ�����£���ô���أ���2�ְ취:

����1��ÿ���ֹ����£����巽����ɾ��fork����Ŀ������forkһ�£��������µ��ˡ�
��������Fork�����Ŀҳ��Ķ���ƫ�ҵ�λ�ã��и�Setting���ӣ����Setting���Ӻ󣬹�����ҳ��ײ����㡰Delete this repository����ť��ɾ��������Fork���ɡ�

����2����ʱ�Զ�ͬ��
����Ҫһ̨ǽ��ĵ��ԣ�����һ̨VPS,������һ̨Linux(Debian 10) VPSΪ�������ȣ���ssh�ͻ��˵�¼linux��Ȼ��ִ���������
```
apt update
apt install git
```

Ȼ��ʹ�� SSH ���ӵ���� GitHub�˺�(���� SSH ��Կ�������� GitHub����������ÿ�η���ʱ�ṩ�û��������룬���㶨ʱ����git���ž���)
�ο�: 
https://docs.github.com/cn/github/authenticating-to-github/connecting-to-github-with-ssh

Ȼ�� ����ִ���������һ��һ�����ο���ִ�У���
```
cd /root
git config --global core.autocrlf input
git clone git@github.com:your-github-username/bnews.git
cd bnews
chmod +x syncnews.sh
git remote add upstream https://github.com/fqnews/bnews.git
```

Ȼ�����нű��ӵ����linux crontab ���涨ʱִ�м��ɣ�
`/root/bnews/syncnews.sh`

