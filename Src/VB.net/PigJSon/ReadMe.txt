Piggy JSon ��һ���ǳ��򵥵�JSon���߰���������ҪDLL���ܹ�ʹ�ã�ֻ��Ҫ�� PigJSon.vb ��ӵ� .net ���̾Ϳ��ԡ�
Piggy JSon ���Խ���JSon �� ��װJSon�ַ�����
����JSon �ķ����ǣ������� New PigJSon ʱ��������ʹ�� ParseJSON ������

��ͨ�����غ��� AddEle ���Խ�ԭʼ����������ֵת����JSon�ı����Իس������Ʊ���������ַ����Զ�ת�塣

***Sample code***
pjAssemble = New PigJSon
With pjAssemble
	.AddEle("SiteName", "Soew Phong Web Site", True)    'The first element needs to be explicitly specified
	.AddEle("SiteUrl", "http://www.sewophong.com")  'The default is not the first element
	.AddEle("Describe", "A website for free software" & vbCrLf & " and shareware") 'The text contains a carriage return
	.AddEle("Rank", 168)
	.AddEle("VisitPerDay", CDec(168.88))
	.AddEle("VisitTimeStr", "8/8/2020")
	.AddEle("VisitTime", Now)
	.AddEle("VisitTimeGT", Now, False, False)   'Global time
	.AddSymbol(PigJSon.xpSymbolType.EleEndFlag)
End With
***Return results***
MainJSonStr={"SiteName":"Soew Phong Web Site","SiteUrl":"http://www.sewophong.com","Describe":"A website for free software\r\n and shareware","Rank":"168","VisitPerDay":"168.88","VisitTimeStr":"8/8/2020","VisitTime":"1597765343553","VisitTimeGT":"1597736543556"}
SiteName=Soew Phong Web Site
SiteUrl=http://www.sewophong.com
Rank=168
VisitPerDay=168.88
VisitTimeStr=8/8/2020
VisitTime=2020/8/18 15:42:23
VisitTimeGT=2020/8/18 7:42:23
